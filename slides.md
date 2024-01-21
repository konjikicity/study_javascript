---
theme: seriph
background: https://source.unsplash.com/collection/94734566/1920x1080
class: text-center
highlighter: shikiji
lineNumbers: false
transition: slide-left
mdc: true
fonts:
  # basically the text
  sans: 'Noto Sans JP'
  # use with `font-serif` css class from windicss
  serif: 'Robot Slab'
  # for code blocks, inline code, etc.
  mono: 'Fira Code'
---

<h1 class="font-bold">Javascriptの歴史</h1>

プロパー勉強会Vol2 by Ond

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Slidevを使って作っています。 <carbon:arrow-right class="inline"/>
  </span>
</div>

---
transition: fade-out
---

# 目次

<div class="pt-6"></div>

1. JavaScriptって何？

<div class="pt-6"></div>

2. 代表的なライブラリとフレームワーク

<div class="pt-6"></div>

3. モダンJavaScriptとは

<div class="pt-6"></div>

4. まとめ

---
transition: fade-out
---

# 今日のテーマ

<h2 class="py-12 font-bold text-red">やっぱり「進研ゼミ」</h2>

### ちょっとでも記憶に残ってくれたら嬉しいです。
### 後半紹介する記法等


---
transition: fade-out
layout: center
---

<h1 class="font-bold">JavaScriptって何？</h1>

---
transition: fade-out
---

# JavaScript

<h2 class="py-12 underline">基本的にはブラウザ上で動作するプログラミング言語</h2>

HTML・CSSに追加して使用することで<br>
Webページを動的にすることができる

<p class="pt-12">例) モーダル表示・拡大表示etc...</p>
---
transition: fade-out
---

# JavaScriptの誕生

<h2 class="py-12 underline">1995年にブレンダン・アイクさんが作った。</h2>

<div class="flex justify-center">
<div class="mr-16">
元々<span class="font-bold text-red">LiveScript</span>という名前だったが<br>
1995年12月に<span class="font-bold text-red">JavaScript</span>として実装された。

<div class="pt-12">
当時<span class="font-bold text-red">Java</span>が勢い付いており、<br>
開発会社と提携していたので、名前を変えたらしい
</div>
</div>

<img border="rounded" width="400" height="400" src="https://github.com/slidevjs/themes/blob/main/screenshots/theme-default/01.png?raw=true" alt="">

</div>

---
transition: fade-out
---

# JavaScript不遇の時代

<h2 class="py-12 underline">誕生当初は不遇の時代が続いた</h2>

- ブラウザ間の互換性

マイクロソフト社がIEをリリースしたけど、ライセンスを許可しなかったので、<br>
<span class="font-bold text-red">JScript</span>という別の言語を作ってしまった。<br>
<span class="font-bold text-red">JavaScript</span>と互換性がない部分が多くdeveloperからは不評の嵐

- あまりに手軽すぎた

ブラウザさえあればすぐ構築できるので、初心者が多く利用するようになったり、<br>
悪用も多発し、Webサイトに負荷をかけたり脆弱性をついたウイルスなど<br>
セキュリティ面でも問題があった

これによりブラウザの<span class="font-bold text-red">JavaScript</span>
自体の機能を切る人が続出した。(<span class="font-bold text-red">Flash</span>が流行ったのもある)

<div class="pt-12">
当時<span class="font-bold text-red">Java</span>が勢い付いており、<br>
開発会社と提携していたので、名前を変えたらしい
</div>

---
transition: fade-out
---

# ECMAScriptとは？

<h3 class="py-12 underline">JavaScriptの標準化を担当するECMAによって定義された標準仕様</h3>

- ブラウザ間の互換性
<p>標準化されることで一定の互換性をブラウザ間で持てるようになった</p>

<div class="pt-12"></div>

- 現在
<p>定期的にバージョンアップがされて、現在は毎年6月にリリースされる。<br>
ver5.1までは<span class="font-bold text-red">ES5</span>のような表示だったが、ver6以降は西暦を含める<span class="font-bold text-red">ES2024</span>のような表記に変更された</p>

---
transition: fade-out
---

# どうやって人気になったのか？

<h2 class="py-12 underline">GoogleMaps</h2>

<div class="pt-12">
    2005年にGoogle社が<span class="font-bold text-red">GoogleMaps</span>を発表した<br>
    <span class="font-bold text-red">Ajax</span>という技術が利用されており、JavaScriptが使用されていたことから<br>
    再び注目されるようになった。
</div>

<div class="pt-12">
後にでたGmailとGoogleCalenderにも<br>
JavaScriptが使用されたことで一気に人気に....
</div>

---
transition: fade-out
---

# Ajaxって何？

<h2 class="py-12 underline">非同期でJavaScriptを使ってサーバーと通信する仕組み</h2>

A  → Asynchronous(非同期の)<br>
Ja → JavaScript<br>
x  → XMLHttpRequest(JavaScript組み込みのHTTP通信できるAPI)<br>

<div class="pt-12"></div>

- 非同期とは？<br>
→ <span class="font-bold text-red">タスクの完了を待つことなく並列に処理を実行できる仕組み</span>

例) メール処理、検索の候補表示、地図

---
transition: fade-out
layout: center
---

<h1 class="font-bold">代表的なライブラリとフレームワーク</h1>


---
transition: fade-out
---

# JavaScriptの代表的なライブラリ

<h3 class="font-bold text-red pt-12">JQuery</h3>
<p>JavaScriptの記述を簡単に書けるライブラリ</p>

<h3 class="font-bold text-red pt-6">Node.js</h3>
<p>サーバーサイドでJavaScriptを実行できるようになる実行環境<br>
最近はクライアントサイドの開発環境でも利用されるのが一般的<br>
有名なパッケージマネージャーとして<span class="font-bold text-red">npm</span>と<span class="font-bold text-red">yarn</span>がある</p>

<h3 class="font-bold text-red pt-6">TypeScript</h3>
<p>JavaScriptに型定義できるようにした静的型付言語</p>

---
transition: fade-out
---

# JavaScriptの代表的なフレームワーク

<h3 class="font-bold text-red pt-12">Vue</h3>
<p>HTMLの記述に近い形で記述が可能</p>

<h3 class="font-bold text-red pt-6">React(ReactNative)</h3>
<p>Viewを宣言的にコードを書けるのが特徴(JSX記法)<br>
過程を書くのが手続き的、最終的な表示をかくのが宣言的</p>

<h3 class="font-bold text-red pt-6">Next.js</h3>
<p>Reactのフレームワークとして登場<br>
現在はこちらの利用がかなり主流<br>
SSR/SSG、画像最適化など様々な機能を持つフルスタックフレームワーク<br>
<span class="font-bold text-blue">https://syu-blog.jp</span>もNext.jsを使用</p>

---
transition: fade-out
layout: center
---

<h1 class="font-bold">モダンJavaScriptとは</h1>

---
transition: fade-out
---

# モダンJavaScriptの特徴

<h3 class="font-bold underline py-12">明確なルールはないが、一般的には以下の特徴</h3>

<div class="pt-6"></div>

- React、Vueなどの仮想DOMを使用するライブラリやフレームワークを使用

<div class="pt-6"></div>

- npmやyarnなどのパッケージマネージャーを使用

<div class="pt-6"></div>

- webpackなどのモジュールバンドラーを使用

<div class="pt-6"></div>

- Babelなどのトランスパイラを使用

<div class="pt-6"></div>

- 主にES2015以降の記法を使用(かなり多くの便利な変更が入った)

---

