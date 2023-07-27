<p>僕が作ったスクリプト類</p>
<h2><a href="https://www.shotadft.com/my_script_js/script/app_prc.js">app_prc.js</a></h2>
<p>言語によって価格表示を変え、表示させるスクリプト。ウェブページ用。</p>
<h3>導入</h3>
<p>先に以下のコードを&lt;head&gt;に記入する。</p>

```html
<script src="https://www.shotadft.com/my_script_js/script/app_prc.js"></script>
```
<p>次にコードを入力する。</p>
<p><b>例：</b></p>

```html
<head>
<script>
document.addEventListener("DOMContentLoaded", function()
  {
    window.globalFunction.Price(id名1, 表示価格);
  });
</script>
</head>
<body>
<!--- 中略 --->
<div id=id名1></div>
<!--- 中略 --->
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
    <script>
      document.addEventListener("DOMContentLoaded", function()
      {
          window.globalFunction.Price('A', 500);
      });
    </script>
  </head>
  <body>
    <div id="A"></div>
  </body>
</html>
```
<p><b>サンプルの実行結果</b></p>
<iframe
  src="https://www.shotadft.com/my_script_js/SampleSite/Sample1.html"
  title="Sample1"
  width="400"
  height="300">
</iframe>
