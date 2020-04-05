# README

# Techonology
* Docker
* docker-compose(ローカル環境構築)
* CircleCI(rspec/rubocopがプッシュされた時に自動で動く)(cacheを使用し高速でCIを実行)

# Requirement
* Docker
* docker-compose

# Installation
* imageを構築(コンテナは作成しない)
```bash
$ docker-compose build
```
* データベース生成
```bash
$ docker-compose run --rm web rails db:create
```
* マイグレーション
 ```bash
$ docker-compose run --rm web rails db:migrate
```

* 起動
 ```bash
$ docker-compose up
```
