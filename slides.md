---
theme: seriph
background: https://source.unsplash.com/collection/94734566/1920x1080
class: text-center
highlighter: shiki
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

<p claas="pt-12">
プロパー勉強会Vol2 by Ond
</p>

---
transition: fade-out
---

<h1 class="font-bold">
    目次
</h1>

<div class="pt-6"></div>

<p class="font-bold">
1. JavaScriptの歴史　
</p>

<div class="pt-6"></div>

<p class="font-bold">
2. 代表的なライブラリとフレームワーク
</p>

<div class="pt-6"></div>

<p class="font-bold">
3. モダンJavaScriptとは
</p>

<div class="pt-6"></div>

<p class="font-bold">
4. ES2015以降の主要な記法の紹介
</p>

---
transition: fade-out
---

<h1 class="font-bold">
今日のテーマ
</h1>

<h2 class="py-12 font-bold text-red">やっぱり「進研ゼミ」</h2>

<h3>
    ちょっとでも記憶に残ってくれたら嬉しいです。
</h3>

---
transition: fade-out
layout: center
---

<h1 class="font-bold">JavaScriptの歴史</h1>

---
transition: fade-out
---

<h1 class="font-bold">JavaScript</h1>

<h2 class="py-12 font-bold text-red">基本的にはブラウザ上で動作するプログラミング言語</h2>

HTML・CSSに追加して使用することで<br>
Webページを動的にすることができる

<p class="pt-12">例) モーダル表示・拡大表示etc...</p>
---
transition: fade-out
---

<h1 class="font-bold">JavaScriptの誕生</h1>

<h2 class="py-12 font-bold text-red">1995年にブレンダン・アイクさんが作った。</h2>

<div class="flex justify-center">
<div class="mr-16">
<div>
<p>
    NetScape Navigater(後のFireFox)というブラウザのために
    開発された。<br>
</p>
</div>
元々<span class="font-bold text-red">LiveScript</span>という名前だったが<br>
1995年12月に<span class="font-bold text-red">JavaScript</span>として実装された。


<div class="pt-6">
当時<span class="font-bold text-red">Java</span>が勢い付いており、<br>
開発会社と提携していたので、名前を変えたらしい
</div>
</div>

<img border="rounded" width="400" height="400" src="https://github.com/slidevjs/themes/blob/main/screenshots/theme-default/01.png?raw=true" alt="">

</div>

---
transition: fade-out
---

<h1 class="font-bold">JavaScriptの不遇の時代</h1>

<h2 class="py-12 font-bold text-red">誕生当初は不遇の時代が続いた</h2>

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

<h1 class="font-bold">ECMAScript</h1>

<h3 class="py-12 font-bold text-red">JavaScriptの標準化を担当するECMAによって定義された標準仕様</h3>

- ブラウザ間の互換性
<p>標準化されることで一定の互換性をブラウザ間で持てるようになった</p>

<div class="pt-6"></div>

- 現在
<p>定期的にバージョンアップがされて、現在は毎年6月にリリースされる。<br>
ver5.1までは<span class="font-bold text-red">ES5</span>のような表示だったが、ver6以降は西暦を含める<span class="font-bold text-red">ES2024</span>のような表記に変更された</p>

---
transition: fade-out
---

<h1 class="font-bold">JavaScriptの転換期</h1>

<h2 class="font-bold text-red pt-12">GoogleMaps</h2>

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

<h1 class="font-bold">Ajax</h1>

<h3 class="font-bold text-red pt-12">非同期でJavaScriptを使ってサーバーと通信する仕組み</h3>

A  → Asynchronous(非同期の)<br>
Ja → JavaScript<br>
x  → XMLHttpRequest(JavaScript組み込みのHTTP通信できるAPI)<br>

<div class="pt-12"></div>

- 非同期<br>
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

<h1 class="font-bold">JavaScriptの代表的なライブラリ
</h1>

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

<h1 class="font-bold">
JavaScriptの代表的なフレームワーク
</h1>
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

<h1 class="font-bold">モダンJavaScriptの特徴</h1>

<h3 class="font-bold text-red pt-12">明確なルールはないが、一般的には以下の特徴</h3>

<div class="pt-12"></div>

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
transition: fade-out
---

<h1 class="font-bold">仮想DOM</h1>

<h3 class="font-bold text-red pt-6">DOM</h3>
<p>
    DOMとはHTMLのソースコード自体のことではなく、画面を表示する際に解釈した<br>
    HTML/CSS/JavaScriptによって構築されたツリー型のオブジェクト<br>
    JavaScript等で値を操作できる。
</p>

<h3 class="font-bold text-red pt-6">仮想DOM</h3>
<p>
    プログラム的に作成された仮のDOM
</p>

<h3 class="font-bold text-red pt-6">通常と仮想DOMの違い</h3>
<p>
    通常は変更が入るとDOMを再構築し再描画していたが、<br>
    仮想DOMは変更を受け取ってもすぐには描画を行わず、<br>
    変更を反映した仮想DOMと通常のDOMを比べて、<br>
    変更差分だけを検出し、描画する。<br>
</p>

---
transition: fade-out
---

<h1 class="font-bold">パッケージマネージャー</h1>

<h3 class="font-bold text-red pt-6">パッケージとは</h3>
<p>
   moduleをまとめて機能するようにしたもの<br>
</p>

<h3 class="font-bold text-red pt-6">npmとは</h3>
<p>
    Node.jsのパッケージ管理システム<br>
    Facebookが作った互換性がある<span class="text-red">Yarn</span>もある
</p>


<h3 class="font-bold text-red pt-6">npmの必要性</h3>

<div class="pt-4"></div>

- パッケージの依存関係の解決
- パッケージの競合関係

---
transition: fade-out
---

<h1 class="font-bold">モジュールバンドラー</h1>

<h3 class="font-bold text-red pt-6">webpack</h3>
<p>
   複数のモジュールの依存関係を解決して、一つにまとめてくれる<br>
   後継で<span class="text-red">Vite</span>がある。
</p>

<h3 class="font-bold text-red pt-6">なぜするのか？</h3>
<p>
    モジュールの数が増えると、リクエストの数が増えるので、<br>
    パフォーマンスが落ちる。<br>
    <br>
    開発時は、機能を分けて保守性高く<br>
    実行するときは、機能をまとめてパフォーマンスを高くできる<br>
</p>

---
transition: fade-out
---

<h1 class="font-bold">トランスパイラ</h1>

<h3 class="font-bold text-red pt-6">Babel</h3>
<p>
    ソースコードを別のソースコードに変更するためのプログラム<br>
    ブラウザで動作させるために古い仕様の範囲内で解釈できる形に変換してくれる。<br>
</p>

<h3 class="font-bold text-red pt-6">なぜするのか？</h3>
<p>
    新しい仕様のJavaScriptやTypeScriptなどで開発できる！<br>
    <br>
    トランスパイル → モジュールバンドルの流れ
</p>

---
transition: fade-out
layout: center
---

<h1 class="font-bold">
    ES2015の主要記法の紹介
</h1>

---
transition: fade-out
---

<h1 class="font-bold">変数宣言</h1>

<div class="flex">
<div class="w-1/2 p-2">

<h3 class="font-bold text-red py-6">var(旧)</h3>

```javascript

// 再宣言と再代入可能
var hoge = 'syu';
var hoge = 'onoda';

```
</div>

<div class="w-1/2 p-2">
<h3 class="font-bold text-red py-6">letとconst(新)</h3>

```javascript

// let 再代入のみ可能
let hoge = 'syu';
hoge = 'onoda';

// const 再宣言と再代入不可
const hoge = 'syu';

```
</div>
</div>

---
transition: fade-out
---

<h1 class="font-bold">アロー関数</h1>

<div class="flex">
<div class="w-1/2 p-2">

<h3 class="font-bold text-red py-6">無名関数</h3>

```javascript

// 宣言した時点では名前がないので無名関数と呼ばれる。
// 名前のない関数を定義して変数onodaBMIに代入

const onodaBMI = function(weight,height){
 return weight + height * 2;
};

```
</div>

<div class="w-1/2 p-2">
<h3 class="font-bold text-red py-6">アロー関数</h3>

```javascript

// アロー関数とは無名関数をシンプルに書けるやつ
const onodaBMI = (weight, height) => {
  return weight + height * 2;
};

// 省略記法とルール

// 1. 1文で終わる時は{}を省略可能
const onodaBMI = (weight, height) => weight + height * 2;

// 2. 引数が一個の時は()を省略可能
const onodaBMI = weight => weight * 172 * 2;

// 3. 引数がないときは()を省略せずに書く
const onodaBMI = () => weight * 172 * 2;

```
</div>
</div>


