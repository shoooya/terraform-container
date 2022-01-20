# terraform
build_career用terraform

# 使い方
## 事前準備
### 接続情報を設定
* `.env.example`をコピーし、対象アカウントに接続できる `ACCESS_KEY` `SECRET_ACCESS_KEY` を追加

## 起動
```
$ docker-compose up -d
```

## コンテナ内に接続
```
$ docker-compose exec terraform bash
```

# 初回環境構築時のみ実行する作業
## terraformのバックエンドに利用するS3バケットを作成
* terraformが状態を持つためのファイルが格納されます

## cloudwatch logsのロググループを作成
* コンテナからの標準出力が吐かれる場所となります
