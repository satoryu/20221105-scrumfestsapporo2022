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

# 自己紹介

---

# 受託開発

- プロダクトを作りたい人、作る人が離れている体制での開発
- 会社が違う、部署が違うなど様々

<div class="flex justify-center">

<img src="/context.excalidraw.png" class="w-1/2"/>

</div>

---

# 経験してきた受託開発

- 他社の社内サービスの開発
- 関係会社から発案のPoCの開発
- 自社の社内サービスの開発、リプレイス

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
  - 人月商売
  - 契約

---

# 作りたいモノがはっきりしていない

- モノや目的が不明瞭
- 要件定義などができていない。PBIもない。
- そのため、**開発を積極的に進めることができない**

---

# どうやっていいのかもわからない

- 役割とその仕事を知らない
- なんとなくの**想像で要件定義やPBIを作ってしまう**
- 受注側がサポートもできるが、難しい
  - 開発以外の仕事が増えてしまう

---

# 人月請求

- 人月での請求だと、受注側が理解しやすい
- 儲けるためには2通り
  - 時間数を増やす
  - 時間単価を上げる
- たくさん働いたら稼げる
- 内容は問われないので、 <br/> 無駄なことをする方が稼げてしまう

---
# 契約

- 契約時点で何を作るかが決まっていないので、準委任になりがち
- 完成を要求されない
- 人月請求と合わさると、期間内での完成を目指さない方が儲けられてしまう

---
# 悪い方向への力が働く

- 曖昧な要件定義で目的が定まらない
- 開発自体も良いものをすぐに作ろうということをしなくても稼げてしまう

---

# 抗うにはどうしたらいいのか？

- 最終的に開発チームに力が流れてくる

---

# そこで、デモ！

---

# デモアプリケーション

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

