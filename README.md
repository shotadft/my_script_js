<p>僕が作ったスクリプト類。
<br />自作発言等禁止。</p>

## [app_prc.js](https://www.shotadft.com/my_script_js/script/app_prc.js)
<p>言語によって価格表示を変え、表示させるスクリプト。ウェブページ用。<br />
日本では&yen;、中国だと元、その他の言語だと$が表示されます。<br />ついでに複数の表示を別々のものにできます。</p>
<h3>導入</h3>
<p>以下のコードを&lt;body&gt;に記入する。<br />
基本、&lt;script&gt;は&lt;head&gt;に記入するが、エラー回避のため&lt;body&gt;に記入する。</p>

```html
<script type="module" src="https://www.shotadft.com/my_script_js/script/app_prc.js"></script>
```
<p>なお、&lt;div&gt;にid要素を入れないと動作しないので要注意。</p>

<h3>プロパティ</h3>
<p><b>必須プロパティ</b></p>

| プロパティ名 | 属性        | 説明                                                               | 構文                | サポート       | 
| ------------ | ----------- | ------------------------------------------------------------------ | ------------------- | -------------- | 
| Price        | string, int | このスクリプトのメイン関数です。<br/><br /> string = &lt;div id="string"&gt;&lt;/div&gt; | Price(string, int); | **サポート中** | 
<p><b>推奨プロパティ</b></p>

| プロパティ名     | 属性                 | 説明                                        | 構文                        | サポート                | 
| ---------------- | -------------------- | ------------------------------------------- | --------------------------- | ----------------------- | 
| setFreePriceText | bool<br />true or false | 価格が0だった場合に無料表記をつけるかどうか<br />現在使用不可 | setFreePriceText = Boolean; | **非サポート** - 開発中 | 
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
// importで関数を呼び出し
        import { Price } from 'https://www.shotadft.com/my_script_js/script/app_prc.js';

// 関数定義
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
src="https://www.shotadft.com/my_script_js/SampleSite/app_prc_js/sample1.html"
  title="Sample1"
  width="360"
  height="120">
</iframe>
<hr />
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />

> この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">クリエイティブ・コモンズ 表示 - 継承 4.0 国際 ライセンス</a>の下に提供されています。
