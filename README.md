# React-Router-Dom

react-route-dom の簡単な動作チェックと SSG としてデプロイするのを試した

セットアップ

```
docker compose run --rm react-router npm install
```

開発

```
docker compose run --rm --service-ports react-router npm run dev
```

ビルド

```
docker compose run --rm react-router npm run build
```

擬似デプロイ

```
docker compose up
```
