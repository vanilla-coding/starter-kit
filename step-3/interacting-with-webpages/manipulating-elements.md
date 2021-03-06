# π  Manipulating Elements

{% embed url="https://vimeo.com/352501832" %}

DOMμ μ΄μ©νμ¬ μ νν μμλ€μ νμμ λ°λΌ μμ νκ±°λ μ­μ ν  μλ μμ΅λλ€.

```markup
<div class="container">
  <h1>I am a Heading</h1>
  <p>I am a Paragraph</p>
  <ul>
    <li class="item">
      <p>I am a Paragraph</p>
    </li>
    <li class="item">
      <p>I am a Paragraph</p>
    </li>
    <li class="item">
      <p>I am a Paragraph</p>
    </li>
  </ul>
  <button id="special-button">I am a Button</button>
</div>
```

μμ κ°μ HTML λ¬Έμκ° μκ³ , `h1` μμμ νμ€νΈλ₯Ό λ³κ²½νκ³  μΆμ μν©μ΄λΌκ³  μκ°ν΄λ³΄μΈμ.

μμ  λ¨κ³μμ νμ΅νλ λ°©μ μ€ νλλ₯Ό μ΄μ©νμ¬ `h1` μμλ₯Ό μ νν ν, ν΄λΉ μμμ νμ€νΈλ₯Ό μμ ν΄λ³΄κ² μ΅λλ€.

```javascript
const $heading = document.querySelector("h1");

$heading.textContent = "I am a NEW Heading";
```

μμ μμ μ²λΌ `textContent`λ μμ±μ μ΄μ©νμ¬ `h1` μμμ νμ€νΈ λ΄μ©μ μμ ν  μ μμ΅λλ€.

λ§μ½ μ¬λ¬λΆκ»μ HTML μμλ₯Ό λμμΌλ‘ μ΄λ ν μμμ ν΄μΌ νλ μν©μΈλ°, μ΄λ»κ² ν΄μΌ ν μ§ λͺ¨λ₯΄μ λ€λ©΄ κ°μ₯ μ’μ λ°©λ²μ μΈν°λ· κ²μμλλ€. `"μλ°μ€ν¬λ¦½νΈ HTML μμ νμ€νΈ μμ "` λ±μ ν€μλλ‘ κ²μνμλ©΄ νμν μ λ³΄λ€μ μ°ΎμΌμ€ μ μμ΅λλ€. λν [Node](https://developer.mozilla.org/ko/docs/Web/API/Node) λ¬Έμλ [Element](https://developer.mozilla.org/ko/docs/Web/API/Element) λ¬Έμμ μΌμͺ½ "κ΄λ ¨ μ£Όμ "μ λμ΄λ μμ±μ΄λ λ©μλλ₯Ό μ΄ν΄λ³΄μκ³  μ μ©ν΄λ³Ό μλ μμ΅λλ€.

[`Node.textContent`](https://developer.mozilla.org/ko/docs/Web/API/Node/textContent)μ λν νμ΄μ§μμ μλ μͺ½ μμ  μ½λλ₯Ό λ³΄μλ©΄ λ°©κΈ μμμ λ³΄μ¬λλ¦° λ°©μμΌλ‘ νμ€νΈλ₯Ό μμ ν  μ μμμ μ μ μμ΅λλ€.

> κ΅¬κΈλ§ν μ λ³΄λ MDNμμ μ°Ύμ μ λ³΄λ₯Ό λ°λ‘ μ μ©νκΈ° μ΄λ ΅λ€λ©΄ jsbin.com λ±μ μΉ μλν°μμ κ°λ¨νκ² νμ€νΈν΄λ³΄μΈμ.

#### μμ£Ό μ¬μ©ν  λ§ν μμ±λ€

μλ λμ΄λ μμ±μ΄λ λ©μλλ μμ£Ό μ¬μ©λλ κ²λ€μ΄λ λ°λμ μμ§ν΄λ³΄μκΈ° λ°λλλ€.

* [Element.children - μμ μμ κ°μ Έμ€κΈ°](https://developer.mozilla.org/ko/docs/Web/API/ParentNode/children)
* [Element.classList - μμμ ν΄λμ€ μ λ³΄](https://developer.mozilla.org/ko/docs/Web/API/Element/classList)
* [Element.innerHTML - μμμ HTML](https://developer.mozilla.org/ko/docs/Web/API/Element/innerHTML)
* [Element.style - μμμ CSS μ€νμΌ](https://developer.mozilla.org/en-US/docs/Web/API/ElementCSSInlineStyle/style)
* [Element.remove - μμ μ­μ νκΈ°](https://developer.mozilla.org/ko/docs/Web/API/ChildNode/remove)
* [Element.appendChild - μμ μμ μΆκ°νκΈ°](https://developer.mozilla.org/ko/docs/Web/API/Node/appendChild)

