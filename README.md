## NestJs, Next.js, Firebaseの開発環境雛形

- すでに必要ファイルはあるので、compose.ymlを使ってコンテナ開発できるようの雛形
- それぞれのコンテナでyarnを行う

```bash
docker compose build

docker compose up
```

### Next.js
下記コマンドで新規作成

```bash
yarn create next-app
```

### NestJS
下記コマンドで新規作成

```bash
npm i -g @nestjs/cli

nest new --strict .
```

### firebase
- 事前にアカウントを用意
  - https://firebase.google.com/?hl=ja
- Authenticationからユーザーを作成

以下のコマンドでfirebaseにログインする

```bash
docker compose run --rm firebase firebase login --no-localhost
```

firebaseの初期化

```bash
docker compose run --rm firebase firebase init
```
