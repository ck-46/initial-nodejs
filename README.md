# Node.js アプリケーションを作成する

Node.js Web アプリケーションを Docker 化する

## 環境構築

### 1. Dockerfile からイメージをビルド
```
docker build . -t ck-46/node-web-app
```

### 2. イメージをコンテナとして実行する
```
docker run -p 49150:8080 -d ck-46/node-web-app
```

## その他のコマンド

### コンテナ内に入る
```
docker exec -it <container id> /bin/bash
```

### アプリを呼び出す
```
curl -i localhost:49150
```

## 参考ドキュメント
https://nodejs.org/ja/docs/guides/nodejs-docker-webapp/
