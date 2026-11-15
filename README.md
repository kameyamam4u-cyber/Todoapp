# シンプルToDoアプリ

Next.js（App Router）で作ったシンプルなToDoアプリです。

- タスクの追加
- 完了チェック
- 削除

タスクはブラウザの localStorage に保存されます（サーバー・データベース不要）。

## ローカルで動かす

```bash
npm install
npm run dev
```

http://localhost:3000 を開きます。

## Vercelへのデプロイ

### 1. GitHub（kameyamam4u-cyber/Todoapp）にpushする

初回のみ:

```bash
git init
git add .
git commit -m "ToDoアプリを作成"
git branch -M main
git remote add origin https://github.com/kameyamam4u-cyber/Todoapp.git
git push -u origin main
```

2回目以降:

```bash
git add .
git commit -m "変更内容"
git push
```

### 2. Vercelでデプロイする

1. https://vercel.com にGitHubアカウントでログイン
2. 「Add New → Project」で `Todoapp` リポジトリを「Import」
3. 設定は変更せず「Deploy」を押す（Next.jsは自動で認識されます）

以降は `git push` するたびに自動で再デプロイされます。
