<Web2-javascript>
- html은 정적이다
- 사용자와 상호작용할 수 있게 js사용

# 1. html과 js가 만나는 3가지 방법
## 1.1 script 태그
- js는 html위에서 동작하는 언어
- html은 정적, js는 동적
```
  <body>
    <h1>JavaScript</h1>
    <script>
      document.write(1+1) #2를 출력
    </script>
    <h1>html</h1>
    hello world
    1+1   #1+1 을 그대로 출력
  </body>
```
- javascript코드라는 것을 웹브라우저에 알려주기 위해서는 
`<script></script>`라는 코드로 알려준다. 




## 1.2 event(이벤트)
- `onclick` 속성(attribute)은 아주 특별: 
  + 'onclick 속성의 값으로는 반드시 js가 와야 한다'라는 규칙.
  + 'onclick 속성의 속성 값은 웹브라우저가 기억하고 있다가 onclick이 위치하고 있는 태그를 사용자가 클릭했을 때 기억하고 있던 js코드를 js문법에 따라 해석해서 웹브라우저 동작하도록' 하라는 규칙
- input에서 property value로 동작하는 코드를 event라고 부름
- 웹브라우저는 웹브라우저 위에서 일어나는 여러 사건 중에 기념할만한 10-20개 정도의 이벤트를 정의하고 있음. 
- 이를 통해 사용자와 상호작용하는 웹사이트를 만들 수 있음.
- event 예시: `onclick`, `onchange`, `onkeydown`


## 1.3. console(콘솔)
- 검사-> console 혹은 elements에서 esc누르면 콘솔 나옴.
- 웹페이지를 대상으로 js가 실행됨



# 2. Javascript를 통해 할 수 있는- 브라우저 제어
- `<body style="background-color:black; color:white;">` <br> 이렇게 바로 할 수 있으나 그럼 항상 이렇게 된다는 문제가 있음.

1) css의 문법(pass)
2) js를 이용해 제어하고자 하는 태그를 선택하는 방법
- ex) `document.querySelector('body')`
- "js selelct css by selectors"라고 검색 가능 
- js는 `''`와`""`가 예민하게 반응하는 것 같음

# 3. js관련 이론(프로그램, 프로그래밍, 프로그래머)
- html: 컴퓨터 언어
- js: 컴퓨터 언어, 컴퓨터 프로그래밍 언어
- 단어의 어원
  + PROGRAM: 순서
  + PROGRAMMING: 순서를 만드는 행위
  + PROGRAMER: 순서를 만드는 사람




# 4. JavaScript 문법
## 4.1 데이터 타입(자료형) - 문자열(string)과 숫자(number)
- 산술연산자 `+`,`-`,`*`,`/`,
- property(`.length`)
```
"hello world".length
--> 11 #공백도 count

"hello world".toUpperCase()
--> 'HELLO WORLD'

"hello world".indexOf('o')
--> 4 #4번째에서 o가 시작된다는 

"helli oworld".indexOf('o')
--> 6 #공백은 count하지 않음..?
```

## 4.2 변수와 대입 연산자
- 예시를 통하여서 
  + `x = 1;`에서 `=`는 대입연산자, `x`는 변수
  + 오른쪽 항의 값을 왼쪽의 변수에 대입한다
  + `3 = 4`는 불가; `3`은 상수이기 때문
- 변수를 쓸때는 `var`이라고 붙여서 쓰기.

## 4.3 조건문
  - 조건에 따라 다른 순서의 기능들이 실행됨.
  - toggle(버튼하나로 왔다갔다하는)


