# π  Arrays

λ°°μ΄μ΄λ μ΄λ ν μ λ³΄(κ°)λ€μ **μμλλ‘** μ μ₯ν  μ μλ κ΅¬μ‘°μλλ€. μλμ κ°μ΄ λκ΄νΈλ₯Ό μ΄μ©ν΄ λ°°μ΄μ λ§λ€ μ μμ΅λλ€.

```javascript
var fruits = [ 'apple', 'orange', 'grape' ];
```

λ°°μ΄ μμ λ€μ΄μλ κ°λ€μ **μμ(element, item, etc)**λΌκ³  ν©λλ€.

μμ `fruits` λ³μμ λ΄κΈ΄ λ°°μ΄μ κ²½μ°, μ²« λ²μ§Έ μμλ `'apple'`(λ¬Έμμ΄ apple)μ΄κ³ , λ λ²μ§Έ μμλ `'orange'`(λ¬Έμμ΄ orange), μΈ λ²μ§Έ μμλ `'grape'`(λ¬Έμμ΄ grape)μλλ€. κ·Έλμ `fruits` λ³μμ λ΄κΈ΄ λ°°μ΄μ 3κ°μ μμλ₯Ό κ°κ³  μλ€κ³  ννν  μ μμ΅λλ€. &#x20;

νμ¬ μμ λ°°μ΄μμλ λͺ¨λ λ¬Έμμ΄ μμλ€μ΄ λ΄κ²¨μμ§λ§, μ¬λ¬λΆμ΄ μνλ μ΄λ€ κ°μ΄λΌλ λ°°μ΄μ μμλ‘ μΆκ°ν  μ μμ΅λλ€. μ’λ₯κ° λ€λ₯Έ κ°λ€λ ν¨κ» λ΄μ μ μμ΅λλ€.

```javascript
var arr = [ 1, '3', true ];
var arr1 = [ undefined, null, false, NaN, 1000 ];
```

#### λ°°μ΄μ κΈΈμ΄

λͺ¨λ  λ°°μ΄μ μμμ κ°―μμ λν μ λ³΄λ₯Ό μλμ κ°μ΄ `.length` μμ±μ μ΄μ©νμ¬ μ κ³΅ν΄μ€λλ€.

```javascript
var fruits = [ 'apple', 'orange', 'grape' ];
console.log(fruits); // [ 'apple', 'orange', 'grape' ]
console.log(fruits.length); // 3
```

μ΄μ  λ μ¨μμ ν¨μλ₯Ό λ°°μ μΌλ, λ°°μ΄μ κΈΈμ΄λ₯Ό λ°νν΄μ£Όλ ν¨μλ₯Ό νλ² λ§λ€μ΄λ³ΌκΉμ?

```javascript
var fruits = [ 'apple', 'orange', 'grape' ];
function getNumOfFruits () {
  return fruits.length;
}
var numOfFruits = getNumOfFruits();
console.log(numOfFruits); // 3
```

μ ν¨μλ `fruits`λΌλ λ³μμ λ΄κΈ΄ λ°°μ΄μ κΈΈμ΄λ§ λλ €μ£Όκ³  μμ΅λλ€. μ‘°κΈ μ¬μ© μ©λκ° μ νμ μΈ μν©μλλ€. λͺ¨λ  λ°°μ΄μ λν΄μ κΈΈμ΄ κ°μ λ°νν΄μ€ μ μλ ν¨μλ₯Ό λ§λ€μ΄λ³΄λ κ²μ μ΄λ¨κΉμ? ν¨μλ μΈμλ₯Ό λ°μ μ μκΈ° λλ¬Έμ, κ·Έλ° μ±μ§μ μ΄μ©νλ©΄ μ’μκ² κ°μ΅λλ€.

```javascript
function getNumOfItems (array) {
  return array.length;
}

var fruits = [ 'apple', 'orange', 'grape' ];
var numOfFruits = getNumOfItems(fruits);
console.log(numOfFruits); // 3
```

μ μμ  μ½λμ `getNumOfItems`λ λ§€κ° λ³μλ‘ `array`λΌλ κ²μ μ μΈν΄λμμ΅λλ€. κ·Έλ¦¬κ³  ν΄λΉ ν¨μλ₯Ό μ€ννλ©° μΈμλ‘ `fruits` λ°°μ΄μ λ£μ΄μ£Όκ³  μμ΅λλ€. κ·Έλ κΈ° λλ¬Έμ ν¨μ λ΄λΆμμ `array`λΌλ λ§€κ° λ³μλ `fruits`κ° λμλκ³ , `fruits`μ κΈΈμ΄λ₯Ό λ°ννκ² λ©λλ€.

μ‘°κΈ λ μ¬μ¬μ©μ΄ μ μ°ν΄μ§ ν¨μκ° μμ±λμμ΅λλ€.

#### λ°°μ΄μ μμ μ κ·Ό

λ°°μ΄μ κ²½μ°, λ¬Έμμ΄κ³Ό λ§μ°¬κ°μ§λ‘ κ° μμλ€μ μΈλ±μ€λ₯Ό μ΄μ©νμ¬ μ κ·Όν  μ μμ΅λλ€.

```javascript
var food = [ 'pasta', 'steak', 'rice' ];
var myFavoriteFood = food[1];
console.log(myFavoriteFood); // 'steak'
```

μΈλ±μ€λ₯Ό μ΄μ©νμ¬ λ°°μ΄μ ν΄λΉ μΈλ±μ€ μμΉμ μλ¦¬ν μμλ₯Ό μμ ν  μλ μμ΅λλ€.

```javascript
var fibonacci = [ 1, 2, 3, 5, 8, 13 ];

console.log(fibonacci[4]); // 8

fibonacci[4] = false;

console.log(fibonacci[4]); // false
```

#### λ°°μ΄μ μμ μΆκ°νκΈ°

μ°μ  μΈλ±μ€λ₯Ό μ΄μ©νμ¬ μνλ μμΉμ μμλ₯Ό μΆκ°ν  μ μμ΅λλ€.

```javascript
var arr = [];
arr[0] = true;
console.log(arr[0]); // true

arr[2] = true;
console.log(arr[2]); // true

console.log(arr); // [ true, undefined, true ]
```

λλ μλμ κ°μ΄ λ©μλλ₯Ό μ΄μ©ν  μλ μμ΅λλ€.

```javascript
var arr = [];

// push λ©μλλ λ°°μ΄μ λ€μ μμλ₯Ό μΆκ°ν©λλ€.
arr.push(1); // arrμ [1]μ΄ λ©λλ€.
arr.push(2); // arrμ [1, 2]κ° λ©λλ€.

// pop λ©μλλ λ°°μ΄μ λ€μμ νλμ μμλ₯Ό μ κ±°ν©λλ€.
arr.pop(); // arrμ λ€μ [1]μ΄ λ©λλ€.
arr.pop(); // arrμ λ€μ λΉ λ°°μ΄μ΄ λ©λλ€.
```

#### λ€μν λ°°μ΄ λ©μλ

[Array Methods](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/Array#%EB%A9%94%EC%84%9C%EB%93%9C)

μ λ§ν¬μμ μ¬λ¬ κ°μ§ λ©μλλ€μ νλ² νμ΅ν΄λ³΄μκΈ° λ°λλλ€.

### μΆκ° νμ΅ μλ£

* [Arrays - W3Schools](https://www.w3schools.com/js/js\_arrays.asp)
* [Arrays - Javascript Info](https://javascript.info/array)
* [Arrays - MDN](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/Array)
* [Arrays and Objects - Eloquent Javascript](https://eloquentjavascript.net/04\_data.html)
