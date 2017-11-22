# Vue.js_study

Javascript フレームワーク
Vue.jsの勉強用リポジトリ

///////2017.11.22　勉強開始！！

とりあえず、公式のガイドに従ってやってみよう。
<a href="https://jp.vuejs.org/v2/guide/">公式ガイド</a>

## 開発環境
- Windows10 64bit
- Brackets


## 勉強したこと
### オプション/DOM
- el<br>
DOM要素にVueのインスタンスを与える。セレクタを指定できる。<br>
要は、DOMとVueオブジェクトの紐づけって感じかな。
<a href="https://jp.vuejs.org/v2/api/index.html#el">elオプション</a>

### オプション/データ
- data<br>
elで指定した（というかバインドされた?）要素内から{{ }}を使った記法を使うことで参照できるようだ。<br>
たとえば、
```
var vm = new Vue({
  el: '#example', // document.getElementById('example'), $('#example')[0] も可
  data: {
    name: 'みかん',
    price: 100
  }
});
```
```
<div id="example">
  <p>{{ name }} は {{ price }}円</p>
</div>
```
この場合、出力結果は
```
みかんは１００円
```
そして、このdataを動的に変更することで画面(View)を変更する事ができるみたい。<br>
<a href="https://jp.vuejs.org/v2/api/index.html#data">dataオプション</a>