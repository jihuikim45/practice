# form의 2가지 속성(attribute)

> ## 1. action <br> <h4> 어떤 페이지로 data를 보낼건지 지정할 수 있음. <br>

```html
<form action="friends.html" id="login-form"></form>
```

> ## 2. method <br> <h4> ⅼ. POST 방식 <br> : 백엔드 서버에 정보를 전송하는 방식. <br> <br> Ⅱ. GET 방식 <br> : 보안에 취약한 단점이 있음. <br> → username, password를 GET 방식으로 보내면 절대 안 됨. <br> → 따라서, URL에 포함되어도 상관없는 정보들을 GET 방식으로 보낸다. <br> <br> "file:///D:/cocoatalk/friends.html?username=dkanrjsk&Password=1234" <br> <br> URL에 이렇게 표시 됨.
