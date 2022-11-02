---
# try also 'default' to start simple
theme: satoryu
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/vbxyFxlgpjM
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
# use UnoCSS
css: unocss
---

# 受託開発受注のための <br /> ちょっとしたコツ
## 〜「何でもかんでもやります」じゃなく、まずはデモ〜

### SATO Tatsuya, Scrum Fest Sapporo 2022, 2022.11.05

<div class="absolute bottom-0 right-0 px-1 text-xs">

Photo by [Jason Goodman](https://unsplash.com/@jasongoodman_youxventures?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [Unsplash](https://unsplash.com/s/photos/meeting?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)

</div>

---
layout: intro
---

# お前、誰よ？

## 自己紹介

---
layout: section
---

# 現地参加の皆さん、
# 羨ましいなー

---
layout: iframe-left
url: https://www.kobe-u.ac.jp/archive/research/20121025_1.html
---

もちろん <br />
エゾアカヤマアリの
スーパーコロニー <br />
ですよね！

---
layout: two-cols
---

<tweet id="901363546545569794" scale="0.6"/>

::right::

ヒアリと違います。 <br />
安心してください。

- 大きさが違います
- 北海道に住めません

---
layout: section
---

# 本題に戻ります

---

# この数年で経験した開発

- 他社の社内サービスの開発
- 関係会社から発案のPoCの開発
- 自社の社内サービスの開発、リプレイス

---
layout: section
---

# 受託開発だ！

---

# ここでの受託開発

- 作りたい人、作る人が離れている開発
- 会社が違う、部署が違うなど様々

<div class="flex justify-center">

<img src="/context.excalidraw.png" class="w-1/2"/>

</div>

---
layout: section
---

# 受託開発に現れる力学

---

# 受託開発に現れる力学

- 発注側
  - 作りたいモノがはっきりしていない
  - どうやっていいのかもわからない
- 受注側
  - 人月請求
  - 契約
- PoC

---

# 作りたいモノがはっきりしていない

- 要件定義ができていない。PBIもない。
- 開始時点では情報が足りていない。
- **開発を積極的に進めることができない**

---

## 失敗理由の筆頭はシステムの「要件定義が不十分」

> 成功率が上がったものの、「半数が失敗」している現状がある。2018年の調査で日経コンピュータは失敗したプロジェクトの失敗理由を調べている。それによると、満足を得られなかった理由の筆頭は「**要件定義が不十分**」、コストを順守できなかった理由の筆頭は「追加の開発作業が発生」、スケジュールを順守できなかった理由の筆頭は「システムの仕様変更が相次いだ」だった。**スケジュールを守れなかったプロジェクトで最も苦労した工程を尋ねると「要件定義」が筆頭に来た。**
>
> -- [プロジェクト失敗の理由、15年前から変わらず (2ページ目)：日経ビジネス電子版](https://business.nikkei.com/atcl/opinion/15/100753/030700005/?P=2)


---

# どうやっていいのかもわからない

- 役割とその仕事を知らない
- **想像で要件定義やPBIを作ってしまう**
- 受注側がサポートもできるが、難しい

---

# 人月請求

- この見積もりだと、受注側が理解しやすい
- 儲けるためには2通り
  - 時間数を増やす
  - 時間単価を上げる
- 内容は問われないので、 <br/> **無駄なことをしても稼げる**

---

# 契約

- 契約時点で何を作るかが決まっていないので、準委任になりがち
- 完成を要求されない
- 人月請求と合わさると、<br /> **期間内での完成を目指さない方が儲けられてしまう**

---

# PoC, Proof Of Concept

- 人によって意味が異なる
  - 新技術を試すことが目的だったり
  - プロダクト開発の初期のことを指したり

---

# 「PoCだから」

- **プロジェクト期間だけでしか利用しない場合**
- PoCは手を抜く理由にされがち
  - パフォーマンスは気にしない
  - ログは残さない
  - テストコードは書かない

---

# 悪い方向への力が多い

- 要件定義や目的が定まらない
- 速く作らなくても稼げてしまう
- 良いものを作らなくても稼げてしまう

---

# 抗うにはどうしたらいいのか？

- 最終的に開発チームに力が流れてくる
- 開発チームで抗うしかない

---
layout: section
---

# 開発チームの**規律**

---

# 規律とは

> き‐りつ【規律／紀律】
>
> 1. 人の行為の基準として定められたもの。おきて。「―を守る」
> 2. 一定の秩序。「―正しい生活」

---
layout: section
---

# では、規律として
# 何をまずやるべきなのか？

---
layout: section
---

# デモを作る

---

# デモ

- 今わかっている情報を集めて、欲しい物を想像して作る
- 誰がどういうときに使って、何を解決するのかを想像

---

# デモアプリのいいこと 3選

- 要件へのフィードバックループが作れる
- 実現可能かを試せる
- 技術プラクティスが使えるようになる

---

# フィードバックループが作れる

- 要件定義だけでは正しいのか検証できない
- 動くものがあれば検証ができる
- フィードバックを繰り返して、要件をよりよくできる

<!--
TODO: V字モデルの図をここに入れる。

その時点でのわかり得る要件定義に対してフィードバックができる
実際に動いているものとして見ることで、意見が生まれやすくなる
-->

---
layout: image
image: https://files.speakerdeck.com/presentations/374d04790e8c4ec6aa227242c370aa4d/slide_5.jpg
---

<div class="px-1 absolute bottom-0 left-0 bg-gray-500 bg-opacity-30 text-xs">

[Agile and Requirement : アジャイルな要件定義について考える - Speaker Deck](https://speakerdeck.com/kawaguti/agile-and-requirement?slide=6)

</div>

---

# 実現可能かを試せる

- 技術的制約がある場合、実現可能なのかのリスクを
- そもそもできなければ、プロジェクトはやらない方が良い
- 制約の不安を消して、見積もりしやすくなる

---

# 技術プラクティスが使えるようになる

- テスト駆動開発やCIを始められる
- 途中から入れるのは難しい

---
layout: section
---

# まとめ

---

# まとめ

- 受託開発に発生する悪い力
- 開発者の規律
- 規律としてのデモ
- デモを使って要件へのフィードバックループを作る

---
layout: section
---

# 受託開発は
# アジャイル開発が難しい？

---

# 受託こそアジャイル開発をすべき

![](/agilemanifest.png)

---
layout: section
---

# どう始める？

---
layout: quote
---

# 包括的なドキュメントよりも <br /> 動くソフトウェアを

---
layout: section
---

# 要件定義書よりも <br /> デモを

---
layout: references
---

# 参考文献

- [岡島幸男, 受託開発の極意 変化はあなたから始まる 現場から学ぶ実践手法, 技術評論社, 2008](https://amzn.to/3ft6LLp)
- [倉貫義人, 「納品」をなくせばうまくいく 」, 日本実業出版社, 2014](https://amzn.to/3sTexkM)
- [浅川直輝, 北川賢一, IT業界に根付く構造問題（日経BP Next ICT選書） 日経コンピュータReport3, 日経BP, 2015](https://amzn.to/3sTl0MA)
- [川口恭伸, Agile and Requirement : アジャイルな要件定義について考える, https://speakerdeck.com/kawaguti/agile-and-requirement, 2022](https://speakerdeck.com/kawaguti/agile-and-requirement)
