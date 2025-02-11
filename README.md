# PayPay 家計簿 Webアプリ

## 📌 概要
PayPayの決済情報を取得し、家計簿のように管理できるWebアプリです。支出の可視化やカテゴリ分類、検索機能を備え、日々の支出管理をより簡単にします。

---

## 🎯 機能一覧
### ✅ データ取得
- **PayPay API** から決済情報を取得（APIキーが必要）
- **CSVインポート対応**（手動でデータを追加可能）

### ✅ データ表示
- 日付ごとの支出一覧
- カテゴリ別支出の可視化（グラフ表示）
- 月ごとの支出合計

### ✅ フィルタ・検索機能
- 日付・カテゴリでの検索
- 金額範囲でのフィルタ

### ✅ アカウント管理
- Google認証などのログイン機能
- ユーザーごとのデータ保存

---

## 🛠 技術構成

| **コンポーネント** | **技術** |
|------------------|------------------|
| フロントエンド | React + Next.js or Vue.js + Nuxt.js |
| バックエンド | FastAPI（Python） or Express（Node.js） |
| データベース | Firebase Firestore / PostgreSQL / MySQL |
| データ可視化 | Recharts / Chart.js / D3.js |
| 認証管理 | Firebase Authentication / OAuth |
| デプロイ | Vercel / Netlify（フロント）<br>Railway / Render / AWS Lambda（バックエンド） |

---

## 🚀 開発フロー

### **1. PayPay APIの調査**
- 公式ドキュメントを確認し、決済履歴取得APIがあるかチェック
- OAuth認証が必要か調査

### **2. バックエンド開発**
- PayPayのデータ取得機能（API or CSVインポート）
- データベース設計と保存処理の実装
- APIエンドポイントの設計（支出データ取得・カテゴリ管理）

### **3. フロントエンド開発**
- 支出一覧の表示
- グラフでの可視化
- フィルタ・検索機能の実装

### **4. ユーザー認証の実装**
- Firebase Authentication / OAuthでユーザー管理

### **5. デプロイ & テスト**
- フロントエンド（Vercel / Netlify）
- バックエンド（Railway / Render / AWS Lambda）
- バグ修正・動作確認

---

## 💡 追加機能（今後の展開）
- **カテゴリの自動分類**（「食費」「交通費」などの分類をAIで自動化）
- **予算管理機能**（月ごとの支出上限を設定し、通知）
- **レシート読み取り機能**（OCRを使い、画像からデータを取得）

---

## 📌 使い方（予定）
1. **ログイン**（Google認証など）
2. **PayPayデータを取得 or CSVをアップロード**
3. **支出データを一覧表示・グラフで可視化**
4. **カテゴリごとに管理・検索・フィルタリング**
5. **月の支出を分析し、予算を管理**

---

## 🎯 今後のタスク
- [ ] PayPay APIの利用可否を確認
- [ ] バックエンドの設計（DB & API）
- [ ] フロントエンドのUI設計
- [ ] 基本機能の実装
- [ ] ユーザー認証の追加
- [ ] デプロイ & 運用開始

---

## 📢 ライセンス
MIT License

