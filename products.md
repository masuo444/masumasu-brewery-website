# 商品情報詳細

## 商品フォルダ構成

各商品フォルダ（`products/` 内）には以下のファイルが含まれています：

### ファイル構成
- **画像ファイル**: `[番号].png` - 商品の画像
- **商品情報**: `商品情報.txt` - 基本的な商品データ
- **一般向けQA**: 
  - `[銘柄名]_一般向けQA.csv` - CSV形式
  - `[銘柄名]_一般向けQA.html` - ブラウザ表示用
  - `[銘柄名]_一般向けQA.json` - API用データ
- **プロ向けQA**:
  - `[銘柄名]_プロ向けQA.csv` - CSV形式
  - `[銘柄名]_プロ向けQA.html` - ブラウザ表示用
  - `[銘柄名]_プロ向けQA.json` - API用データ

## 商品ラインナップ詳細

### 1. 純米大吟醸「益々」/ Masu Masu - Zenith
- **種別**: 純米大吟醸
- **精米歩合**: 35%
- **アルコール度数**: 16%
- **価格**: 720ml：¥8,800
- **特徴**: 年間500本限定、最高峰の技術
- **フォルダ**: `products/1_純米大吟醸益々/`

### 2. 純米吟醸「益々」/ Masu Masu - Fragrance
- **種別**: 純米吟醸
- **精米歩合**: 50%
- **アルコール度数**: 15.5%
- **価格**: 720ml：¥3,500 / 1.8L：¥6,800
- **特徴**: フルーティーな香り
- **フォルダ**: `products/2_純米吟醸益々/`

### 3. 特別純米酒「益々」/ Masu Masu - Tradition
- **種別**: 特別純米酒
- **精米歩合**: 60%
- **アルコール度数**: 15%
- **価格**: 720ml：¥2,800 / 1.8L：¥5,400
- **特徴**: 伝統的な味わい
- **フォルダ**: `products/3_特別純米酒益々/`

### 4. 本醸造「益々」/ Masu Masu - Classic
- **種別**: 本醸造
- **精米歩合**: 65%
- **アルコール度数**: 15%
- **価格**: 720ml：¥2,200 / 1.8L：¥4,200
- **特徴**: 日常の晩酌に最適
- **フォルダ**: `products/4_本醸造益々/`

### 5. にごり酒「益々」/ Masu Masu - Cloud
- **種別**: にごり酒
- **精米歩合**: 70%
- **アルコール度数**: 14%
- **価格**: 720ml：¥3,000
- **特徴**: 冬季限定、クリーミーな口当たり
- **フォルダ**: `products/5_にごり酒益々/`

### 6. スパークリング清酒「益々」/ Masu Masu - Celebration
- **種別**: スパークリング
- **アルコール度数**: 12%
- **価格**: 720ml：¥4,500
- **特徴**: 乾杯シーンに最適
- **フォルダ**: `products/6_スパークリング清酒益々/`

### 7. 貴醸酒「益々」/ Masu Masu - Noble
- **種別**: 貴醸酒
- **精米歩合**: 60%
- **アルコール度数**: 17%
- **価格**: 500ml：¥7,000
- **特徴**: デザート酒、濃厚な甘み
- **フォルダ**: `products/7_貴醸酒益々/`

### 8. 古酒「益々」/ Masu Masu - Vintage
- **種別**: 古酒 (純米)
- **精米歩合**: 65%
- **アルコール度数**: 18%
- **価格**: 720ml：¥12,000
- **特徴**: 数量限定、5年以上熟成
- **フォルダ**: `products/8_古酒益々/`

### 9. 季節限定酒「益々」/ Masu Masu - Seasonal
- **種別**: 純米吟醸 生原酒
- **精米歩合**: 55%
- **アルコール度数**: 17%
- **価格**: 720ml：¥3,800
- **特徴**: 春季限定、フレッシュな味わい
- **フォルダ**: `products/9_季節限定酒益々/`

### 10. 梅酒「益々」/ Masu Masu - Plum
- **種別**: リキュール (梅酒)
- **アルコール度数**: 12%
- **価格**: 720ml：¥3,200
- **特徴**: 純米酒ベース、上品な甘さ
- **フォルダ**: `products/10_梅酒益々/`

## QAシステムについて

### 一般向けQA（8項目）
1. 基本情報 - 冷やして飲むのがいいか
2. 飲み方 - 燗にしても美味しいか
3. 料理との相性 - 合う料理について
4. 保存方法 - 開封後の日持ち
5. 種類 - 純米酒と本醸造の違い
6. 酒米 - 使用している酒米について
7. 味の特徴 - 甘口か辛口か
8. アルコール度数 - 度数について

### プロ向けQA（11項目）
1. 製造工程 - 使用酵母
2. 製造工程 - 火入れ回数
3. 製造工程 - もろみ期間
4. 製造工程 - 搾り方法
5. 科学データ - 日本酒度
6. 科学データ - 酸度・アミノ酸度
7. 科学データ - 香り成分
8. 科学データ - ガス感の有無
9. 熟成・保管 - 熟成期間
10. 熟成・保管 - 保存推奨温度
11. 輸出・認証 - 海外輸出について