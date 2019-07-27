参考： https://docs.docker.com/compose/rails/

## 使い方

+ git clone https://github.com/oshimamasara/docker-rails-windows.git
+ cd docker-rails-windows
+ open file
+ 改行コードを LF に変更し、保存
+ docker volume create mydb
+ docker-compose run web rails new . --force --no-deps --database=postgresql
+ docker-compose build
+ database.yml の変更（公式ドキュメント参考）
+ docker-compose up
+ docker-compose run web rake db:create
+ docker-compose up -d

## YouTube

https://youtu.be/xI6Vf9CfHg4
