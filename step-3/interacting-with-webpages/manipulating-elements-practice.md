# ๐  Manipulating Elements Practice

### Quiz #1

```javascript
/*

  < Manipulating Elements basic 1 >
  
  ํ๋ฉด์ "I am a paragraph"๋ผ๋ ํ์คํธ๊ฐ ๋ํ๋  ์ ์๋๋ก
  
  <p> ํ๊ทธ์ ํ์คํธ๋ฅผ ์ถ๊ฐํด์ฃผ์ธ์!
  
  ๐จ HTML, CSS๋ ๊ฑด๋๋ฆฌ์ง ์๊ณ  JS๋ง ์์ ํด์ฃผ์ธ์.

*/

const pElement = document.querySelector("p");
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/LYzKyJv?editors=1010)



### Quiz #2

```javascript
/*

  < Manipulating Elements basic 2 >
  
  "paragraph1"์ ์๋ "paragraph2"์ ๋์ผํ ๋จ์ด๊ฐ ๋๋๋ก
  
  ํฐํธ ์ฌ์ด์ฆ๋ 100px, ์์์ #55ff00๋ก ์์ ํด์ฃผ์ธ์!
  
  ๐จ HTML, CSS๋ ๊ฑด๋๋ฆฌ์ง ์๊ณ  JS๋ง ์์ ํด์ฃผ์ธ์.

*/

const itemElement = document.querySelector(".item");
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/jOGjmga?editors=1010)

###

### Quiz #3

```javascript
/*

  < Manipulating Elements basic 3 >
  
  ์ค๋ฅธ์ชฝ ์์๊ฐ ์ผ์ชฝ ์์์ ๊ฐ์ด "yellow" ์์์ ๊ฐ์ง ์ ์๋๋ก
  
  ๋ฐฐ๊ฒฝ์์ ์์ ํด์ฃผ์ธ์!
  
  ๐จ HTML, CSS๋ ๊ฑด๋๋ฆฌ์ง ์๊ณ  JS๋ง ์์ ํด์ฃผ์ธ์.

*/

const rightElement = document.querySelector(".right");
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/mdBZwpW?editors=1010)



### Quiz #4

```javascript
/*

  < Traffic Lights >
  
  ์ผ์ชฝ ์ ํธ๋ฑ์ ์ค๋ฅธ์ชฝ ์ ํธ๋ฑ๊ณผ ๊ฐ์ด
  
  Stop, Pause, Go๋ผ๋ ํ์คํธ๋ฅผ ์ถ๊ฐํด์ฃผ์๊ณ 
  
  red, orange, green ํด๋์ค๋ฅผ ์ถ๊ฐํ์ฌ
  
  ๋นจ๊ฐ์, ์ฃผํฉ์, ์ด๋ก์ ๋ฐฐ๊ฒฝ์์ ๊ฐ์ง ์ ์๋๋ก ์์ ํด์ฃผ์ธ์!
  
  ๐จ HTML, CSS๋ ๊ฑด๋๋ฆฌ์ง ์๊ณ  JS๋ง ์์ ํด์ฃผ์ธ์.
  
*/

const wrapperElement = document.querySelector(".lightWrapper");
const redLightElement = wrapperElement.children[0];
const orangeLightElement = wrapperElement.children[1];
const greenLightElement = wrapperElement.children[2];
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/jOGjYOJ)
