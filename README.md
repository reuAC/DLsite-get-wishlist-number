# DLsite-get-wishlist-number
Retrieving content ID numbers from the favorites page on DLsite.
[ English | [中文](https://github.com/reuAC/DLsite-get-wishlist-number/blob/re_uAC/README_CN.md) | [日本語](https://github.com/reuAC/DLsite-get-wishlist-number/blob/re_uAC/README_JP.md) ]

## Introduction
You need to first navigate to the favorites page on DLsite, then open the browser's developer tools. In the console, copy and execute one of the code versions below. The content IDs of the favorites on the current page will then be printed.

## Uncompressed version
```javascript
var main = "";
document.querySelectorAll(".work_name > a").forEach((item)=>{
	main += "," + item.href.match(/RJ\d+/)[0];
});
```

## Compressed version
```javascript
var a="";document.querySelectorAll(".work_name > a").forEach(b=>{a+=","+b.href.match(/RJ\d+/)[0]});console.log(a)
});
```
