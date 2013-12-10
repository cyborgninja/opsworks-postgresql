#Opsworks on rails+postgres

AWS提供のopsworks上で、rails + postgresの環境を作る方法です。


## 手順

以下が手順です。

###1. Stackの設定

1. Use custom Chef cookbooks をアクティブにする
2. Repository URLにこのgitのURL( https://github.com/cyborgninja/opsworks-postgresql.git )をコピペする

###2. Layerの設定
1. Custom Chef Recipes に先ほど設定したURLが表示されているか確認する
2. Setupに**postgresql::ruby**と書いて＋を押す

###3. Instancesの設定
普通にInstancesを作成してください。
エラー出たら、ログチェックして対応しましょう。


以上です。


##エラーログのチェックポイント
gemのbundle installのログを確認しましょう。
Installing pg ...
のところがきちんと突破できていればこのリポジトリで出来るエリアは完了です。 



