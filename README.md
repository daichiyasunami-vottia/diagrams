# diagrams

記事に埋め込む対話的な図の置き場。各図は [archify](https://github.com/anthropics/skills) が出力する 1 ファイル完結の HTML で、外部依存は無く、パン・ズーム・検索・関係のトレース・テーマ切り替えがそのまま動く。

Zenn は `<br>` 以外の HTML を受け付けないため、記事へは StackBlitz 経由の埋め込みか、PNG に書き出して `/images/` に置く形で載せる。

## 構成

```
index.html                    図の一覧
<記事スラッグ>/<図の名前>.html   図の本体
```

## 記事への埋め込み

```
@[stackblitz](https://stackblitz.com/github/daichiyasunami-vottia/diagrams?embed=1&view=preview&initialPath=/<記事スラッグ>/<図の名前>.html&hideExplorer=1&hideNavigation=1)
```

`initialPath` で表示する図を選ぶ。

## 収録

| 記事 | 図 |
|---|---|
| バグ報告を出したら、1 分で bot に読まれて 25 分で PR になった | `issue-to-pr/triage-flow.html` |
