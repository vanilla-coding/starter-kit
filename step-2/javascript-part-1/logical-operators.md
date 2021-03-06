# π  Logical Operators

### Logical NOT Operator

* `!`λ₯Ό μ΄μ©ν΄ ννν©λλ€.
* `!` λ€μ μ€λ κ°μ `true`(Boolean)μΌλ‘ λ³νν  μ μλ€λ©΄ `false`λ₯Ό λ°ννκ³ , κ·Έλ μ§ μμ κ²½μ° `true`λ₯Ό λ°νν©λλ€.

```javascript
!true;                 // false
!2;                    // false
!"abc";                // false
!(function foo () {})  // false
!{ name: 'ken' }       // false

!false;                // true
!"";                   // true
!0;                    // true
```

#### Truthy and Falsy

μ΄μ  λ¨κ³μμ λ°°μ λ€μνΌ, μλ°μ€ν¬λ¦½νΈμ λͺ¨λ  κ°λ€μ **μλ£νμ λ°λΌ 7κ°μ§λ‘** λλ μ μμ΅λλ€.

μλ£νκ³Ό λλΆμ΄ μλ°μ€ν¬λ¦½νΈμ κ°λ€μ λλλ λ λ€λ₯Έ κΈ°μ€μ΄ ν κ°μ§ λ μμ΅λλ€. κ·Έκ²μ΄ **λ°λ‘ Truthinessμ Falsinessμλλ€.** νκ΅­λ§λ‘ ν΄μνμλ©΄, "μ§μ€κ°μ μ±κ²©"(Truthiness)μ "κ±°μ§κ°μ μ±κ²©"(Falsiness)μλλ€. μλ°μ€ν¬λ¦½νΈμ λͺ¨λ  κ°λ€μ λ μ€ ν κ°μ§μ μν©λλ€.

μλμ λμ΄λ κ°λ€μ λͺ¨λ Falsyμλλ€. μ¦, `false`λ‘ λ³νλλ κ°μλλ€.

{% tabs %}
{% tab title="JavaScript" %}
{% code title="Falsy κ° λͺ©λ‘" %}
```javascript
0
-0
false
undefined
null
""
''
``
NaN
```
{% endcode %}

{% hint style="success" %}
**μμ λμ΄λμ§ μμ κ°λ€μ λͺ¨λ Truthyμλλ€.** μ¦, `true`λ‘ λ³νλλ κ°μλλ€.
{% endhint %}
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="JavaScript" %}
```javascript
Boolean([ 1, 2, 3 ]);         // true? false?
Boolean([]);                  // true? false?
Boolean({ name: 'hello' });   // true? false?
Boolean({});                  // true? false?
Boolean('abc');               // true? false?
Boolean('  ');                // true? false?
Boolean('   '.trim());        // true? false?
Boolean(300);                 // true? false?
Boolean(-10);                 // true? false?
Boolean(function foo () {});  // true? false?
```

μμ μ€νλ¬Έλ€μ κ²°κ³Όλ₯Ό μΆμΈ‘ν΄λ³΄μκ³ , νμΈν΄λ³΄μκΈ° λ°λλλ€.
{% endtab %}
{% endtabs %}

### Logical OR Operator

* `||`λ‘ ννν©λλ€.
* `true`λ `false`κ°μ΄ μλ, νΌμ°μ°μ(operand) κ°μ΄ λ°νλ©λλ€.

#### μ°μ° λ°©μ

1. μ°μ°μλ₯Ό κΈ°μ€μΌλ‘ μΌμͺ½λΆν° Truthy κ°μ μ°Ύμ΅λλ€.
2. Truthy κ°μ μ°Ύμ κ²½μ°, μ°μ°μ μ€μ§νκ³  ν΄λΉ κ°μ λ°νν©λλ€.
3. λ§μ§λ§κΉμ§ Truthy κ°μ μ°Ύμ§ λͺ»ν κ²½μ°, λ§μ§λ§μ μμΉν κ°μ λ°νν©λλ€.

{% tabs %}
{% tab title="JavaScript" %}
```javascript
true || true;                   // ?
true || false;                  // ?
false || true;                  // ?
false || false;                 // ?
"hello" || {};                  // ?
[] || "hello";                  // ?
(function foo () {}) || "hello";  // ?
false || "";                    // ?
```

μμ μ€νλ¬Έλ€μ κ²°κ³Όλ₯Ό μΆμΈ‘ν΄λ³΄μκ³ , νμΈν΄λ³΄μκΈ° λ°λλλ€.
{% endtab %}
{% endtabs %}

### Logical AND Operator

* `&&`λ‘ ννν©λλ€.
* `true`λ `false`κ°μ΄ μλ, νΌμ°μ°μ(operand) κ°μ΄ λ°νλ©λλ€.

#### μ°μ° λ°©μ

1. μ°μ°μλ₯Ό κΈ°μ€μΌλ‘ μΌμͺ½λΆν° Falsy κ°μ μ°Ύμ΅λλ€.
2. Falsy κ°μ μ°Ύμ κ²½μ°, μ°μ°μ μ€μ§νκ³  ν΄λΉ κ°μ λ°νν©λλ€.
3. λ§μ§λ§κΉμ§ Falsy κ°μ μ°Ύμ§ λͺ»ν κ²½μ°, λ§μ§λ§μ μμΉν κ°μ λ°νν©λλ€.

{% tabs %}
{% tab title="JavaScript" %}
```javascript
true && true;                  // ?
true && false;                 // ?
false && true;                 // ?
false && false;                // ?
"hello" && {};                 // ?
[] && "hello";                 // ?
"" && "hello";                 // ?
(function foo () {}) && "hello"; // ?
false && "";                   // ?
```

μμ μ€νλ¬Έλ€μ κ²°κ³Όλ₯Ό μΆμΈ‘ν΄λ³΄μκ³ , νμΈν΄λ³΄μκΈ° λ°λλλ€.
{% endtab %}
{% endtabs %}

### Operator Precedence

{% hint style="success" %}
AND μ°μ°μμ μ°μ μμκ° OR μ°μ°μμ μ°μ μμλ³΄λ€ λμ΅λλ€.
{% endhint %}

![MDNμ μ°μ°μ μ°μ μμ νμ΄λΈ](../../.gitbook/assets/1-2.png)

{% embed url="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Operator_Precedence" %}

### μΆκ° νμ΅ μλ£

* [Logical Operators - Javascript Info](https://javascript.info/logical-operators)
* \[λΌλ¦¬ μ°μ°μ - MDN]\([https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Operators/%EB%85%BC%EB%A6%AC\_%EC%97%B0%EC%82%B0%EC%9E%90(Logical\_Operators](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Operators/%EB%85%BC%EB%A6%AC\_%EC%97%B0%EC%82%B0%EC%9E%90\(Logical\_Operators)))
