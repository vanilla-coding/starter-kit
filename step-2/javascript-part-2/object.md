# ๐  Object

๊ฐ์ฒด๋ผ๊ณ  ํ๋ ๊ฒ์ key/value pair๋ฅผ ์ ์ฅํ  ์ ์๋ ๊ตฌ์กฐ์๋๋ค.

key/value๊ฐ ๋ฌด์์ผ๊น์? ์ด๋ค ์ฌ๋์ ํ๋กํ์ ์์ฑํ๋ค๊ณ  ์๊ฐํด๋ด์๋ค. ์๋์ ๊ฐ์ด ์์ฑํ  ์ ์์ต๋๋ค.

< ์ฌ๋ 1 >

* ์ด๋ฆ: Ken Huh
* ๋์ด: 13
* ์ฃผ์: ์์ธํน๋ณ์ ๊ฐ๋จ๊ตฌ ์ผ์ฑ๋ก 86๊ธธ 20

์์์ "์ด๋ฆ", "๋์ด", "์ฃผ์"๋ฅผ key๋ผ๊ณ  ํ  ์ ์๊ณ , ๊ทธ์ ํด๋นํ๋ ๊ฐ ์ ๋ณด๋ฅผ value๋ผ๊ณ  ๋ถ๋ฅผ ์ ์์ต๋๋ค.

> key: "์ด๋ฆ", "๋์ด", "์ฃผ์" value: "Ken Huh", 13, "์์ธํน๋ณ์ ๊ฐ๋จ๊ตฌ ์ผ์ฑ๋ก 86๊ธธ 20"

์ ์ ๋ณด๋ฅผ ์๋ฐ์คํฌ๋ฆฝํธ ๊ฐ์ฒด๋ก ํํํด๋ณด์๋ฉด ์๋์ ๊ฐ์ด ํ  ์ ์์ต๋๋ค.

```javascript
var person1 = {
  name: "Ken Huh",
  age: 13,
  address: "์์ธํน๋ณ์ ๊ฐ๋จ๊ตฌ ์ผ์ฑ๋ก 86๊ธธ 20"
};
```

์๋ฐ์คํฌ๋ฆฝํธ์์ ๊ฐ์ฒด๋ ์ค๊ดํธ ํ๊ธฐ๋ฅผ ์ด์ฉํ์ฌ ๋ง๋ค ์ ์๊ณ , ๊ฐ๊ฐ์ key/value์ ๋ํ ์ ๋ณด๋ฅผ ์์ ๊ฐ์ด ๋์ดํ  ์ ์์ต๋๋ค. ํ ์์ key/value ๋ค์ "์ผํ"๋ฅผ ์ด์ฉํ์ฌ ๊ทธ ๋ค์ ์ค๋ key/value์ ๊ตฌ๋ถํด์ฃผ์ด์ผ ํฉ๋๋ค.

### ๊ฐ์ฒด์ ์ ์ฅ๋ ๋ด์ฉ ๊ฐ์ ธ์ค๊ธฐ

๊ฐ์ฒด์ ์ ์ฅ๋ ์ ๋ณด๋ ์๋์ ๊ฐ์ด ์ ๊ทผํ์ฌ ๊ฐ์ ธ์ฌ ์ ์์ต๋๋ค.

```javascript
var person1 = {
  name: "Ken Huh",
  age: 13,
  address: "์์ธํน๋ณ์ ๊ฐ๋จ๊ตฌ ์ผ์ฑ๋ก 86๊ธธ 20"
};

var myName = person1.name;
var myAge = person1.age;

console.log(myName); // "Ken Huh"
console.log(myAge); // 13
```

์๋์ ๊ฐ์ด๋ ํ  ์ ์์ต๋๋ค.

```javascript
var person1 = {
  name: "Ken Huh",
  age: 13,
  address: "์์ธํน๋ณ์ ๊ฐ๋จ๊ตฌ ์ผ์ฑ๋ก 86๊ธธ 20"
};

var myName = person1["name"];
var myAge = person1["age"];

console.log(myName); // "Ken Huh"
console.log(myAge); // 13
```

{% tabs %}
{% tab title="JavaScript" %}
```javascript
const person = {
  name: 'Ken Huh',                       // ์์ฑ ์ด๋ฆ - 'name', ์์ฑ ๊ฐ - 'Ken Huh'
  age: 36,                               // ์์ฑ ์ด๋ฆ - 'age', ์์ฑ ๊ฐ - 36
  'languages': [ 'Korean', 'English' ],  // ์์ฑ ์ด๋ฆ - 'languages', ์์ฑ ๊ฐ - ๋ฐฐ์ด
  'ํ๊ตญ ๋์ด': 36                          // ์์ฑ ์ด๋ฆ - 'ํ๊ตญ ๋์ด', ์์ฑ ๊ฐ - 36
};
```

์์์ `person` ๋ณ์์ ํ ๋น๋ ๊ฐ์ฒด์๋ 4๊ฐ์ ์์ฑ(Key)๊ฐ ์ ์ฅ๋์์ต๋๋ค.

`'languages'`์ `'ํ๊ตญ ๋์ด'`์ ๊ฐ์ด ์์ฑ ์ด๋ฆ ๋ถ๋ถ์ ๋ฌธ์์ด์ ์จ๋ ์๊ด์์ต๋๋ค๋ง, `'ํ๊ตญ ๋์ด'`์ ๋ค์ด๊ฐ ๊ณต๋ฐฑ๊ณผ ๊ฐ์ด **์๋ณ์์ ํ์ฉ๋์ง ์๋ ๋ฌธ์๊ฐ ๋ค์ด๊ฐ ์์ฑ ์ด๋ฆ**์ ์ ์ํ  ๋๋ **๋ฐ๋์ ๋ฌธ์์ด ํ๊ธฐ(๋ฐ์ดํ)๋ฅผ ์ฌ์ฉ**ํด์ผ ํฉ๋๋ค.

**๋ฐ์ดํ๊ฐ ๊ตณ์ด ํ์ํ์ง ์์ ๊ฒฝ์ฐ(`name`, `age`, `languages`)์๋ ์ผ๋ฐ์ ์ผ๋ก ๋ฐ์ดํ๋ฅผ ์ฌ์ฉํ์ง ์์ต๋๋ค.**
{% endtab %}
{% endtabs %}

#### ์๋ณ์ (Identifier)

![MDN ๋ฌธ๋ฒ๊ณผ ์๋ฃํ](../../.gitbook/assets/1-5.png)

### ๊ฐ์ฒด์ ์๋ก์ด key/value ์ถ๊ฐํ๊ธฐ

```javascript
var person = {
  name: "Ken Huh"
};

console.log(person.name); // "Ken Huh"
console.log(person.age); // undefined (์กด์ฌํ์ง ์๋ key/value)

// ์ถ๊ฐ
person.age = 13; // ํน์ person["age"] = 13;

console.log(person.age); // 13
```

### ๊ฐ์ฒด key/value ์์ ํ๊ธฐ

```javascript
var person = {
  name: "Ken Huh",
  age: 13
};

console.log(person.name); // "Ken Huh"
console.log(person.age); // 13

// ์์ 
person.age = 15; // ํน์ person["age"] = 15;

console.log(person.age); // 15
```

### ๊ฐ์ฒด key/value ์ญ์ ํ๊ธฐ

```javascript
var person = {
  name: "Ken Huh",
  age: 13
};

console.log(person.name); // "Ken Huh"
console.log(person.age); // 13

// ์ญ์ 
delete person.age;

console.log(person.age); // undefined (๋ ์ด์ ์กด์ฌํ์ง ์๋ key/value)
```

### ๊ฐ์ฒด ์ํํ๊ธฐ

์ฃผ๋ก ๊ฐ์ฒด์ Key/Value๋ฅผ ์ํํ๊ธฐ ์ํ ๋ชฉ์ ์ผ๋ก ์ฌ์ฉ๋ฉ๋๋ค.

```javascript
const sample = {
  one: 1,
  two: 2,
  three: 3
};

for (let prop in sample) {
  console.log(prop);
  console.log(sample[prop]);
}
```

* `prop` ๋ณ์์ `in` ์ฐ์ฐ์ ๋ค์ ์์นํ ๊ฐ์ฒด์ ์์ฑ๋ค์ด ํ๋์ฉ ๋ด๊น๋๋ค.
  * ์๋ฅผ ๋ค์ด, ์ฒซ ๋ฐ๋ณต ๋๋ `prop` ๋ณ์์ ๊ฐ์ `"one"`, ๋๋ฒ์งธ ๋ฐ๋ณต ์์๋ `"two"`, ์ธ๋ฒ์งธ ๋ฐ๋ณต ์์๋ `"three"` ๋ฑ์๋๋ค.
* ๊ฐ์ฒด์ ์์ฑ์ ๋๊ดํธ๋ฅผ ์ด์ฉํ์ฌ ์ ๊ทผํ  ์ ์๊ธฐ ๋๋ฌธ์, `sample[prop]`์ ์ด์ฉํ์ฌ ํด๋น ํค๊ฐ์ Value๋ฅผ ์ฌ์ฉํ  ์๋ ์์ต๋๋ค.

{% hint style="info" %}
๊ฐ์ฒด์ Key/Value๋ ์์๋ฅผ ์ ์ํ  ์ ์์ต๋๋ค. ๊ทธ๋์ **for In loop์ ์์๋ ์์๋ก ์ ํด์ง๋๋ค.** ์ฆ, for in loop ๋ด๋ถ์ ์์ฑํ ์ฌ๋ฌ๋ถ์ ๋ก์ง์ด Key/Value์ ์์์ ์์กดํ๋ค๋ฉด ๊ทธ ์ฝ๋๋ ๋ถ์์ ํ๋ค๋ ์๋ฏธ์๋๋ค.\
\
์ฐธ๊ณ ๋งํฌ: [MDN](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Statements/for...in)
{% endhint %}

{% tabs %}
{% tab title="JavaScript" %}
```javascript
const me = 'Ken Huh';

function getAge () {
  return 36;
}

const person = {
  name: me,
  age: getAge()
};
```

๊ฐ์ฒด ๋ฆฌํฐ๋ด์ ์ด์ฉํด ์์ฑ์ ์ง์ ํ  ๋, ์์ ๊ฐ์ด ์ด๋ฏธ ์ ์๋ ๋ณ์๋ ํจ์๋ฅผ ์ด์ฉํ์ฌ Value๋ก ์ง์ ํ  ์๋ ์์ต๋๋ค.
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="JavaScript" %}
```javascript
const property = 'name';

const obj = {
  [property]: 'Ken Huh'
};

obj.property;  // undefined
obj.name;      // 'Ken Huh'
```

์์ ๊ฐ์ด ๋๊ดํธ๋ฅผ ์ฌ์ฉํด์ ๋ค๋ฅธ ๋ณ์์ ์ ์ฅ๋ ๋ฌธ์์ด์ ์์ฑ(Key)์ ์ด๋ฆ์ผ๋ก ์ฐ๋ ๊ฒ๋ ๊ฐ๋ฅํฉ๋๋ค.
{% endtab %}
{% endtabs %}

### Dot Notation, Bracket Notation

์๋์ ๊ฐ์ด **์์ฑ ์ ๊ทผ์(property accessor)**๋ฅผ ์ด์ฉํด ์ด๋ฏธ ์์ฑ๋ ๊ฐ์ฒด์ ์์ฑ์ ๋ํ Value๋ฅผ ๊ฐ์ ธ์ฌ ์๋, ๋๋ ์ง์ ํด์ค ์๋ ์์ต๋๋ค.

```javascript
const person = {}; // Empty

// Dot notation
person.name = 'Ken Huh';
person.age = 36;
person.languages = ['Korean', 'English'];

console.log(person);
console.log(person.age);
console.log(person.languages);
```

์์์๋ ๊ฐ์ฒด ๋ฆฌํฐ๋ด์ ์ด์ฉํด ๋น ๊ฐ์ฒด๋ฅผ ์์ฑํด ์ค ๋ค, **Dot Notation**์ ํตํด ์์ฑ์ ๊ฐฑ์ ํด์ฃผ์์ต๋๋ค. ๊ทธ๋ฌ๋, JavaScript์์ ์๋ณ์๋ก ํ์ฉ๋์ง ์๋ ๋ฌธ์๊ฐ ๋ค์ด๊ฐ ์์ฑ ์ด๋ฆ์ ์ฌ์ฉํด์ผ ํ๋ ๊ฒฝ์ฐ์๋ ๋ฐ๋์ **Bracket notation**์ ์ฌ์ฉํด์ผ ํฉ๋๋ค.

```javascript
// Bracket notation
person['ํ๊ตญ ๋์ด'] = 36;
```

์์ ๊ฐ์ด ํน๋ณํ ๊ฒฝ์ฐ๊ฐ ์๋๋ผ๋ฉด, **์ผ๋ฐ์ ์ผ๋ก Dot Notation์ด ๋ง์ด ์ฌ์ฉ๋๋ ํธ์๋๋ค.**

### Method

๊ฐ์ฒด์ ์์ฑ๊ฐ์ผ๋ก **ํจ์**๋ฅผ ์ง์ ํ  ์๋ ์์ต๋๋ค. **์ด๋ค ๊ฐ์ฒด์ ์์ฑ์ผ๋ก ์ ๊ทผํด์ ์ฌ์ฉํ๋ ํจ์**๋ฅผ **method**๋ผ๊ณ  ๋ถ๋ฆ๋๋ค.

```javascript
const person = {
  greet: function() {
    return 'hello';
  }
};

person.greet(); // 'hello';
```

### Arrays and Functions

์๋ฐ์คํฌ๋ฆฝํธ์์๋ ๋ฐฐ์ด๊ณผ ํจ์ ๋ํ ๊ฐ์ฒด๋ผ๋ ๋ฒ์ฃผ์ ํฌํจ๋ฉ๋๋ค. ๋ฐฐ์ด๊ณผ ํจ์ ๋ํ ์ผ๋ฐ ๊ฐ์ฒด์ ๋์ผํ ์ฑ์ง์ ๊ฐ๊ณ  ์์ต๋๋ค.

```javascript
const arr = [ 1, 2, 3 ];

console.log(arr[0]);    // 1
console.log(arr.title); // undefined

arr.title = 'Vanilla Coding';

console.log(arr.title); // 'Vanilla Coding'
```

```javascript
function foo (a, b) {
  return a + b + 3;
}

console.log(foo.title); // undefined

foo.title = 'Vanilla Coding';

console.log(foo.title); // 'Vanilla Coding'

console.log(foo(1, 2)); // 6
```

์ ์์ ์ฒ๋ผ ๋ฐฐ์ด์ด๋ ํจ์ ๋ํ ๊ฐ์ฒด์ ํ ์ข๋ฅ์ด๊ธฐ ๋๋ฌธ์, ์ฐ๋ฆฌ๊ฐ ์ํ๋ค๋ฉด ์์ฑ์ ์ถ๊ฐํ  ์ ์์ต๋๋ค. ํ์ง๋ง ์ผ๋ฐ์ ์ผ๋ก ๋ฐฐ์ด์ด๋ ํจ์์ ์ฐ๋ฆฌ๊ฐ ๋ณ๋์ ์์ฑ์ ์ถ๊ฐํ์ฌ ์ฌ์ฉํ๋ ๊ฒฝ์ฐ๋ ๊ฑฐ์ ์๊ณ  ์ฃผ๋ก ๊ธฐ๋ณธ์ ์ผ๋ก ์ ๊ณต๋ ์์ฑ๊ณผ ๋ฉ์๋๋ฅผ ์ฌ์ฉํฉ๋๋ค.

### ์ถ๊ฐ ํ์ต ์๋ฃ

* [Objects - W3Schools](https://www.w3schools.com/js/js\_object\_definition.asp)
* [Objects - Javascript Info](https://javascript.info/object)
