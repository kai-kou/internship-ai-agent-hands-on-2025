# GitHub Pages 手動設定手順（詳細版）

## 📋 事前準備

- ✅ リポジトリがパブリックになっている
- ✅ `docs/handson-36g33suk`フォルダがコミットされている
- ✅ `docs/.nojekyll`ファイルが存在する

---

## 🚀 手動設定手順（ステップバイステップ）

### Step 1: GitHubリポジトリにアクセス

1. ブラウザでGitHubにログイン
2. 以下のURLにアクセス：
   ```
   https://github.com/aainc/internship-ai-agent-hands-on-2025
   ```

### Step 2: Settingsページに移動

1. リポジトリページの上部にあるタブメニューを確認
   - 「Code」「Issues」「Pull requests」「Actions」「Projects」「Wiki」「Security」「Insights」などが表示されています
2. 右端の **「Settings」** タブをクリック
   - リポジトリ名の右側にあります

### Step 3: Pages設定ページに移動

1. 左サイドバーのメニューをスクロール
2. **「Code and automation」** セクションを探す
3. **「Pages」** をクリック
   - 「Pages」は「Environments」の下にあります

### Step 4: Source設定

1. **「Source」** セクションを確認
   - ページ上部に「Build and deployment」という見出しがあります
   - その下に「Source」セクションがあります

2. **「Deploy from a branch」** が選択されていることを確認
   - デフォルトで選択されているはずです
   - 選択されていない場合は、ラジオボタンをクリック

3. **「Branch」** ドロップダウンをクリック
   - `main` を選択
   - 他のブランチが表示される場合は、`main`を選択してください

4. **「Folder」** ドロップダウンをクリック
   - `/ (root)` がデフォルトで選択されている可能性があります
   - `/docs` を選択してください
   - ドロップダウンに `/docs` が表示されない場合は、一度保存してから再度確認してください

5. **「Save」** ボタンをクリック
   - ページ上部または下部にある「Save」ボタンをクリック

### Step 5: 設定の確認

1. 設定が保存されると、ページ上部に以下のようなメッセージが表示されます：
   ```
   Your site is ready to be published at:
   https://aainc.github.io/internship-ai-agent-hands-on-2025/
   ```
   または
   ```
   Your site is live at:
   https://aainc.github.io/internship-ai-agent-hands-on-2025/
   ```

2. **「Visit site」** ボタンが表示される場合があります
   - これはデプロイが完了したことを示します

### Step 6: デプロイの待機

1. 初回デプロイには数分かかります（通常1-5分）
2. ページ上部にデプロイ状況が表示されます：
   - 「Your site is being built from the latest commit」
   - 「Your site is live at: ...」
3. デプロイが完了するまで待機してください

### Step 7: デプロイ状況の確認

1. **「Actions」** タブをクリックしてデプロイログを確認できます
2. 左サイドバーに **「pages build and deployment」** というワークフローが表示されます
3. 緑色のチェックマークが表示されれば、デプロイ成功です

---

## 🔗 公開URLの確認

### ベースURL

設定が完了すると、以下のベースURLでアクセスできます：

```
https://aainc.github.io/internship-ai-agent-hands-on-2025/
```

### スライドのURL

実際のスライドは以下のURLでアクセスできます：

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
- [ ] 画像が正しく表示される（`assets/`フォルダ内の画像）
- [ ] スライドのナビゲーションが動作する（矢印キー、マウス操作）
- [ ] robots.txtが正しく機能している
- [ ] URLが難読化されている（`handson-36g33suk`）

### robots.txtの確認

ブラウザで以下のURLにアクセス：

```
https://aainc.github.io/internship-ai-agent-hands-on-2025/handson-36g33suk/robots.txt
```

以下の内容が表示されればOK：

```
User-agent: *
Disallow: /
```

---

## ⚠️ 組織制限がある場合の対処法

### エラーメッセージが表示される場合

以下のようなエラーメッセージが表示される場合：

- 「GitHub Pages is disabled for this repository」
- 「Organization administrators disabled Pages creation」
- 「You don't have permission to enable Pages」

### 対処方法

1. **組織の管理者に連絡**
   - 組織のSettings > Pages で「Allow members to publish sites」を有効化してもらう

2. **組織の設定を確認**
   - 組織の管理者権限がある場合は、組織のSettings > Pages を確認

3. **代替案を検討**
   - Netlify、Vercel、Cloudflare Pagesなどの外部ホスティングサービスを使用

---

## 🔧 トラブルシューティング

### デプロイが完了しない場合

1. **「Actions」タブでログを確認**
   - エラーメッセージを確認
   - デプロイが失敗している場合は、エラー内容を確認

2. **ファイルの存在を確認**
   - `docs/handson-36g33suk/slides/index.html` が存在するか確認
   - `docs/.nojekyll` が存在するか確認

3. **ブランチを確認**
   - `main`ブランチに`docs`フォルダが存在するか確認

### 404エラーが表示される場合

1. **URLが正しいか確認**
   - `handson-36g33suk`のスペルを確認
   - 大文字小文字を確認

2. **デプロイが完了しているか確認**
   - 「Actions」タブでデプロイ状況を確認
   - デプロイが完了するまで数分待つ

3. **ファイルパスを確認**
   - `docs/handson-36g33suk/slides/index.html` のパスが正しいか確認

### 画像が表示されない場合

1. **画像ファイルの存在を確認**
   - `docs/handson-36g33suk/assets/` に画像ファイルが存在するか確認

2. **相対パスを確認**
   - HTMLファイル内の画像パスが正しいか確認
   - 相対パスが正しく設定されているか確認

---

## 📞 サポート

設定で困った場合は、以下を確認してください：

- GitHub Pagesの公式ドキュメント: https://docs.github.com/ja/pages
- リポジトリの「Actions」タブでデプロイログを確認
- 組織の管理者に連絡（組織制限がある場合）

---

**最終更新日**: 2025年11月13日

