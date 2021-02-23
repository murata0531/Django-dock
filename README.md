# Django-dock

コンテナ立ち上げ

```
$ docker-compose up -d
```

コンテナとイメージ破棄

```
$ docker-compose down --rmi all --volumes --remove-orphans
```

mysqlを確認

```
mysqlが動いているコンテナの名前(NAMES)を確認

$ docker ps

コンテナに入る

docker exec -it コンテナ名 bash


mysqlのバージョンを確認

bash# mysql -V
```

構築

setiing.pyと同じ階層にsetting_local.pyを作成し、キーを格納する

↓キーはここから生成↓

djangoキージェネレーター
https://miniwebtool.com/ja/django-secret-key-generator/

```
$ docker-compose up -d
```

windows環境ではdockerコマンドの前にwinptyが必要かも

例: winpty docker exec -it db bash