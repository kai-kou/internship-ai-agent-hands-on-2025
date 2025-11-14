# AIエージェント開発ハンズオン 2025

インターン向けAIエージェント開発ハンズオンの資料リポジトリです。

---

## 📋 プロジェクト概要

このリポジトリには、AIエージェント（Cursor/Windsurf）を使ったWebアプリケーション開発ハンズオンの資料が含まれています。

参加者は、AIエージェントと対話しながらECサイトを構築し、バイブコーディング（AIとの協働開発）を体験します。

---

## 📁 ディレクトリ構成

```
.
├── docs/
│   ├── handson-36g33suk/  # ハンズオン本番資料（GitHub Pages公開用）
│   │   ├── assets/        # 画像ファイル
│   │   ├── setup/         # 環境構築手順
│   │   └── slides/        # スライド資料
│   ├── sample/            # サンプルコード・資料（GitHub Pages公開用）
│   ├── planning/          # 企画資料（Git除外）
│   └── presentation/      # 発表資料テンプレート
```

---

## 🚀 クイックスタート

### 1. 環境構築

ハンズオンで使用する開発環境の構築手順は以下を参照してください：

👉 [環境構築手順](./docs/handson/setup/README.md)

**推奨ツール**: Cursor（またはWindsurf）

### 2. スライド資料の確認

ハンズオンのスライド資料は以下で確認できます：

👉 [スライド資料](./docs/handson-36g33suk/slides/index.html)

ローカルで確認する場合：

```bash
cd docs/handson-36g33suk/slides
python3 -m http.server 8000
# ブラウザで http://localhost:8000 にアクセス
```

### 3. サンプルコードの確認

完成例のサンプルコードは `docs/sample/` フォルダにあります。

---

## 📚 主要な資料

### ハンズオン資料

- **[環境構築手順](./docs/handson-36g33suk/setup/README.md)**: Cursor/Windsurfのインストール手順
- **[スライド資料](./docs/handson-36g33suk/slides/index.html)**: ハンズオンのスライド（Reveal.js）
- **[発表資料テンプレート](./docs/presentation/template.md)**: 発表で使用するテンプレート

### サンプル

- **[サンプルECサイト](./docs/sample/index.html)**: 完成例のコード
- **[実装レポート例](./docs/sample/docs/implementation-report.md)**: 実装レポートのサンプル
- **[発表資料例](./docs/sample/docs/presentation.md)**: 発表資料のサンプル

---

## 🛠️ 使用技術

- **AIエージェントIDE**: Cursor / Windsurf
- **API**: [FakeStoreAPI](https://fakestoreapi.com/)
- **フロントエンド**: HTML, CSS, JavaScript（Vanilla JS）
- **スライド**: Reveal.js

---

## 📝 注意事項

- `docs/planning/` フォルダはGitのコミット対象外です（企画資料のため）
- サンプルコードは参考用です。ハンズオンでは自分で作成してください

---

## 🔗 参考リンク

- **FakeStoreAPI公式ドキュメント**: https://fakestoreapi.com/docs
- **Cursor公式サイト**: https://cursor.com/
- **Windsurf公式サイト**: https://www.windsurf.dev/

---

## 📞 サポート

ハンズオン当日は、運営スタッフがサポートします。お気軽にご質問ください！

---

**最終更新日**: 2025年11月13日

