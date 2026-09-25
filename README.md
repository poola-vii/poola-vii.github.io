# poola-vii.github.io

`poola-vii` の共通公式サイト（GitHub Pages）のソースです。公開されるサイトは <https://poola-vii.github.io/> です。

**2026-09-25 時点で、公開している製品はありません。** サイトは「準備中・未公開β」の表示で置いています。

## 構成

| 場所 | 内容 |
|:---|:---|
| `index.md` | トップ。公開者、製品の一覧、入手先、サポート窓口への入口 |
| `privacy.md` | **このサイト**のプライバシー（GitHub Pages が訪問者の IP を記録すること）。当方が持つ文書 |
| `twotile/index.md` | TwoTile の紹介・動作条件・入手方法 |
| `twotile/` のその他 | TwoTile の利用条件、プライバシーポリシー、第三者ライセンス、既知の制限、変更履歴、ログ採取方法、サポート範囲 |

## 文面の正

`twotile/` に置いた文書は、**`poola-vii/TwoTile` リポジトリの `docs/public/` が文面の正**です。ここにあるのは写しです。直すときは正の側を直してから写し直します。ここで直して済ませると、2か所が食い違います。

写すときの決まり:

- 先頭の `# 見出し` を外し、`title:` に移す（front matter は `layout: page` と `title:` だけ）。
- 文書どうしの相対リンク（`known_issues.md` など）はそのまま残す。`jekyll-relative-links` が公開後の URL へ直す。
- ディレクトリをまたぐリンクは、出力先のパス（`/privacy.html` など）で書く。
- 公開前の状態に合わせて、制定日・発効日・入手先・SHA-256 の欄に「準備中」の断り書きを入れる。

`privacy.md` は写しではありません。サイト（GitHub Pages）の話であって、アプリの話ではないためです。

サイトの作り: Jekyll + minima（GitHub Pages の既定）。ビルドは GitHub 側で行うため、ローカルに用意するものはありません。
