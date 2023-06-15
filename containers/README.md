# Pandas 100本ノック

・以下のコマンドを実行しコンテナを立ち上げる
```shell
docker image build -t pandas100 .
docker run --rm -v {{ cloneしたリポジトリまでのパス }}/Pandas_100_knocks:/work -p 8887:8888 --name pandas100c -it pandas100:latest
```
・http://localhost:8887 にアクセスする
