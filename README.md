# diagrams

記事に埋め込む対話的な図の置き場。各図は [archify](https://github.com/anthropics/skills) が出力する 1 ファイル完結の HTML で、外部依存は無く、パン・ズーム・検索・関係のトレース・テーマ切り替えがそのまま動く。

Zenn は `<br>` 以外の HTML を受け付けないので、記事本文には PNG を置き、対話版はここへのリンクで渡す。

StackBlitz 埋め込みは使えない。WebContainers が埋め込み元ページに cross-origin isolation (COOP/COEP) ヘッダを要求し、Zenn はそれを送らないため `Unable to run Embedded Project` になる。

## 構成

```
index.html                    図の一覧
<記事スラッグ>/<図の名前>.html   図の本体
```

## 公開先

GitHub Pages で配信する。

```
https://daichiyasunami-vottia.github.io/diagrams/<記事スラッグ>/<図の名前>.html
```

記事にはこの URL を単独行で貼る（Zenn がリンクカードにする）。

## 収録

| 記事 | 図 |
|---|---|
| バグ報告を出したら、1 分で bot に読まれて 25 分で PR になった | `issue-to-pr/triage-flow.html` |
