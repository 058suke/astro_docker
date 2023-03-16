# Astro Runs on Docker

静的サイトジェネレーター「[Astro](https://astro.build/)」の開発環境をDockerおよびDocker Composeで立ち上げることができます。

## 使用手順

### コンテナ起動

```sh
docker-compose up -d --build
```

### 開発環境を立ち上げる

以下のコマンドを実行し、ブラウザで`http://localhost:3000`にアクセスすると閲覧可能です。

```sh
docker-compose exec astro npx astro dev --host 0.0.0.0
```

### サイトをビルドする（HTMLやCSSといった静的ファイルにして吐き出す）

```sh
docker-compose exec astro npm run build
```
