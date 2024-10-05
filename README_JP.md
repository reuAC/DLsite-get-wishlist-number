# DLsite-get-wishlist-number
DLsiteのお気に入りページからコンテンツID番号を取得します。

## はじめに
まず、DLsiteのお気に入りページに移動し、ブラウザの開発者ツールを開く必要があります。コンソールに、以下のコードのいずれかをコピーして実行してください。現在のページのお気に入りのコンテンツIDが印刷されます。

## 圧縮されていないバージョン
```javascript
var main = "";
document.querySelectorAll(".work_name > a").forEach((item)=>{
	main += "," + item.href.match(/RJ\d+/)[0];
});
```

## 圧縮バージョン
```javascript
var a="";document.querySelectorAll(".work_name > a").forEach(b=>{a+=","+b.href.match(/RJ\d+/)[0]});console.log(a)
});
```
