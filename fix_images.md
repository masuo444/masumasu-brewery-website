# 画像表示の問題と解決方法

## 問題の原因

1. **日本語ファイル名**: GitHub Pagesで日本語ファイル名が正しく処理されない
2. **大文字小文字の違い**: Windowsでは区別されないが、Linuxサーバーでは区別される
3. **特殊文字**: 一部の特殊文字がURLエンコードされる

## 実施した修正

### 1. ファイル名の変更
- `イメージ画像.png` → `main_image.png`
- `風景.png` → `landscape1.png`
- `風景2.png` → `landscape2.png`

### 2. HTMLの更新
- メインビジュアルの画像パスを修正
- 酒蔵風景の画像パスを修正

## GitHub Pagesでの確認手順

1. ファイルをGitHubにプッシュ
2. ブラウザの開発者ツールでNetworkタブを確認
3. 404エラーが出ている画像を特定
4. 必要に応じて追加修正

## 追加の対策

### キャッシュクリア
```html
<!-- HTMLに追加してキャッシュを無効化 -->
<meta http-equiv="Cache-Control" content="no-cache, no-store, must-revalidate">
<meta http-equiv="Pragma" content="no-cache">
<meta http-equiv="Expires" content="0">
```

### 画像の存在確認JavaScript
```javascript
// 画像の読み込みエラーをチェック
document.addEventListener('DOMContentLoaded', function() {
    const images = document.querySelectorAll('img');
    images.forEach(img => {
        img.addEventListener('error', function() {
            console.log('画像読み込みエラー:', this.src);
            // フォールバック画像を設定
            this.src = 'images/placeholder.png';
        });
    });
});
```

## 一般的なGitHub Pages画像問題の解決方法

1. **ファイル名は英数字のみ使用**
2. **小文字を推奨**
3. **スペースは避けてアンダースコアやハイフンを使用**
4. **相対パスを使用**
5. **画像ファイルのサイズを適切に圧縮**