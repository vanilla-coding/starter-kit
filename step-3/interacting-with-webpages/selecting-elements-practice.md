# ๐  Selecting Elements Practice

### Quiz #1

```javascript
/*

  < Selecting Elements basic 1 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

const $p1 = document.getElementById("first-item");
const $p2 = document.getElementsByClassName("third-item");

const text1 = $p1.textContent;
const text2 = $p2[0].textContent;

const result = text1 + text2;

if (result === ๐ฌ) {
  alert("๐");
}
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/rNYapVK?editors=1010)



### Quiz #2

```javascript
/*

  < Selecting Elements basic 2 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

const $li = document.getElementsByTagName("li");
const $p = document.getElementsByTagName("p");

const text1 = $li[2].textContent;
const text2 = $p[1].textContent;

const result = text1 + text2;

if (result === ๐ฌ) {
  alert("๐");
}
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/zYPxpqm)



### Quiz #3

```javascript
/*

  < Selecting Elements basic 3 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

const $item = document.querySelectorAll(".item");
const $li = document.querySelectorAll("li");

const length1 = $item.length;
const length2 = $li.length;

const result = length1 + length2;

if (result === ๐ฌ) {
  alert("๐");
}
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/mdqypre?editors=1010)
