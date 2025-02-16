## 폰트 추가 방법

> ### 내 컴퓨터에 없는 폰트를 보여주고 싶다면≣

1. google fonts (https://fonts.google.com/)<br>
2. 원하는 폰트를 선택 <br>
3. 글꼴 가져오기 선택 <br>
4. 우측 <>임베드 코드 받기 선택 <br>

- html의 head에 link or @import 를 써서 추가하는 방법<br>

```html
<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
<link
  href="https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300..800;1,300..800&family=Roboto:ital,wght@0,100..900;1,100..900&display=swap"
  rel="stylesheet"
/>
```

```html
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300..800;1,300..800&display=swap');
```

- css에 추가하는 방법

```css
body {
  font-family: "Roboto", serif;
}
```

## 적용

```style.css
@import url("https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300..800;1,300..800&display=swap");
body {
  font-family: "Open Sans", serif;
}

```
