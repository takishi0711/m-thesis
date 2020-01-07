# M Thesis Template

## Overivew

LaTeX template files of M thesis


## Requirements

- LaTeX


## Compilation

```
$ platex mthesis
$ pbibtex mthesis
$ platex mthesis
$ platex mthesis
$ dvipdfmx mthesis
```


## How to see diff in github.com

`[github.comのリモートリポジトリのURL]/compare/[比較元のcommit, tag, branch]...[比較先のcommit, tag, branch]` にアクセスすることで，github.com上で比較できます．
第n稿を書き上げたタイミングでcommitにtagを打っておくと比較しやすいでしょう．

## Filename

ファイル名にprefixをつけることで，github.com上でのdiff表示の順序制御をしています．
基本的に `xx-hogehoge.tex` と順番をつけていますが，章構成の変更などで間に章を追加したくなることがあると思います．
例えば，関連研究（ `02-related_work.tex` ）と設計（ `03-design.tex` ）の間にアプローチの章を入れる場合は， `02_1-approach.tex` のように， `_` で間に値を挟むと順序が保存されるので，そうしてください．
`04-design.tex` のようにリネームしてしまうと，リネーム前後でdiffを取れなくなるので，リネームするのはオススメしません．
