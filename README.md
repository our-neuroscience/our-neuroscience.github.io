Copyright (c) 2013-2018 Michael Rose and contributors
Released under the MIT license
https://github.com/mmistakes/minimal-mistakes/blob/master/LICENSE

## ファイル/ディレクトリ概要

### _data/navigation.yml
このファイルを編集してナビゲーションバーのカスタマイズが可能です。

### _pages
`about.md`などのページはこのディレクトリ以下に作成します。ここで作成したページはRecent Postsなどに表示されません。ページには`permalink`の設定をする必要があります。

### _posts
このディレクトリ以下のMarkdownファイルが投稿として扱われます。Markdownファイルは`YYYY-MM-DD-title.md`の形式でなければなりません。

### _config.yml
このファイルから検索設定やコメント、プロフィール等の設定を行えます。詳しくは公式ドキュメントを参照して下さい。

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

