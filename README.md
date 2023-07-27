<p>僕が作ったスクリプト類</p>
<h2><a href="https://www.shotadft.com/my_script_js/script/app_prc.js">app_prc.js</a></h2>
<p>言語によって価格表示を変え、表示させるスクリプト。ウェブページ用。</p>
<h3>導入</h3>
<p>先に以下のコードを&lt;head&gt;に記入する。</p>

```html
<script src="https://www.shotadft.com/my_script_js/script/app_prc.js"></script>
```
<p>次に、&lt;body&gt;に ``` onload ``` 属性を追加し、内容としてコードを入力する。</p>
<p><b>例：</b></p>

```html
<body onload="Price(id名1, 表示価格);">
<!--- 中略 --->
<div id=id名1></div>
<!--- 中略 --->
</body>
```
<p><b>仕様書</b></p>
<p>置き換え：</p>
<p>id名=文字列<br />
表示価格=数値</p>

<h3>サンプル</h3>
