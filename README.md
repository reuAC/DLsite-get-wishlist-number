# DLsite-get-wishlist-number
从DLsite的收藏页面检索内容ID号码。  
[ 中文 | [English](https://github.com/reuAC/DLsite-get-wishlist-number/blob/re_uAC/README_EN.md) | [日本語](https://github.com/reuAC/DLsite-get-wishlist-number/blob/re_uAC/README_JP.md) ]

## 介绍
你需要先打开DLsite的收藏页面，而后打开浏览器开发者工具，并在控制台复制并执行（回车即执行）下面其中一个版本的代码，随后页面内全部的收藏内容的编号会被打印出来

## 无压缩版本
```javascript
var main = "";
document.querySelectorAll(".work_name > a").forEach((item)=>{
	main += "," + item.href.match(/RJ\d+/)[0];
});
```

## 压缩版本
```javascript
var a="";document.querySelectorAll(".work_name > a").forEach(b=>{a+=","+b.href.match(/RJ\d+/)[0]});console.log(a)
});
```
