# ๐  Reference Practice

### Quiz #1

```javascript
/*

  < Reference basic 1 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

const person1 = { name: "Jett", age: 30 };
const person2 = { name: "Jett", age: 30 };

const result = (person1 === person2);

if (result === ๐ฌ) {
  alert("๐");
}
```

[Codepen์ผ๋ก ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/JjOdNoj)



### Quiz #2

```javascript
/*

  < Reference basic 2 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

const person1 = { name: "Jett", age: 30 };
const person2 = person1;

person2.name = "Ken";

const result = (person1.name + person2.name);

if (result === ๐ฌ){
  alert("๐");
}

```

[Codepen์ผ๋ก ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/RwjPVNo?editors=0010)



### Quiz #3

```javascript
/*

  < Reference basic 3 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

const fruitList = ["Apple", "Banana"];
const fruitList2 = fruitList;

fruitList2.push("Melon");

const fruit1 = fruitList[fruitList.length - 1];
const fruit2 = fruitList2[fruitList2.length - 1];

const result = (fruit1 + fruit2);

if (result === ๐ฌ) {
 alert("๐");
}
```

[Codepen์ผ๋ก ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/PoOqmwj)



### Quiz #4

```javascript
/*

  < Copy ID >

  ์ ๋ถ์ฆ์ ๋ณต์ฌํ  ์ ์๋ ๋ ๊ฐ์ ํจ์๊ฐ ์์ต๋๋ค.

  ๊ฐ ํจ์๋ฅผ ํตํด ๋ณต์ฌํ ์ ๋ถ์ฆ์ ์ด๋ฆ์ด ๋ฌด์์ธ์ง

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

const ID = { name: "Jett", age: 30 };

function copyMachine1(obj1) {
  const newID1 = {};

  for (const key in obj1) {
    newID1[key] = obj1[key];
  }

  return newID1;
}

function copyMachine2(obj2) {
  const newID2 = obj2;

  return newID2;
}

const copyID1 = copyMachine1(ID);
const copyID2 = copyMachine2(ID);

ID.name = "Ken";

const result1 = (copyID1.name === ๐ฌ);
const result2 = (copyID2.name === ๐ฌ);

if (
  result1 &&
  result2
) {
  alert("๐");
}
```

[Codepen์ผ๋ก ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/MWOwmYZ)
