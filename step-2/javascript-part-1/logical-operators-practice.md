# ๐  Logical Operators Practice

### Quiz #1

```javascript
/*

  < Logical operators basic 1 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

const seven = 7;
const trueOrFalse = !!"";

const result = (seven && trueOrFalse);

if (result === ๐ฌ) {
  alert("๐");
}
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/02028834dbdfd5267d841e332f040809?editors=0010)



### Quiz #2

```javascript
/*

  < Logical operators basic 2 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

const empty = null;
const trueOrFalse = !0;
const str = "Vanillacoding";

const result = (empty || trueOrFalse || str);

if (result === ๐ฌ) {
  alert("๐");
}
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/ced6acd5a93e18a273b931dd8309da15?editors=0010)



### Quiz #3

```javascript
/*

  < Logical operators basic 3 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

const trueOrFalse = !null;
const zero = 0;
const str = "Vanillacoding";

const result = (trueOrFalse && zero && str);

if (result === ๐ฌ) {
  alert("๐");
}
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/98b6514ef92496137c7af9d42ae3ea3e?editors=0010)



### Quiz #4

```javascript
/*

  Ken์ ํ ๋ก ํ์ ์ฐธ์ํ์์ต๋๋ค.

  ๋ ๊ฐ์ง ์๊ฒฌ์ ํ ๋ก  ๊ฒฐ๊ณผ๋ logical operator์ ๋ฐ๋ผ ๊ฒฐ์ ๋ฉ๋๋ค.

  ํ ๋ก ์ ์ต์ข ๊ฒฐ๊ณผ๊ฐ truthy ๊ฐ์ด ๋๋๋ก ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

const Ryan = false;
const Blake = true;
const Scott = false;
const Ken = true;

const result = (Ryan || Blake) ๐ฌ (Scott && Ken);

if (result) {
  alert("๐");
}
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/9b2fb3a309605e295f86d173749d71d9?editors=0010)



