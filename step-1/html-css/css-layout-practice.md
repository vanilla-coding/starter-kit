# ๐  CSS Layout Practice

### layout with margin

margin ์์ฑ์ ์ฌ์ฉํด์ ์๋ฆฌ๋จผํธ๋ฅผ ์ํ ๊ฐ์ด๋ฐ ์ ๋ ฌ์ํฌ ์ ์์ต๋๋ค.

```css
div {
  margin: 0 auto;
}
```

[Codepen์ผ๋ก ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/ZEabLRO?editors=1100)

### position (1)

*   `position: static`

    ๋ฐ๋ก position์ ์ค์ ํ์ง ์์์ ๋์ ๊ธฐ๋ณธ๊ฐ
*   `position: relative`

    ์ฃผ๋ณ์ ๋ค๋ฅธ ์๋ฆฌ๋จผํธ๋ค๊ณผ์ ์๋์ ์ธ ์์น๋ฅผ ์ค์ ํ  ์ ์๊ฒ ๋ฉ๋๋ค.

```css
.class {
  position: relative;
}
```

![์ฌ์ง๊ณผ ๊ฐ์ ๋ชจ์์ผ๋ก ๋ง๋ค์ด์ฃผ์ธ์!](<../../.gitbook/assets/pos1 (1).png>)

[Codepen์ผ๋ก ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/ExbVZpX?editors=1100)

### position (2)

*   `position: absolute`

    ์ฃผ๋ณ์ ์๋ฆฌ๋จผํธ๋ ๋ฌด์ํ๊ณ , position์ด relative๋ก ์ค์ ๋์ด ์๋ ๊ฐ์ฅ ๊ฐ๊น์ด ์์ ์๋ฆฌ๋จผํธ๋ง์ ๊ธฐ์ค์ผ๋ก ์์น๋ฅผ ์ค์ ํ  ์ ์๊ฒ ๋ฉ๋๋ค.

```css
.class {
  position: absolute;
}
```

![์ฌ์ง๊ณผ ๊ฐ์ ๋ชจ์์ผ๋ก ๋ง๋ค์ด์ฃผ์ธ์!](../../.gitbook/assets/pos2.png)

[Codepen์ผ๋ก ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/VwrvPBd?editors=1100)

### layout - flex

flex๋ ํฌ๊ฒ ๋๊ฐ์ง ์์๋ก ๊ตฌ์ฑ๋ฉ๋๋ค.

* `flex container`: flex box ๋ค์ ๊ฐ์ธ๋ ์์์๋๋ค.
* `flex item`: ์ ์ฐ(flexible)ํ๊ฒ ๋์ด๋๊ฑฐ๋ ์ค์ด๋ค๋ฉฐ ๋ ์ด์์์ ๊ตฌ์ฑํ๋ ์์๋ค ์๋๋ค.

```css
.flex-container {
  display: flex;
}

.flex-box {
  flex: 1;
}
```

![์ฌ์ง๊ณผ ๊ฐ์ ๋ชจ์์ผ๋ก ๋ง๋ค์ด์ฃผ์ธ์!](../../.gitbook/assets/flex.png)

[Codepen์ผ๋ก ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/WNXQRgN?editors=1100)

### layout - flex (2)

flex-direction ์์ฑ์ ํตํด flex item๋ค์ด ์ ๋ ฌ๋  ๋ฐฉํฅ(์ถ)์ ๋ฐ๊ฟ ์ ์์ต๋๋ค.

```css
.flex-container {
  display: flex;
  flex-direction: column;
}
```

![์ฌ์ง๊ณผ ๊ฐ์ ๋ชจ์์ผ๋ก ๋ง๋ค์ด์ฃผ์ธ์!](../../.gitbook/assets/flex2.png)

[Codepen์ผ๋ก ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/QWOjdZw?editors=1100)

### layout - flex (3)

flex container์ `justify-content`์ `align-items` ์์ฑ์ ํตํด flex item๋ค์ ์ ๋ ฌ์ํฌ ์ ์์ต๋๋ค.

```css
.flex-container {
  display: flex;
  justify-content: center;
  align-items: center;
}
```

![์ฌ์ง๊ณผ ๊ฐ์ ๋ชจ์์ผ๋ก ๋ง๋ค์ด์ฃผ์ธ์!](../../.gitbook/assets/flex3.png)

[Codepen์ผ๋ก ์ง์  ํด๋ณด๊ธฐ](https://codepen.io/vanillacoding/pen/YzEyNJj?editors=1100)
