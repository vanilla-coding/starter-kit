# π  Scope Quiz

μλ μμ  μ½λλ₯Ό λ³΄κ³  μ΄λ€ κ²°κ³Όκ° λμ¬μ§ μ€μ€λ‘ μΆμΈ‘νκ³  νκ΅¬ ν΄λ³΄μΈμ.

{% tabs %}
{% tab title="JavaScript" %}
{% code title="Quiz 1" %}
```javascript
function foo () {
  var a = 5;

  for (var i = 0; i < a; i++) {
    console.log(a);
  }

  console.log(i);  // λ¬΄μμ΄ μΆλ ₯λ κΉμ?
}

foo();
```
{% endcode %}

#### Q1. Line 8μμ μΆλ ₯λλ κ°μ?

1. `0`
2. `5`
3. `4`
4. `undefined`
5. `Error`
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="JavaScript" %}
{% code title="Quiz 2" %}
```javascript
var a = 1;

function bar () {

  function foo() {
    console.log(a);  // ?
  }

  foo();
}

bar();
```
{% endcode %}

#### Q2. Line 6μμ μΆλ ₯λλ κ°μ?

1. `1`
2. `undefined`
3. `Error`
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="JavaScript" %}
{% code title="Quiz 3" %}
```javascript
var a = 1;

function bar () {

  function foo() {
    console.log(a);  // ?
  }
  
  a = 2;

  foo();
}

bar();
```
{% endcode %}

#### Q3. Line 6μμ μΆλ ₯λλ κ°μ?

1. `1`
2. `2`
3. `undefined`
4. `Error`
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="JavaScript" %}
{% code title="Quiz 4" %}
```javascript
function foo() {
  var a = 1;

  function bar () {
    a = 2;
  }

  console.log(a); // ?
  bar();
}

foo();
```
{% endcode %}

#### Q4. Line 8μμ μΆλ ₯λλ κ°μ?

1. `1`
2. `2`
3. `undefined`
4. `Error`
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="JavaScript" %}
{% code title="Quiz 5" %}
```javascript
var x = 1; 
  
function foo () { 
    if (x > 1) { 
        var x = 2; 
    } 
  
    console.log(x); 
} 
  
foo(); 
```
{% endcode %}

#### Q5. Line 8μμ μΆλ ₯λλ κ°μ?

1. `1`
2. `2`
3. `undefined`
4. `Error`
{% endtab %}
{% endtabs %}
