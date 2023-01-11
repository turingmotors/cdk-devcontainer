# Template for AWS CDK

## 使い方

### 1. このリポジトリテンプレートから新規リポジトリを作る。

### 2. CDK アプリケーションを初期化する。

```bash
npx projen new awscdk-app-ts
```

### 3. AWS の認証情報を取得する。

[IAM Identity Center](https://aws.amazon.com/jp/iam/identity-center/) を利用している場合は、SSO の設定が必要。

```bash
aws configure sso --profile default
```

2回目以降は login のみでよい。

```bash
aws sso login
```
