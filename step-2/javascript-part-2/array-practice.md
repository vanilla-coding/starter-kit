# ๐  Array Practice

### Quiz #1

```javascript
/*

  < Arrays basic 1 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

const fruitList = ["Apple", "Lemon", "Banana", "Melon"];
const fruitLength = fruitList.length;

if (fruitLength === ๐ฌ) {
  alert("๐");
}
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/mdBYjLB)



### Quiz #2

```javascript
/*

  < Arrays basic 2 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

const foodList = ["Pizza", "Hamburger", "Chicken", "Steak"];

const food1 = foodList[0];
const food2 = foodList[foodList.length - 1];

const result = food1 + food2;

if (result === ๐ฌ) {
  alert("๐");
}
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/eYGajrq)



### Quiz #3

```javascript
/*

  < Arrays basic 3 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/


const fruitList = ["Apple"];

fruitList.push("Lemon");
fruitList.push("Mango");

const fruit1 = fruitList[1];
const fruit2 = fruitList.pop();

const result = fruit1 + fruit2;

if (result === ๐ฌ) {
  alert("๐");
}
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/zYEQLLG)



### Quiz #4

```javascript
/*

  < Arrays basic 4 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

const animalList = ["Dog", "Cat", "Lion", "Koala"];
let result = "";

for (let i = 0; i < animalList.length; i++) {
  result += ๐ฌ;
}

if (result === "DogCatLionKoala") {
  alert("๐");
}
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/oNGRMMB)



### Quiz #5

```javascript
/*

  ์๋ฃ ์ํ๊ธฐ(machine)์ 4๊ฐ์ง ์ข๋ฅ์ ์๋ฃ ์ค์ "Sprite"๊ฐ ๋น ์ ธ์๋ค์

  ์ฐฝ๊ณ (storage)์์ ๋ถ์กฑํ ์๋ฃ์ ์ข๋ฅ๋ฅผ ์ฐพ์ ์ํ๊ธฐ์ ๋ง์ง๋ง ์์๋ก ์ฑ์์ง ์ ์๋๋ก

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

const machine = ["Coke", "Pepsi", "Fanta"];
const storage = ["Pepsi", "Coke", "Sprite", "Fanta"];

for (let i = 0; i < storage.length; i++) {
  if (machine.indexOf(storage[i]) === ๐ฌ) {
    machine.push(storage[i]);
  }
}

const result =  machine[machine.length - 1];

if (result === "Sprite") {
  alert("๐");
}
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/MWEdBBM)

