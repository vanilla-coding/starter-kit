# ๐  CSS ์ ํ์ Practice

### Selector (1)

ํ๊ทธ ์ ํ์๋ฅผ ์ฌ์ฉํด ์คํ์ผ์ ์ ์ฉ์์ผ ๋ด๋๋ค.

```css
tag {
  background-color: navy;
}
```

[Codepen์ผ๋ก ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/LYOpxOO)

### Selector (2)

ํด๋์ค ์ ํ์๋ฅผ ์ฌ์ฉํด ์คํ์ผ์ ์ ์ฉ์์ผ ๋ด๋๋ค.

```css
.class {
  background-color: orange;
}
```

[Codepen์ผ๋ก ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/mdqeRpG?editors=1100)

### Selector (3)

์์ด๋ ์ ํ์๋ฅผ ์ฌ์ฉํด ์คํ์ผ์ ์ ์ฉ์์ผ ๋ด๋๋ค.

```css
#id {
  background-color: orange;
}
```

[Codepen์ผ๋ก ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/jOabyZO?editors=1100)

### Selector (4)

HTML ๊ตฌ์กฐ์ ๋ฐ๋ผ ์๋ฆฌ๋จผํธ๋ฅผ ์ ํํด์ ์คํ์ผ์ ์ ์ฉํ  ์ ์์ต๋๋ค.

```css
/* div ํ๊ทธ ๋ด๋ถ์ ์๋ "๋ชจ๋  p ํ๊ทธ" ์๊ฒ ํด๋น ์คํ์ผ์ ์ ์ฉ */
div p {
  background-color: navy;
}

/* div ํ๊ทธ์ "์ง๊ณ ํ์ p ํ๊ทธ์๊ฒ๋ง" ํด๋น ์คํ์ผ์ ์ ์ฉ */
div > p {
  background-color: pink;
}
```

[Codepen์ผ๋ก ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/LYOpxQO?editors=1100)



### margin

margin์ ์๋ฆฌ๋จผํธ์ ๋ฐ๊นฅ์ชฝ ์ฌ๋ฐฑ๊ณผ ๊ด๋ จ๋ ์์ฑ์๋๋ค.

```css
div {
  margin: 10px;
}
```

[Codepen์ผ๋ก ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/WNXQRMV?editors=1100)

### padding

padding์ ์๋ฆฌ๋จผํธ์ ์์ชฝ ์ฌ๋ฐฑ๊ณผ ๊ด๋ จ๋ ์์ฑ์๋๋ค.

```css
div {
  padding: 10px;
}
```

[Codepen์ผ๋ก ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/abVvpYw)



### font family

CSS๋ฅผ ์ฌ์ฉํด HTML ํ๊ทธ ๋ด๋ถ์ ํ์คํธ์ ์ํ๋ ํฐํธ๋ฅผ ์ ์ฉ์ํฌ ์ ์์ต๋๋ค.

```css
p {
  font-family: "Font Name"
}
```

[Codepen์ผ๋ก ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/OJOyWvq?editors=1100)
