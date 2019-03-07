# highlight.js

* 公式ページ

https://highlightjs.org/

* jsソースへのアクセス

`https://cdnjs.cloudflare.com/ajax/libs/highlight.js/<Version>/highlight.min.js`

* スタイルとかはここで探す

https://highlightjs.org/static/demo/

* スタイルソースへのアクセス

`https://cdnjs.cloudflare.com/ajax/libs/highlight.js/<Version>/styles/<StyleName>.min.css`

EX.プライベートでAtom使ってるのでそのCSSソースをよく使う。

https://cdnjs.cloudflare.com/ajax/libs/highlight.js/9.15.6/styles/atom-one-dark.min.css

# 使い方
* jsソースとcssソースを用意する
* ソースコピペでもいいし以下でもいい
```html
<!-- これ書いとけば読み込んでくれる -->
<!-- バージョンとかスタイルとか公式サイト見て適宜いい感じにしてくれ -->
<link rel="stylesheet" href="//cdnjs.cloudflare.com/ajax/libs/highlight.js/9.15.6/styles/default.min.css">
<script src="//cdnjs.cloudflare.com/ajax/libs/highlight.js/9.15.6/highlight.min.js"></script>
```
* 適用させるページに以下のコードを書く
```html
<!-- このコードが読み込まれるページにシンタックスハイライトが適用される -->
<script>hljs.initHighlightingOnLoad();</script>
```

* シンタックスハイライトを適用させるテキストは以下タグで囲んで書く
```html
<pre><code>console.log("Hello World!")</code></pre>
<!-- codeタグにclassで明示的に言語を指定することもできる -->
<pre><code class="javascript">console.log("Hello World!")</code></pre>
```
