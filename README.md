# 📝 TechLog-app - 学習ログ共有アプリケーション

**TechLog-app** は、日々の学習内容を記録・共有することを目的とした  
Ruby on Rails 製のログアプリです。  
本アプリは [Rails実践ガイド（Muscle Coding）](https://musclecoding.com/rails-practical-guide/) を参考に構築しています。

---

## 🚀 主な機能

- ユーザー認証（Deviseを使用）
- 学習ログの作成・一覧表示・詳細表示・削除
- RSpec + Capybara によるテスト
- Rubocop によるコード品質チェック
- Tailwind CSS によるスタイリング

---

## 🛠 使用技術

| 区分 | 技術 |
|------|------|
| バックエンド | Ruby 3.0.4 / Rails 7.0.x |
| 認証機能 | Devise |
| テスト | RSpec / Capybara |
| 静的解析 | Rubocop（+ Performance / RSpec） |
| スタイリング | Tailwind CSS |
| 環境構築 | rbenv / Bundler |
| バージョン管理 | Git / GitHub |
| CI/CD（予定） | GitHub Actions / Render など |

---

## 📌 開発状況（2025年6月現在）

- ✅ Devise によるログイン/サインアップ機能の実装完了
- ✅ 学習ログのCRUD機能 完成
- ✅ 基本的なテストコード実装（RSpec + System Spec）
- ✅ Rubocop によるコード整備完了
- ⬜️ UI改善 / エラーハンドリング強化予定
- ⬜️ CI/CDパイプラインの構築予定

---

## 📁 ディレクトリ構成（例）

```bash
.
├── app/                  # モデル・コントローラー・ビュー
├── config/               # ルーティング・設定ファイル
├── spec/                 # RSpecテスト
├── .github/              # Issue・PRテンプレート
│   ├── ISSUE_TEMPLATE.md
│   └── PULL_REQUEST_TEMPLATE.md
├── .rubocop.yml          # コードスタイル設定
└── README.md

---

🚀 セットアップ方法
# Rubyインストール（rbenv使用）
rbenv install 3.0.4
rbenv local 3.0.4

# Bundler設定・インストール
bundle config set path '.bundle'
bundle install

# TailwindCSSなど必要な初期セットアップ
bundle exec rails importmap:install
bundle exec rails tailwindcss:install

# サーバー起動
bundle exec rails server
ブラウザで http://localhost:3000 にアクセスして確認してください。

---

🧪 テストの実行
bin/rspec
エラーがなければ、テストは正常に通過しています。

---

📄 ライセンス
MIT License

📚 参考資料
Muscle Coding: Rails実践ガイド

Devise / RSpec / Tailwind CSS 公式ドキュメント

Rubocop スタイルガイド
