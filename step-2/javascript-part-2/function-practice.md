# ๐  Function Practice

### Quiz #1

```javascript
/*

  < Function basic 1 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

function sayHello(name) {
  return `Hello, ${๐ฌ}`;
}

const result = sayHello("Jett");

if (result === "Hello, Jett") {
  alert("๐");
}
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/ff557febf996cb0a0b8b3e5ee0b72975)



### Quiz #2

```javascript
/*

  < Function basic 2 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

function greetingMaker(greet, name) {
  return `๐ฌ`;
}

const hello = greetingMaker("Hello", "Jett");
const goodBye = greetingMaker("Goodbye", "Justin");

const result = (hello === "Hello, Jett") && (goodBye === "Goodbye, Justin");

if (result) {
  alert("๐");
}
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/xxXNJLG)



### Quiz #3

```javascript
/*

  < Function basic 3 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

function findStaff(name) {
  if (name === "Jett") {
    return "Staff";
  }

  if (name === "Leo") {
    return "Staff";
  }

  return "Spy";
}

const isFound1 = findStaff("Leo");
const isFound2 = findStaff("Jett");

const result = (isFound1 === isFound2);

if (result === ๐ฌ) {
  alert("๐");
}
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/zYEQLEO)



### Quiz #4

```javascript
/*

  < Making Hamburger with Functions >

  ํ๋ฒ๊ฑฐ๋ฅผ ๋ง๋ค์ด ๋จน์ผ๋ ค๊ณ  ํฉ๋๋ค. ํ์ฌ๋ ํ ๋งํ ๊ฐ ๋น ์ ธ์๋ค์ ๐

  ์์ฑ๋ ํ๋ฒ๊ฑฐ์ ๋์ผํ๋๋ก ๐ฌ ๋ฅผ ์ ์ ํ ๋ด์ฉ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

let myBurger = "Hamburger";

const addCheese = function (burger) {
  const cheese = " with Cheese";

  return burger + cheese;
};

const addPatty = function (burger) {
  const patty = " with Patty";

  return burger + patty;
};

const addTomato = ๐ฌ;

myBurger = addCheese(myBurger);
myBurger = addPatty(myBurger);
myBurger = addTomato(myBurger);

if (myBurger === "Hamburger with Cheese with Patty and Tomato") {
  alert("๐");
}
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/53d82a88cffdcd23fbb84e54b7df74ce)



### Quiz #5

```javascript
/*

  < Simple subtraction function >
  
  ๋ ๊ฐ์ง ์ธ์๋ฅผ ๋ฐ์ ํฐ ์์์ ์์ ์๋ฅผ ๋นผ์ฃผ๋ ํจ์๋ฅผ ์์ฑํด์ฃผ๋ ค๊ณ  ํฉ๋๋ค. 

  ์๋ ์กฐ๊ฑด์ด ํต๊ณผํ  ์ ์๋๋ก ๐ฌ ๋ฅผ ์ ์ ํ ๋ด์ฉ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

const subtraction = ๐ฌ;

const sum1 = subtraction(10, 3);
const sum2 = subtraction(7, 12);

const result = sum1 + sum2;

if (result === 12) {
  alert("๐");
}
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/jOGopZQ)

