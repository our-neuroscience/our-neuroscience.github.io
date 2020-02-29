Copyright (c) 2013-2018 Michael Rose and contributors
Released under the MIT license
https://github.com/mmistakes/minimal-mistakes/blob/master/LICENSE

# configured-mmistakes
色々と設定済みの[minimal-mistakes](https://mademistakes.com/work/minimal-mistakes-jekyll-theme/)テーマです。

- 最小限のファイル構成
- 最低限の設定
- Netlify CMSの設定済み
  
## 使い方
1. このリポジトリをクローンする。
   - `$ git clone https://github.com/izmth/configured-mmistakes`
2. 良い感じにカスタマイズする。
   - テスト投稿を削除する。
   - aboutを自分のものに変更する。
   - _config.ymlを編集する。
3. GitHub/GitLab/Bitbucketに上げる。
4. Netlifyの設定を行う。
    - [高機能ホスティングサービスNetlifyについて調べて使ってみた](https://qiita.com/TakahiRoyte/items/b7c4d1581df1a17a93fb#step1re-%E3%83%97%E3%83%AD%E3%82%B8%E3%82%A7%E3%82%AF%E3%83%88%E3%81%AE%E8%BF%BD%E5%8A%A0)
    - `Site settings` > `Identity` の設定を行う。

## ファイル/ディレクトリ概要
### _data/navigation.yml
このファイルを編集してナビゲーションバーのカスタマイズが可能です。

### _pages
`about.md`などのページはこのディレクトリ以下に作成します。ここで作成したページはRecent Postsなどに表示されません。ページには`permalink`の設定をする必要があります。

### _posts
このディレクトリ以下のMarkdownファイルが投稿として扱われます。Markdownファイルは`YYYY-MM-DD-title.md`の形式でなければなりません。

### admin
Netlify CMSの設定に必要なディレクトリです。編集する必要はありません。

### assets/uploads
Netlify CMSから投稿した画像はこのディレクトリに保存されます。このディレクトリ以外に保存したい場合は`admin/config.yml`を編集して下さい。

### _config.yml
このファイルから検索設定やコメント、プロフィール等の設定を行えます。詳しくは公式ドキュメントを参照して下さい。

### admin/config.yml
Netlify CMSの設定ファイルです。編集時にどのオプションを表示するかや、アップロードした画像の保存先を設定することが出来ます。
詳しくは[公式ドキュメント](https://www.netlifycms.org/docs/add-to-your-site/#configuration)を参照して下さい。

## ページの設定項目

| 項目 | 概要 | 設定方法 |
| --- | --- | --- |
| title | タイトル | "About Me"など |
| layout | ページレイアウトの設定 | single, splashなど |
| permalink | 記事のリンク先 | `/about`など
| author_profile | 記事の左側にプロフィールを表示するか | true, false |
| toc | 目次を表示するか | true, false |
| read_time | 記事を読むのに掛かる時間の目安を表示するか | true, false |
| comments | コメント出来るようにするか | true, false |
| share | 共有ボタンを表示するか | true, false |
| related | 関連記事を表示するか | true, false |

`_config.yml`からデフォルトの設定を変更することが出来ます。

