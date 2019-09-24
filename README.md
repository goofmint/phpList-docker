# phplist-docker

phpListをDockerで動かします。

postflixの設定を[Customers Mail Cloud](https://smtps.jp/)に寄せています。

## 必要なもの

- Docker
- Docker Compose

## 設定

設定ファイルを作成します。.env-distをコピーして編集してください。

    cp .env-dist .env
   

## 立ち上げ

ビルドした後、立ち上げます。

```
docker-compose build
```

```
docker-compose up
```

立ち上がったら、下記のアドレスにアクセスします。

http://localhost:8000/lists/admin/

ログイン情報は下記の通りです。設定で変更できます。

- **ユーザ名**  
admin
- **パスワード**  
SomeRandomPassword
