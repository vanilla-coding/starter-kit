# π  Creating Elements

μμ κ³Ό μ­μ κ° κ°λ₯νλ―, μ°λ¦¬κ° μνλλλ‘ μμ±ν  μλ μμ΅λλ€. μμ  μ½λμ ν¨κ» λ³΄μ¬λλ¦¬κ² μ΅λλ€.

```javascript
// h1 μμ λ§λ€μ΄μ `heading`μ΄λΌλ λ³μμ ν λΉ
const heading = document.createElement("h1");

// λ°©κΈ μμ±ν `heading` μμμ νμ€νΈ μ€μ 
heading.textContent = "μ λͺ©μλλΉ";
// λ°©κΈ μμ±ν `heading` μμμ μ€νμΌ μ€μ 
heading.style.fontSize = "50px";

// λ°©κΈ μμ±ν `heading` μμλ₯Ό body νκ·Έμ μμμΌλ‘ μΆκ°
document.body.appendChild(heading);
```

μ μμ μ²λΌ μ°λ¦¬κ° μνλ μμλ₯Ό λ§λ€κ³ , κΈμ¨λ₯Ό μμ νκ³  μ€νμΌλ μμ ν  μ μμ΅λλ€. κ·Έλ¦¬κ³  μ°λ¦¬κ° μνλ μλ¦¬μ μΆκ°ν  μλ μμ΅λλ€.

> μ°λ¦¬κ° μλ°μ€ν¬λ¦½νΈλ‘ μμ±ν μμλ μ°λ¦¬κ° μ§μ  νλ©΄ μ΄λκ°μ λͺμμ μΌλ‘ μΆκ°νκΈ° μ κΉμ§λ μκ°μ μΌλ‘ νλ©΄μ λνλμ§ μμ΅λλ€. μλ₯Ό λ€λ©΄, μ μμ  μ½λμμ `document.body.appendChild(heading);`λΌλ μ½λκ° μμλ€λ©΄, headingμ νλ©΄μ λνλμ§ μμ΅λλ€.

#### π¨ ν΄μ¦

μλ λ κ°μ§ μμ  μ½λμ μ°¨μ΄μ μ λΆλ³ν΄λ³΄μΈμ.

{% code title="Example 1" %}
```javascript
const something = document.createElement("p");

for (let i = 0; i < 5; i++) {
  something.textContent = i;
  document.body.appendChild(something);
}
```
{% endcode %}

{% code title="Example 2" %}
```javascript
for (let i = 0; i < 5; i++) {
  const something = document.createElement("p");
  something.textContent = i;
  document.body.appendChild(something);
}
```
{% endcode %}
