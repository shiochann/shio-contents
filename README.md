# SHIO.CONTENTS

Threads運用のおすすめコンテンツをまとめたLP（1ページ完結）。

note記事「[Threads総フォロワー３万人の私が教えるこれだけあればOK!!コンテンツリスト](https://note.com/shiochan07/n/nc68b72f54fe0)」をサイト型に再構成したもの。

## 構成

- `index.html` — LP本体。CSS/JSはすべて内包した単一ファイル
- `assets/img/` — 教材サムネイル（各販売ページのog:imageを640px幅のJPEGにリサイズしたもの）
- `.nojekyll` — GitHub PagesのJekyll処理を無効化

外部依存はGoogle Fonts（Poppins）のみ。ビルド不要。

## セクション

| # | セクション | 内容 |
|---|---|---|
| 1 | HERO | キャッチ＋実績4指標 |
| 2 | WHY | 売上が出ない2つの理由／買う前に決めること |
| 3 | 3 PILLARS | 集客・教育ファン化・マネタイズ |
| 4 | CONTENTS LIST | 教材カード（BASIC / AFFILIATE / GENRE / NOTE SALES） |
| 5 | SPECIAL BONUS | 経由購入特典 |
| 6 | HOW TO GET | 特典受け取り3ステップ |
| 7 | CTA | 公式LINE誘導 |
| 8 | FAQ | よくある質問 |
| 9 | 広告表記 | ステマ規制対応のPR表記 |

## 編集メモ

- 教材を追加するときは `<!-- ============ LIST ============ -->` 内の `.cat` ブロックをコピーする
- PRリンクには `rel="noopener sponsored"` を付ける。note等の非PRリンクは `sponsored` を外し、タグを `特典対象外` にする
- 数値（部数・実績）は本文にベタ書きなので、更新時は該当箇所を直接編集する
- サムネは販売ページのog:imageを取得 → `sips -s format jpeg -s formatOptions 78 -Z 640` で圧縮して `assets/img/` に置く

## ローカル確認

```bash
python3 -m http.server 8000
```

## 公開

`main` ブランチへのpushでGitHub Pagesに反映される。
