# ๐  Hoisting Practice

### Quiz #1

```javascript
/*

  < Hoisting basic 1 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

function foo() {
  if (result === ๐ฌ) {
    alert("๐");
  }

  var result = "something"; // const, let, var์ ์ฐจ์ด๋ ๋ฌด์์ผ๊น์ ?
}

foo();
```

[Codepen์ผ๋ก ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/QWObpem)



### Quiz #2

```javascript
/*

  < Hoisting basic 2 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

let something = "Something";
let result = null;

function foo () {
  if (something === "Something") {
    result = "Is something";
  }
  
  var something = "Else";
}

foo();

if (result === ๐ฌ) {
  alert("๐");
}
```

[Codepen์ผ๋ก ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/abVOJee)



### Quiz #3

```javascript
/*

  ์๋ ์ฝ๋์์ "bar ๐" ์ฑ๊ณต ์๋ฆผ์ฐฝ ๋ํ๋  ์ ์๋๋ก ๋ง๋ค์ด์ฃผ์ธ์!

*/

foo();
bar(); // bar ํจ์ ์คํ๋ฌธ์ ์์น๋ฅผ ์ฎ๊ฒจ์ฃผ์ธ์.

function foo() {
  console.log("foo ๐");
}

const bar = function () {
  alert("bar ๐");
};
```

[Codepen์ผ๋ก ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/ZEaGKzV)
