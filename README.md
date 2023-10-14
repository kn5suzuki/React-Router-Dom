# React-Router-Dom

react-route-domの簡単な動作チェックとSSGとしてデプロイするのを試した

セットアップ
```
docker compose run react-router npm install
```

開発
```
docker compose run --service-ports react-router npm run dev
```

ビルド
```
docker compose run react-router npm run build
```

擬似デプロイ
```
docker compose up
```
