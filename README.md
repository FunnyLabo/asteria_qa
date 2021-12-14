############################
## サービスの概要
# ASTERIA QAサービス
Asteriaに関するQAを管理するサービス

## 環境情報(lang,package)
Python3.6.9
Django3.2

## DataBase
sqlite3

## サービス起動(docker-compose.ymlがあるディレクトリで)
- docker-compose up

## Docker コンテナに入るコマンド(docker-compose upした状態で)
- docker-compose exec app bash

## その他事項
### Linuxを使用している方はDockerにてファイルを生成したらこちらのコマンドで権限を合わせてください(Dockerはrootにしてます)
- sudo chown -R $USER:$USER .

############################