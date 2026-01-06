# GitHub Pagesデプロイ手順

## ステップ1: GitHubリポジトリにプッシュ

以下のコマンドを実行してください（YOUR_USERNAME を自分のGitHubユーザー名に置き換えてください）：

```bash
cd ~/job-diagnosis-app
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/job-diagnosis-app.git
git push -u origin main
```

## ステップ2: GitHub Pagesを有効化

1. GitHubのリポジトリページにアクセス
2. 「Settings」タブをクリック
3. 左サイドバーの「Pages」をクリック
4. 「Source」セクションで:
   - Branch: `main` を選択
   - Folder: `/ (root)` を選択
5. 「Save」をクリック

## ステップ3: 公開URLにアクセス

数分後、以下のURLでアプリが公開されます：

```
https://YOUR_USERNAME.github.io/job-diagnosis-app/
```

## トラブルシューティング

- プッシュできない場合: GitHubの認証設定を確認してください
- ページが表示されない場合: 5-10分ほど待ってから再度アクセスしてください
- エラーが出る場合: GitHubのActionsタブでビルドログを確認してください
