# ๐  Scope Chain Practice

### Quiz #1

```javascript
/*

  < Scope Chain basic 1 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

const name = "Jett";

function foo() {
  const name = "Justin";

  if (name === ๐ฌ) {
    alert("๐");
  }
}

foo();
```

[Codepen์ผ๋ก ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/GROJWLN)



### Quiz #2

```javascript
/*

  < Scope Chain basic 2 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

const name = "Jett";

function foo() {
  if (true) {
    const name = "Justin";
  }
	
  if (name === ๐ฌ) {
    alert("๐");
  }
}

foo();
```

[Codepen์ผ๋ก ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/QWObpPQ)



### Quiz #3

```javascript
/*

  < Scope Chain basic 3 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

let result = "";

function parent() {
  const role = "Parent";

  result += role;

  function child() {
    const role = "Children";

    result += role;
  }

  child();
}

parent();

if (result === ๐ฌ) {
  alert("๐");
}
```

[Codepen์ผ๋ก ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/dyZovEY)



### Quiz #4

```javascript
/*

  ์ฐ์ด๊ฐ ํ์ฐจ๊ฒ ๊ฐ๋ฌผ์ ๊ฑฐ์ฌ๋ฌ ์ฌ๋ผ๊ฐ๋ฏ,

  ์ค์ฝํ ์ฒด์ธ๋ ํ์์์ ์์ ์ฒด์ธ์ผ๋ก ๊ฑฐ์ฌ๋ฌ ์ฌ๋ผ๊ฐ๋ฉฐ ๊ฐ์ ํ์ํฉ๋๋ค.

  ๊ฐ river1, river2, river3 ์ด๋ผ๋ ๊ฐ๋ฌผ์ ๊ฑฐ์ฃผํ๊ณ  ์๋ ์ฐ์ด์ ์๊ฐ ๋ค๋ฆ๋๋ค

  ์ด ์ฐ์ด์ ์๊ฐ ๋ช ๋ง๋ฆฌ์ธ์ง ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

function river1 () {
  const salmon1 = 3;

  function river2 () {
    const salmon2 = 7;

    function river3 () {
      const salmon3 = 13;
      const result = (salmon1 + salmon2 + salmon3);

      if (result === ๐ฌ) {
        alert("๐");
      }
    }
  
    river3();
  }
  
  river2();
}

river1();
```

[Codepen์ผ๋ก ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/gOXpmNm)
