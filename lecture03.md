# 第3回課題を通して学んだこと

## APサーバー
- Puma version: 5.6.4
- APサーバー終了させた場合→アクセス不可

## DBサーバー
- 今回使用したのはMySQL バージョン：8.0.29
- サーバー終了させた場合→Can't connect to local MySQL server~と表示されアクセス不可


## Railsの構成管理ツール
- Bundler version 2.3.14

## その他
1. MySQLをRails上でDBサーバーとして使用するためにはgemとしてmysql2が必要

2. sudo service mysqld startでサーバー起動、sudo service mysqld stopでサーバー停止

3. mysql -u ユーザー名 -p　→パスワード入力　でMySQLの中身をいじれるようになる

4. database.ymlにおいてソケットの設定が違うと接続が上手くいかない

5. BundlerはGemfileを参照して必要なgemを（依存関係等を考慮しながらいい感じに）インストールする。
実際にインストールされたgemがGemfile.lockに残るためバージョンはこのファイルを見れば確認可能

6. 実際に起こったエラーについては該当箇所を和訳したり、検索欄にそのまま突っ込むことで解決策までたどり着けることが多いと感じた
