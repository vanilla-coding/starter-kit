# ๐  Object Practice

### Quiz #1

```javascript
/*

  < Object basic 1 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

const person = {
  age: 30,
  name: "Jett",
  address: "Seoul"
};

const name = person["name"];
const age = person.age;

const result = `${name} ${age}`;

if (result === ๐ฌ) {
  alert("๐");
}
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/gOGJjJz)



### Quiz #2

```javascript
/*

  < Object basic 2 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!

*/

const person = {
  age: 35,
  name: "Justin",
  address: "Busan"
};

delete person.address;

const result = person.address;

if (result === ๐ฌ) {
  alert("๐");
}
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/rNGgrEO)



### Quiz #3

```javascript
/*

  < Object basic 3 >

  ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์!
	
  console.log(`Person age 30`);
  console.log(`Person name Jett`);
  console.log(`Person address Seoul`);
	
*/

const person = {
  age: 30,
  name: "Jett",
  address: "Seoul"
};

for (const prop in person) {
  console.log(`Person ${prop} ${๐ฌ}`);
}
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/gOGJjNK)



### Quiz #4

```javascript
/*

  < Personal Inforamtion >

  ๋ฐ๋๋ผ์ฝ๋ฉ์ ์ ์ฐ์ค๋ฅ๋ก ์ธํด ์๊ฐ์์ ๊ฐ์ธ์ ๋ณด์ ์ค๋ฅ๊ฐ ์๊ฒผ๋ค์

  ์ค๋ฅ ์ ๋ณด์(errorInfo)์ key value ๊ฐ์ ์์ ํ์ฌ ์ฌ๋ฐ๋ฅธ ์ ๋ณด(correctInfo)์ 

  ๊ฐ์ด ๊ฐ์์ง ์ ์๋๋ก ๐ฌ ๋ฅผ ์ ์ ํ ๊ฐ์ผ๋ก ๊ณ ์ณ์ฃผ์ธ์ !

*/

let isInfoValid = true;

const correctInfo = {
  name: "Jett",
  age: 30,
  isVacoder: true
};

const errorInfo = {
  name: "Jett",
  age: 20,
  habit: "Running",
};

errorInfo.๐ฌ = 30;
errorInfo.๐ฌ = true;
delete ๐ฌ;

for (const prop in errorInfo) {
  if (errorInfo[prop] !== correctInfo[prop]) {
    isInfoValid = false;
  }
}

if (isInfoValid) {
  alert("๐");
}
```

[Codepen์์ ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/eYGajqN)

