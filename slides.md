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

- モノや目的が不明瞭
- 要件定義などができていない。PBIもない。
- **開発を積極的に進めることができない**

---

# どうやっていいのかもわからない

- 役割とその仕事を知らない
- **想像で要件定義やPBIを作ってしまう**
- 受注側がサポートもできるが、難しい
  - 開発以外の仕事が増えてしまう

---

# 人月請求

- 人月での請求だと、受注側が理解しやすい
- 儲けるためには2通り
  - 時間数を増やす
  - 時間単価を上げる
- たくさん働いたら稼げる
- 内容は問われないので、 <br/> **無駄なことをしても稼げる**

---

# 契約

- 契約時点で何を作るかが決まっていないので、準委任になりがち
- 完成を要求されない
- 人月請求と合わさると、**期間内での完成を目指さない方が儲けられてしまう**

---

# PoC, Proof Of Concept

- 人によって意味が異なる
  - 何か試してみたかったり、新しいことをやることが目的
  - 開発の初期のことを指したり
- プロダクトは、そのプロジェクトだけでしか利用されない

---

# 「PoCだから」

PoCは手を抜く理由にされがち

> パフォーマンスは気にしない

> ログは残さない

> テストコードは書かない

---

# 悪い方向への力が多い

- 要件定義や目的が定まらない
- 速く作らなくても稼げてしまう
- 良いものを作らなくても稼げてしまう

---

# 抗うにはどうしたらいいのか？

- 最終的に開発チームに力が流れてくる
- 開発チームで抗うしかない
- 開発チームの**規律**

---
layout: iframe
url: https://kotobank.jp/word/%E8%A6%8F%E5%BE%8B-480311
---

# 規律

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
- 実装可能かを試せる
- 技術プラクティスが使えるようになる

---

# 要件へのフィードバックループが作れる

- 要件定義だけでは正しいのか検証できない
- 動くものを作った上で検証を進める
- プロダクトを先に作り、要件定義へのフィードバックできる仕組みを作る

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

# 受託開発はアジャイル開発が難しい？

---
layout: image
---

# 受託こそアジャイル開発をすべき

![](/agilemanifest.png)

---

# 受託こそアジャイル開発をすべき

- アジャイルソフトウェア開発宣言に集まった当時の状況がそれと似ているのでは
- そこから生まれたからこそ、アジャイル開発が活用できるはず

---

# どう始める？

---
layout: quote
---

# 包括的なドキュメントよりも <br /> 動くソフトウェアを

---

# そのためにデモを作るところから始めよう

---
layout: references
---

# 参考文献

- [岡島幸男, 受託開発の極意 変化はあなたから始まる 現場から学ぶ実践手法, 技術評論社, 2008](https://amzn.to/3ft6LLp)
- [倉貫義人, 「納品」をなくせばうまくいく 」, 日本実業出版社, 2014](https://amzn.to/3sTexkM)
- [浅川直輝, 北川賢一, IT業界に根付く構造問題（日経BP Next ICT選書） 日経コンピュータReport3, 日経BP, 2015](https://amzn.to/3sTl0MA)
- [川口恭伸, Agile and Requirement : アジャイルな要件定義について考える, https://speakerdeck.com/kawaguti/agile-and-requirement, 2022](https://speakerdeck.com/kawaguti/agile-and-requirement)
