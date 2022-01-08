# サービスの概要
【ASTERIA QAサービス】
Asteriaに関するQAを管理するサービス

# 環境情報(lang,package)※requirements.txt参照
Docker20.10.11
Python3.6.9
Django3.2
django-environ0.8.1

# DataBase
sqlite3

# サービス起動(docker-compose.ymlがあるディレクトリで)
「docker-compose up」

またはmanage.pyがあるディレクトリで
「python manage.py runserver」
※こちらは環境を揃える必要があります

※両者とも起動前にsaqmpleに合わせた項目の環境変数(.env)作成は行ってください。

# その他事項
■Linuxを使用している方はDockerにてファイルを生成したらこちらのコマンドで権限を合わせてください(Dockerはrootにしてます)
「sudo chown -R $USER:$USER .」

■環境変数(.env)を追加した場合、.env.sampleにも追加をお願いします。

■Docker コンテナに入るコマンド(docker-compose upした状態で)
「docker-compose exec app bash」