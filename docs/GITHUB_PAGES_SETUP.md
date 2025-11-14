# GitHub Pages設定手順（手動設定）

## 📋 概要

このリポジトリの`docs/handson-36g33suk`フォルダをGitHub Pagesで公開します。

**公開URL**: `https://aainc.github.io/internship-ai-agent-hands-on-2025/handson-36g33suk/slides/`

## 🔒 セキュリティ対策

### 1. 検索インデックス対策

- ✅ `robots.txt`でクロールを拒否
- ✅ HTMLに`noindex`メタタグを追加
- ✅ `.nojekyll`ファイルでJekyll処理を無効化

### 2. URL難読化

- ✅ フォルダ名を`handson-36g33suk`に変更（推測しにくい文字列）

---

## 🚀 手動設定手順（詳細）

### Step 1: GitHubリポジトリにアクセス

1. ブラウザでGitHubにログイン
2. 以下のリポジトリにアクセス：
   ```
   https://github.com/aainc/internship-ai-agent-hands-on-2025
   ```

### Step 2: Settingsページに移動

1. リポジトリページの上部メニューから **「Settings」** をクリック
   - リポジトリ名の右側にあるタブメニューから選択

### Step 3: Pages設定に移動

1. 左サイドバーの **「Pages」** をクリック
   - 「Code and automation」セクション内にあります

### Step 4: Sourceを設定

1. **「Source」** セクションで以下を設定：
   - **「Deploy from a branch」** を選択（デフォルトで選択されているはず）
   - **「Branch」**: `main` を選択
   - **「Folder」**: `/docs` を選択
     - ドロップダウンから `/docs` を選択してください

2. **「Save」** ボタンをクリック

### Step 5: 設定の確認

設定が正しく反映されると、以下のように表示されます：

```
Your site is live at:
https://aainc.github.io/internship-ai-agent-hands-on-2025/
```

**注意**: 初回デプロイには数分かかる場合があります。

### Step 6: デプロイ状況の確認

1. **「Pages」** ページの上部にデプロイ状況が表示されます
2. **「Visit site」** ボタンが表示されたら、デプロイが完了しています
3. デプロイが完了するまで数分待ってください（通常1-3分）

---

## 🔗 公開URL

### スライドのURL

設定が完了すると、以下のURLでアクセスできます：

```
https://aainc.github.io/internship-ai-agent-hands-on-2025/handson-36g33suk/slides/
```

### スライドの直接リンク

```
https://aainc.github.io/internship-ai-agent-hands-on-2025/handson-36g33suk/slides/index.html
```

---

## ✅ 動作確認チェックリスト

デプロイ完了後、以下を確認してください：

- [ ] スライドが正常に表示される
- [ ] 画像が正しく表示される
- [ ] スライドのナビゲーションが動作する
- [ ] robots.txtが正しく機能している（検索エンジンでインデックスされない）
- [ ] URLが難読化されている

### robots.txtの確認方法

ブラウザで以下のURLにアクセスして、内容が表示されることを確認：

```
https://aainc.github.io/internship-ai-agent-hands-on-2025/handson-36g33suk/robots.txt
```

以下の内容が表示されればOK：

```
User-agent: *
Disallow: /
```

---

## 📝 注意事項

### プライベートリポジトリの場合

- **プライベートリポジトリでは、GitHub Pagesは有料プラン（GitHub Pro、Team、Enterprise）が必要です**
- 無料プランでGitHub Pagesを使用する場合は、リポジトリをパブリックにする必要があります
- リポジトリをパブリックにする場合：
  1. **Settings** > **General** に移動
  2. ページ下部の **「Danger Zone」** セクションで **「Change visibility」** をクリック
  3. **「Make public」** を選択して確認

### セキュリティについて

- **URLは推測しにくいですが、完全に秘密ではありません**
- URLを知っている人はアクセスできます
- `robots.txt`と`noindex`メタタグで検索エンジンへのインデックスは防げますが、URLが漏れた場合はアクセス可能です
- より厳格なアクセス制御が必要な場合は、認証機能の追加を検討してください

---

## 🔧 トラブルシューティング

### デプロイが完了しない場合

1. **「Actions」** タブでデプロイのログを確認
2. エラーメッセージを確認
3. `docs`フォルダが正しくコミットされているか確認

### 404エラーが表示される場合

1. URLが正しいか確認（`handson-36g33suk`のスペル）
2. ファイルパスが正しいか確認
3. デプロイが完了しているか確認（数分待つ）

### 画像が表示されない場合

1. 画像ファイルが`docs/handson-36g33suk/assets/`に存在するか確認
2. 相対パスが正しいか確認

---

## 📞 サポート

設定で困った場合は、以下を確認してください：

- GitHub Pagesの公式ドキュメント: https://docs.github.com/ja/pages
- リポジトリの「Actions」タブでデプロイログを確認

---

**最終更新日**: 2025年11月13日

