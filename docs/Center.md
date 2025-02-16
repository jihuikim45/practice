## 컨테이너 하나를 중심에 놓는 방법

> ### justify-content를 사용 <br>

```
.status-bar {
  display: flex;
  justify-content: space-between;
}
```

다른 width를 가지고 있기 때문에 space-between이 안 맞을 수 있있다는 단점이 있음

> ### css hack <br>
>
> 레시피 같이 어디서든 적용이 가능 <br>

> <h3> 상위 박스<br> <h5>justify-content: center; <h5>중앙으로 배치 <br>

---

> <h3> 내부 박스<br> <h5>width: 33%; <h5>왼쪽으로 몰려서 범위가 벌어진다 <br> 왼쪽에 위치할 박스는 왼쪽에 붙어서 정렬된다 <br>

---

> <h3> 중앙에 위치할 박스<br>  <h5>display: flex;justify-content: center; <br> <h5> 중앙에 위치할 박스만 중앙에 위치한다 <br>

---

> <h3> 오른쪽에 정렬할 박스<br> <h5>display: flex;justify-content: flex-end; <br> align-items: center; <br> <h5>오른쪽에 붙어서 정렬된다

<h3> º상위박스

```html
.status-bar { display: flex; justify-content: center; padding: 5px 3px; }
```

<h3> º내부박스

```html
.status-bar__column { width: 33%; }
```

.status-bar\_\_column:first-child span {
margin-right: 5px;
}

<h3> º중앙 박스

```html
.status-bar__column:nth-child(2) { display: flex; justify-content: center; }
```

<h3> º우측 박스

```html
.status-bar__column:last-child { display: flex; justify-content: flex-end;
align-items: center; }
```

.status-bar\_\_column .fa-battery-full {
margin: 0px 5px;
}
