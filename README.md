## 事前準備

### Docker環境の準備

DockerとDocker Composeを用います。
そのためDockerとDocker Composeに関してはインストールが必要です。
WindowsOSは非対応となっています。
そのためmacOS/Linuxのの入ったPCを用意して下さい。

#### 必要なファイル

./laravel下にLaravelのプロジェクトファイル
./nuxt下にnuxtのプロジェクトファイルを配置してください

#### Run setup script

下記を叩くだけでDocker Image、DB構築をすべて完了します。
順番に実行してください。

```
$ git clone https://github.com/nyanko-kota/CodeGO
```

```
$ ./setup.sh
```

#### アプリの起動

```
$ docker-compose up
```

このコマンドを入力後、

http://localhost:3000  にアクセスすると、トップページが表示されます。

http://localhost:8081  にアクセスすると、pgwebが表示されます。

http://localhost:8000  にアクセスすると、apiサーバー(Laravel)が表示されます。
