# qiita-rticles
Qiita記事の原稿を置いているリポジトリ。

# how to
```
Microsoft Windows [Version 10.0.26200.7462]
(c) Microsoft Corporation. All rights reserved.

C:\Users\xxxxx\Desktop\git\syachiku-kun\repositories>git clone https://github.com/syachiku-kun/qiita-rticles.git
Cloning into 'qiita-rticles'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (3/3), done.

C:\Users\xxxxx\Desktop\git\syachiku-kun\repositories>cd qiita-rticles

C:\Users\xxxxx\Desktop\git\syachiku-kun\repositories\qiita-rticles>(echo(&echo [user]&echo     name = syachiku-kun  # ユーザ名&echo     email = xxxxxxxxxx@gmail.com  # メールアドレス) >> ".\.git\config"

C:\Users\xxxxx\Desktop\git\syachiku-kun\repositories\qiita-rticles>npm -v
11.6.2

C:\Users\xxxxx\Desktop\git\syachiku-kun\repositories\qiita-rticles>npm install @qiita/qiita-cli --save-dev

added 110 packages in 3s

47 packages are looking for funding
  run `npm fund` for details

C:\Users\xxxxx\Desktop\git\syachiku-kun\repositories\qiita-rticles>npx qiita version
[dotenv@17.2.3] injecting env (0) from .env -- tip: ⚙️  suppress all logs with { quiet: true }
1.7.0

C:\Users\xxxxx\Desktop\git\syachiku-kun\repositories\qiita-rticles>npx qiita init
[dotenv@17.2.3] injecting env (0) from .env -- tip: ⚙️  load multiple .env files with { path: ['.env.local', '.env'] }
設定ファイルを生成します。

  Creating C:\Users\xxxxx\Desktop\git\syachiku-kun\repositories\qiita-rticles\.github\workflows\publish.yml
     Created!

  Creating C:\Users\xxxxx\Desktop\git\syachiku-kun\repositories\qiita-rticles\.gitignore
     Already exists.

  Creating C:\Users\xxxxx\Desktop\git\syachiku-kun\repositories\qiita-rticles\qiita.config.json
     Created!

Success! ✨

次のステップ:

  1. トークンを作成してログインをしてください。
    npx qiita login

  2. 記事のプレビューができるようになります。
    npx qiita preview


C:\Users\xxxxx\Desktop\git\syachiku-kun\repositories\qiita-rticles>npx qiita login
[dotenv@17.2.3] injecting env (0) from .env -- tip: 🔄 add secrets lifecycle management: https://dotenvx.com/ops

以下のURLにアクセスしてトークンを発行してください。（「read_qiita」と「write_qiita」にチェックを入れてください）
  https://qiita.com/settings/tokens/new?read_qiita=1&write_qiita=1&description=qiita-cli

発行したトークンを入力: xxxxxxxxxx
Hi cipher-31186!

ログインが完了しました 🎉
以下のコマンドを使って執筆を始めましょう！

🚀 コンテンツをブラウザでプレビューする
  npx qiita preview

🚀 新しい記事を追加する
  npx qiita new (記事のファイルのベース名)

🚀 記事を投稿、更新する
  npx qiita publish (記事のファイルのベース名)

💁 コマンドのヘルプを確認する
  npx qiita help

C:\Users\xxxxx\Desktop\git\syachiku-kun\repositories\qiita-rticles>npx qiita help
[dotenv@17.2.3] injecting env (0) from .env -- tip: ✅ audit secrets and track compliance: https://dotenvx.com/ops
USAGE:
qiita <COMMAND> [<OPTIONS>]

COMMAND:
  init                    記事をGitHubで管理するための初期設定
  login                   Qiita APIの認証認可
  new [<basename>] ...    新しい記事を追加
  preview                 コンテンツをブラウザでプレビュー
  publish <basename> ...  記事を投稿、更新
  publish --all           全ての記事を投稿、更新
  pull                    記事ファイルをQiitaと同期
  version                 Qiita CLIのバージョンを表示
  help                    ヘルプを表示

OPTIONS:
  --credential <credential_dir>
    Qiita CLIの認証情報を配置するディレクトリを指定

  --root <root_dir>
    記事ファイルをダウンロードするディレクトリを指定

  --verbose
    詳細表示オプションを有効

  --config
    設定ファイルを配置するディレクトリを指定

詳細についてはReadme(https://github.com/increments/qiita-cli)をご覧ください


C:\Users\xxxxx\Desktop\git\syachiku-kun\repositories\qiita-rticles>npx qiita pull --force
[dotenv@17.2.3] injecting env (0) from .env -- tip: 🛠️  run anywhere with `dotenvx run -- yourcommand`
Sync local articles from Qiita
Successful!

C:\Users\xxxxx\Desktop\git\syachiku-kun\repositories\qiita-rticles>
```