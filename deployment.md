# GitHub Pagesへのデプロイ手順

## 1. GitHubリポジトリの作成

1. GitHubにログイン
2. 新しいリポジトリを作成
   - リポジトリ名: `masumasu-brewery-website`
   - 公開設定: Public
   - README.mdを含める: チェックしない（既に存在するため）

## 2. ローカルファイルをGitHubにプッシュ

```bash
# フォルダに移動
cd /Users/masuo/Desktop/蔵元/masumasu-brewery-website

# Gitリポジトリを初期化
git init

# ファイルをステージング
git add .

# コミット
git commit -m "初回コミット: 益々酒造ウェブサイト"

# リモートリポジトリを追加
git remote add origin https://github.com/YOUR_USERNAME/masumasu-brewery-website.git

# メインブランチに変更
git branch -M main

# GitHubにプッシュ
git push -u origin main
```

## 3. GitHub Pagesの設定

1. GitHubのリポジトリページに移動
2. **Settings** タブをクリック
3. 左サイドバーの **Pages** をクリック
4. **Source** セクションで：
   - "Deploy from a branch" を選択
   - Branch: "main" を選択
   - Folder: "/ (root)" を選択
5. **Save** をクリック

## 4. デプロイの確認

- 数分後、サイトが以下のURLで公開されます：
  `https://YOUR_USERNAME.github.io/masumasu-brewery-website`

## 5. カスタムドメインの設定（オプション）

独自ドメインを使用する場合：

1. ドメインのDNS設定でCNAMEレコードを設定
2. CNAMEファイルにドメイン名を記載
3. GitHub Pagesの設定でカスタムドメインを指定

## 6. 更新方法

ファイルを更新した後：

```bash
git add .
git commit -m "更新内容の説明"
git push
```

自動的にGitHub Pagesに反映されます。

## トラブルシューティング

### 画像が表示されない場合
- ファイル名の大文字小文字を確認
- パスが正しいか確認
- ファイルが正しくアップロードされているか確認

### CSSが適用されない場合
- `style.css` のパスを確認
- ブラウザのキャッシュをクリア

### 404エラーが発生する場合
- `index.html` がルートディレクトリにあるか確認
- GitHub Pagesの設定を再確認