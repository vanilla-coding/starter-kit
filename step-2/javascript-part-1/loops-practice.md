# ๐  Loops Practice

### Quiz #1

```javascript
/*

  < Loops basic 1 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

  console.log(slogan[0]);
  console.log(slogan[1]);
  console.log(slogan[2]);
  console.log(slogan[3]);
  console.log(slogan[4]);
  console.log(slogan[5]);
  ...
  ...
  ...
  console.log(slogan[20]);
  console.log(slogan[21]);
  console.log(slogan[22]);

*/

const slogan = "Progress Not Perfection";

for (let i = 0; i < slogan.length; ๐ฌ) {
  console.log(slogan[i]);
}

alert("๐");
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/b157e4743dd1ae297eecfc28886af5fb?editors=0010)



### Quiz #2

```javascript
/*

  < Breaking the for loop >

  ๋ฐ๋๋ผ์ฝ๋ฉ์ ์ฌ๋ก๊ฑด์์ ๋ฌธ์ n์ ์ฐพ์๋ด๋ ค๊ณ  ํฉ๋๋ค.

  n์ ๋ฐ๊ฒฌํ๋ฉด ๋ฐ๋ณต๋ฌธ์ ๋ฉ์ถฐ์ฃผ๊ธฐ ์ํด ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

const slogan = "Progress, not perfection";
let result = null;

for (let i = 0; i < slogan.length; i++) {
  result = slogan[i];

  if (slogan[i] === "n") {
    ๐ฌ;
  }
}

if (result === "n") {
  alert("๐");
}
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/05435c17533bb9498b7db05ddf094c01?editors=0010)



### Quiz #3

```javascript
/*

  < Skipping the for loop >

  ์ด๋ฒ์๋ n, o, t ๊ฐ ๋์ค๋ฉด ๋ฐ๋ณต๋ฌธ ์คํ์ ๊ฑด๋๋ฐ์ด์

  ๊ฒฐ๊ณผ์ ์ถ๊ฐ๋์ง ์๋๋ก ํ๋ ค๊ณ  ํฉ๋๋ค.

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

const slogan = "Progress, not perfection";
let result = "";

for (let i = 0; i < slogan.length; i++) {
  if (slogan[i] === "n" || slogan[i] === "o" || slogan[i] === "t") {
    ๐ฌ;
  }

  result += slogan[i];
}

if (result === "Prgress,  perfeci") {
  alert("๐");
}
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/34037032b1c757e8a2438974420c3963?editors=0010)



