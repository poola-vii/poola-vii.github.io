# poola-vii.github.io

`poola-vii` の共通公式サイト（GitHub Pages）のソースです。公開されるサイトは <https://poola-vii.github.io/> です。

## 構成

| 場所 | 内容 |
|:---|:---|
| `index.md` | トップ。公開者、製品の一覧、入手先、サポート窓口への入口 |
| `privacy.md` | **このサイト**のプライバシー（GitHub Pages が訪問者の IP を記録すること）。当方が持つ文書 |
| `twotile/index.md` | TwoTile の紹介・動作条件・入手方法 |
| `twotile/` のその他 | TwoTile の利用条件、プライバシーポリシー、第三者ライセンス、既知の制限、変更履歴、ログ採取方法、サポート範囲 |
| `nintimer/index.md` | Nintimer の紹介・動作条件・入手方法 |
| `nintimer/` のその他 | Nintimer の利用条件、プライバシーポリシー、第三者ライセンス、既知の問題、変更履歴、サポート範囲 |
| `twotile/screenshot.png`・`screenshot.en.png`、`nintimer/` の同名の2つ | 紹介ページ（日英）の冒頭に載せる画像。Store に出しているスクリーンショットの1枚目 |
| `assets/main.scss` | minima の見た目に足す設定。幅 800px 未満の画面（スマホ、タブレットの縦置き）で、本文の途中で切れない長い文字列（SHA-256 の値、URL など）を折り返し、ページが横にスクロールしないようにしている。800px 以上では折り返さない |

## 文面の正

`twotile/` に置いた文書は、**`poola-vii/TwoTile` リポジトリの `docs/public/` が文面の正**です。`nintimer/` に置いた文書は、**`poola-vii/Nintimer` リポジトリの `docs/public/` が文面の正**です（`index.md` は `release_readme.md` の写し）。ここにあるのは写しです。直すときは正の側を直してから写し直します。ここで直して済ませると、2か所が食い違います。

写すときの決まり:

- 先頭の `# 見出し` を外し、`title:` に移す（front matter は `layout: page` と `title:`。英語のページには `lang: en` も入れる）。
- 文書どうしの相対リンク（`known_issues.md` など）はそのまま残す。`jekyll-relative-links` が公開後の URL へ直す。
- ディレクトリをまたぐリンクは、出力先のパス（`/privacy.html` など）で書く。
- 公開前の製品では、制定日・発効日・入手先・SHA-256 の欄に「準備中」の断り書きを入れる。

**紹介ページ（`index.md`・`index.en.md`）の冒頭の画像は、写しにだけ足しています**（正の側には無い。写し直すときに消さない）。画像は Store に出しているスクリーンショットの1枚目で、Store の画像を差し替えるときに、ここも同じ画像に替えます。

`privacy.md` は写しではありません。サイト（GitHub Pages）の話であって、アプリの話ではないためです。

サイトの作り: Jekyll + minima（GitHub Pages の既定）。ビルドは GitHub 側で行うため、ローカルに用意するものはありません。
