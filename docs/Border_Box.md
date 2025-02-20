## CSS box model defalt value

css에서 하단처럼 명령을 내렸을 때,

```html
.nav { position: fixed; bottom: 0; width: 100%; padding: 20px 50px; }
```

내가 원한 box size는 padding 값 포함 with 100을 유지하는 것이었지만, <br>
브라우저가 이해하기를 with 100이 padding 값 50px 만큼 <br>
줄어들었기 때문에 그 만큼 50px을 늘려버린다. <br>
따라서, 설정한 아이콘이 사라질 위험이 크다. <br>

#### ※ 해결 방법

box-sizing: border-box; 명령어를 입력해준다. <br>
→ CSS에게 "내가 padding을 줘도 신경쓰지 마. 내 box 사이즈를 늘리지 말아 줘" 라는 의미이다. <br>
CSS에게 box 사이즈를 변경하지 말라고 알려줘야 함.

```html
.nav { position: fixed; bottom: 0; width: 100%; padding: 20px 50px; box-sizing:
border-box; }
```
