# Baukis2 - 顧客管理システム

## 説明
Baukis2は企業向けの顧客管理システム(Ruby on Rails学習用サンプル)です。

## 推奨されるシステム環境
- Ubuntu 18.04
- Ruby 2.6.4
- PostgreSQL 11.2

## 注意事項
- 以下の手順では、一般ユーザーの権限でコマンドを実行してください

## インストール手順
- この`READEME.md`が存在するディレクトリで`bin/bundle`コマンドを実行してください。

## データベースのセットアップ
- このシステム専用のデータベースを PostgreSQL 上に作成してください。
- データベースへの接続パラメータに基づいて `config/database.yml` を作成してください。
- `bin/rails db:setup` コマンドを実行してください。

## hostsファイルの設定
- ホストOSの `hosts` ファイルに次の1行を追加してください（要root権限）。`hosts`ファイルは、Mac OS Xの場合は、
`/private/etc/hosts` フォルダに、Windonsの場合は `C:\Windows\system32\drivers` フォルダにあります。

`127.0.0.1 example.com baukis2.example.com`

## システムの起動と終了
- `bin/rails s`コマンドを実行するとシステムが起動します。
- Ctrl-Cを入力するとシステムが終了します。

## システムの利用
- ブラウザで以下の URL にアクセスしてください:
  - http://baukis2.example.com:3000 -- 職員向けサイト
  - http://baukis2.example.com:3000/admin -- 管理者向けサイト
  - http://example.com:3000/mypage -- 顧客向けサイト
