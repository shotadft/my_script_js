<p>僕が作ったスクリプト類。
<br />自作発言等禁止。</p>
<h2><a href="https://www.shotadft.com/my_script_js/script/app_prc.js">app_prc.js</a></h2>
<p>言語によって価格表示を変え、表示させるスクリプト。ウェブページ用。<br />
日本では&yen;、中国だと元、その他の言語だと$が表示されます。<br />ついでに複数の表示を別々のものにできます。</p>
<h3>導入</h3>
<p>先に以下のコードを&lt;body&gt;に記入する。<br />
基本、&lt;script&gt;は&lt;head&gt;に記入するが、エラー回避のため&lt;body&gt;に記入する。</p>

```html
<script type="module" src="https://www.shotadft.com/my_script_js/script/app_prc.js"></script>
```
<p>次にコードを入力する。</p>
<p><b>例：</b></p>

```html
<!--- 前略 --->
<body>
      <script type="module" src="https://www.shotadft.com/my_script_js/script/app_prc.js"></script>
      <script type="module">
        import { Price } from 'https://www.shotadft.com/my_script_js/script/app_prc.js';
        Price('id名', 500);
    </script>
<div id="id名"></div>
</body>
```
<p><b>置き換え</b></p>
<p>id名=文字列<br />
表示価格=数値</p>

<h3>サンプル</h3>

```html
<!DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta charset="UTF-8">
    <title>Sample1</title>
  </head>
  <body>
      <script type="module" src="https://www.shotadft.com/my_script_js/script/app_prc.js"></script>
      <script type="module">
        import { Price } from 'https://www.shotadft.com/my_script_js/script/app_prc.js';
        Price('A', 500);
        Price('B', 0);
    </script>
    <div id="A"></div>
    <div id="B"></div>
  </body>
</html>
```
<p><b>サンプルの実行結果</b></p>
<iframe
src="https://www.shotadft.com/my_script_js/SampleSite/sample1.html"
  title="Sample1"
  width="360"
  height="120">
</iframe>
<hr />
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />

> この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">クリエイティブ・コモンズ 表示 - 継承 4.0 国際 ライセンス</a>の下に提供されています。
