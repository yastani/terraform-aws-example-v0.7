# terraform-aws-example-v0.7
Terraform 0.7の頃に作ったらしき遺物

## 推測する構成

踏み台とWebサーバ、それにLambdaがSNSを使ってSlackに通知する何からしい

## 説明書らしきもの

[1]makeコマンドをインストールし、環境変数にセット
[2]S3にtfstateファイルを保存するためのBucketを作成しておく
[3-1]terraformのルートディレクトリまで移動して下記コマンドを実行
[3-2]make terraform-get ENV=development
[4-1]リソースをデプロイする場合、下記コマンドを実行
[4-2]make terraform remote-enable ENV=development ARGS=apply


※環境はあらかじめ定義した上で実行すること
※必要に応じてMakefileの値も変更すること