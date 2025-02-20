## 아이콘을 넣는 2가지 방법

> ### 첫번째 방법 <br>
>
> 직접 아이콘을 구하는 방법<br>
> 직접 이미지를 만들고 추출하거나 svg파일을 이용<br>
> ( SVG는 픽셀이 없는 이미지 파일형식, 수학으로만 구성된 형식)

> ### 두번째 방법 <br>
>
> html 언어로 넣을 수 있는 아이콘 사이트 활용하는 방법<br>
> Heroicons (https://heroicons.dev/) <br>
> → 무료 (아이콘 이미지가 크게 보임)
> FontAwesome (https://fontawesome.com/) <br>
> → 유료 (Kit Code를 받아야 사용 가능) <br>
> 아이콘 kit code 주소를 복붙할 때는 div 태그를 닫은 다음, body 태그를 닫기 직전에 위치 시켜준다 <br>

```</div>

    <script
      src="https://use.fontawesome.com/releases/v5.2.0/js/all.js"
      crossorigin="anonymous"
    ></script>
  </body>


*script태그* 는 항상 body 직전에 와야 한다.!!
```

<br>

---

<br>

> ### 아이콘 크기를 바꾸는 방법

```html
<i class="fas fa-battery-full"></i>
```

아이콘 이름 옆에 <<space>> fa-2x라고 붙여준다

```html
<i class="fas fa-battery-full fa-2x"></i>
```

```html
º 아이콘 크기
<i class="fas fa-user fa-xs"></i>
<i class="fas fa-user fa-sm"></i>
<i class="fas fa-user fa-lg"></i>
<i class="fas fa-user fa-2x"></i>
<i class="fas fa-user fa-3x"></i>
<i class="fas fa-user fa-5x"></i>
<i class="fas fa-user fa-7x"></i>
<i class="fas fa-user fa-10x"></i>
```

> ### 아이콘이 정해지지 않았을 때 <br>
>
> 주석처리로 표시함 <br>
> 주석: 프로그래머만 볼 수 있는 코드

```html
<!--  Icon -->
```

> css 상에서 주석처리 <br>

```css
/* To Do Icon */
```

## BEM 형식이란? <br>

BEM(Block Element Modifier) : 더 쉽게 읽히는 css를 가지게 함 <br>
예를 들어 <br>

```html
<div class="column"></div>
```

이 명칭은 너무 흔하기 때문에 아래처럼 쓰기를 권한다 <br>

```html
<div class="status-bar__column"></div>
```

많은 곳에 column은 존재할 수 있기에 css를 볼 때
어느 부분에 해당하는 column인지 찾이 어렵기 때문이다. <br>

```
☆ TIP ☆
class 이름 안에는 부모+자식으로 명시하면 가독성이 올라간간다.
```
