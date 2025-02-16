## not

#### not이란?

뭔가가 적용되는 것을 원하지 않을 때

```html
body :not(crazy, fancy) { font-family: sans-serif; }
```

```html
body :not
<p></p>
```

```css
#login-form input {
  border: none;
  padding: 15px 0px;
  font-size: 18px;
  margin-bottom: 25px;
}

#login-form input:not([type="submit"]) {
  border-bottom: 1px solid rgba(0, 0, 0, 0.2);
}
```

```html
<form id="login-form">
  <input type="text" placeholder="Email or phone number" />
  <input type="Password" placeholder="Password" />
  <input type="submit" value="Log In" />
  <input type="submit" value="Sign Up" />
  <a href="#">Find Kokoa Account or Password</a>
</form>
```

> input:not([type="submit"] 코드의 의미는 input type이 submit이이 아니다. <br> []이 사이에 쓰인 것들은 특성 선택자 (attribute selector)이다.
