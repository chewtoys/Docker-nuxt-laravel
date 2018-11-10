### Docker環境の準備

DockerとDocker Composeを使います。

WindowsOSは非対応となっています。
macOS/Linuxのの入ったPCを用意して下さい。

#### Run setup script

下記を叩くだけでDocker Image、DB構築をすべてやってくれます。
初回`git clone`しか実行はしません。

```
$ git clone https://github.com/nyanko-kota/Docker-laravel-nuxt
```

```
$ ./setup.sh
```

#### アプリの起動

```
$ docker-compose up
```

このコマンドを入力後、
http://localhost:3000  にアクセスするとNuxt.jsのトップページが表示されます。
http://localhost:10050 にアクセスするとLarevelのトップページが表示されます。


#### 注意事項
これは開発環境です。
本番環境には流用できるものではありません。
使用される際は、Laravelフォルダ内にLaravel関連ファイルを、Nuxtフォルダ内にNuxt関連ファイルを、配置しご使用ください。
