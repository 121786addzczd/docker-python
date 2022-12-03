# docker-python
docker上でpythonの実行環境を作成し、学習するためのリポジトリです

## 環境構築
```
#コンテナ起動・作成
docker-compose up -d --build
```

コンテナの作成・起動が完了したら以下のリンクにアクセスします。

http://localhost:8888/lab

jupyter labの画面が表示されたら環境構築は完了です。


## Dockerの全削除の方法
Dockerのイメージやコンテナを削除します。
他のイメージやコンテナも削除されるのでそれをしっかり理解した上で実行してください。
```
docker image prune -af
docker volume prune -f
docker container prune -f
docker system prune -f
```