# π  Conditional Statements

### μ‘°κ±΄λ¬Έ μκ°

μλ°μ€ν¬λ¦½νΈμμ μ°λ¦¬λ μ΄λ€ μ‘°κ±΄μ μν΄ μ½λμ μ€νμ μ μ΄ν  μ μμ΅λλ€. μ°μ  μλμ μμ λ₯Ό λ³ΌκΉμ?

```javascript
if (false) {
  console.log("Hello, World!");
}
```

μ μ½λλ₯Ό μ€ννκ² λλ©΄, μ½μμ μλ¬΄λ° λ©μμ§λ λνλμ§ μμ΅λλ€. `if` κ΅¬λ¬Έμ΄ μ£Όμ΄μ§ μ‘°κ±΄μ μν΄ μ€κ΄νΈ(`{}`) λ΄λΆ μ½λμ μ€νμ μ μ΄ν κ²μλλ€. λ§μ½ μ μ½λμ μ‘°κ±΄μ΄ `false`κ° μλλΌ `true`μλ€λ©΄, μ€κ΄νΈ λ΄λΆ μ½λκ° μ€νλμμ κ²μλλ€.

μμ κ°μ΄ μ°λ¦¬λ μ΄λ€ μ‘°κ±΄μ μν΄ μ½λμ μ€νμ μ μ΄νκ³  μΆμλ `if` κ΅¬λ¬Έμ μ¬μ©ν  μ μμ΅λλ€.

```javascript
if (/* μ‘°κ±΄ */) {
  // μ€νλ¬Έ
}
```

### κΈ°λ³Έ μ¬μ©λ²

`if`λΌλ μμ΄ λ¨μ΄κ° λ»νλ― "λ§μ½μ AλΌλ©΄ Bλ₯Ό ν΄μ£ΌμΈμ."λΌκ³  μ»΄ν¨ν°μκ² λͺλ Ήμ λ΄λ¦΄ μ μλ κ²μλλ€.

μ‘°κΈ λ μκ°μ ν΄λ³Έλ€λ©΄, μλμ κ°μ ννμ νκ³  μΆμ μλ μμ΅λλ€.

**"λ§μ½μ AλΌλ©΄ Bλ₯Ό ν΄μ£ΌμΈμ. κ·Έλ°λ° λ§μ½μ CλΌλ©΄ Dλ₯Ό ν΄μ£ΌμΈμ. μλλ©΄ κ·Έλ₯ Eλ₯Ό ν΄μ£ΌμΈμ."**

μμ κ°μ ννμ μλμ²λΌ μμ±ν  μ μμ΅λλ€.

```javascript
// μλμ μ½λμμ Aμ CλΌλ κ²μ μ μλμ§ μμκΈ° λλ¬Έμ, μ μμ μΌλ‘ μ€νλμ§ μμ΅λλ€. λΉμ μ μΌλ‘ Aμ Cμ μ‘΄μ¬κ° μλ μν©μ κ°μ νμ¬ μμ±ν κ²μλλ€.

if (A) {
  // B..
} else if (C) {
  // D..
} else {
  // E..
}
```

### μ‘°κ±΄λ¬Έμ μ€μ²©

`if` κ΅¬λ¬Έμ μ¬λ¬λΆμ΄ μνλ λλ‘ μ€μ²©μμΌμ μ¬μ©νμ€ μ μμ΅λλ€.

```javascript
var something = true;
var moreSomething = true;

if (something) {
  console.log("I am inside something");

  if (moreSomething) {
    console.log("I am inside moreSomething");
  } else {
    console.log("I never gets called.");
  }
} else {
  console.log("I never gets called either.");
}
```

### μ μν  μ 

λ§μ½ `if..else` κ΅¬λ¬Έμ μ΄μ©νμ¬ μλμ κ°μ μ½λλ₯Ό μμ±νλ€κ³  μκ°ν΄λ³΄μΈμ.

```javascript
if (A) {
  // one..
} else if (B) {
  // two..
} else if (C) {
  // three..
} else if (D) {
  // four..
} else if (E) {
  // five..
} else {
  // six..
}
```

μμ `if..else if`μμ λ³΄λ©΄, 6κ°μ§ μ‘°κ±΄μ΄ μμ΅λλ€. `A ~ E` κ·Έλ¦¬κ³  `else`κ° μμ΅λλ€.

μ μνμ€ μ μ ν­μ μ  μ‘°κ±΄λ€ μ€, _λ¨ ν κ°μ§μ μ‘°κ±΄λΆ μ½λλ§ μ€νλλ€λ κ²μλλ€._ μ€μ¬ Aμ Cκ° λͺ¨λ μ°Έμ΄λΌ ν΄λ, A μ‘°κ±΄μ ν΄λΉνλ μ½λλ§ μ€νλκ³  C μ‘°κ±΄μ ν΄λΉνλ μ½λλ μ€νλμ§ μμ΅λλ€. μ΄κ²μ `else if`λΌλ κ΅¬λ¬Έ λλ¬Έμλλ€. `else`λΌλ λ¨μ΄λ "μλλ©΄\~"μ΄λΌλ λ»μ΄κΈ° λλ¬Έμλλ€.

### ν΄μ¦

{% tabs %}
{% tab title="JavaScript" %}
```javascript
// #1. λ¬΄μμ΄ μΆλ ₯λ κΉμ?
if (true) {
  console.log(1);
} else if (true) {
  console.log(2);
} else {
  console.log(3);
}

// #2. λ¬΄μμ΄ μΆλ ₯λ κΉμ?
if ("") {
  console.log(1);
} else if ("a") {
  console.log(2);
} else {
  console.log(3);
}

// #3. λ¬΄μμ΄ μΆλ ₯λ κΉμ?
if (null) {
  console.log(1);
} else if (5) {
  console.log(2);
} else {
  console.log(3);
}
```

Truthy κ°μ΄ μ‘°κ±΄μΌλ‘ μ£Όμ΄μ§ κ²½μ°, ν΄λΉ μ‘°κ±΄λ¬Έμ΄ μ€νλκ³  κ·Έλ μ§ μμ κ²½μ° λ€μ μ‘°κ±΄μΌλ‘ λμ΄κ°λλ€.
{% endtab %}
{% endtabs %}

### μΆκ° νμ΅ μλ£

* [if..else - MDN](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Statements/if...else)
* [switch - MDN](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Statements/switch) (`if` κ΅¬λ¬Έκ³Ό λΉμ·ν κΈ°λ₯μ νλ `switch` κ΅¬λ¬Έμλλ€. νλ² μ΄ν΄λ³΄μΈμ.)
* [Control Flow - PoiemaWeb](https://poiemaweb.com/js-control-flow#21-ifelse-%EB%AC%B8)
* [if..else - W3Schools](https://www.w3schools.com/js/js\_if\_else.asp)
