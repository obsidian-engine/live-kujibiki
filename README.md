# 配信用くじ引きアプリ

リアルタイムで複数プレイヤーのくじ引きを管理するWebアプリケーション

## セットアップ

### 1. GitHub Secretsの設定

リポジトリの Settings > Secrets and variables > Actions で以下のシークレットを設定：

- `FIREBASE_API_KEY`
- `FIREBASE_AUTH_DOMAIN`
- `FIREBASE_PROJECT_ID`
- `FIREBASE_STORAGE_BUCKET`
- `FIREBASE_MESSAGING_SENDER_ID`
- `FIREBASE_APP_ID`
- `FIREBASE_MEASUREMENT_ID`

⚠️ **注意**: Firebase APIキーは公開されるため、Firestoreセキュリティルールで適切なアクセス制御を設定してください。

### 2. GitHub Pagesの有効化

1. リポジトリの Settings > Pages
2. Source: "GitHub Actions" を選択
3. Save

### 3. デプロイ

mainブランチにpushすると自動的にGitHub Pagesへデプロイされます。

## 使い方

デプロイ後、以下のURLでアクセス可能：
`https://[username].github.io/[repository-name]/`

ルームを指定する場合：
`https://[username].github.io/[repository-name]/?room=room-name`