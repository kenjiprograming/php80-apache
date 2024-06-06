# PHP8.0-Apacheのdocker環境

## 想定する環境

- PHP8.0

  [php:8.0-apache](https://hub.docker.com/_/php/tags?page=&page_size=&ordering=&name=8.0)

## 構成

- www/htmlが公開ディレクトリ

## 使い方

```bash
■ クローン
$ cd DocRoot/
$ git clone ${this repo}

■ ビルド
$ docker-compose build

■ 起動
$ docker-compose up -d

■ 終了
$ docker-compose down
```

## url

[http://localhost:80/](http://localhost:80/)
