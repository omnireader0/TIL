# HTML(Hyper Text Markup Language)

웹 페이지나 웹 애플리케이션을 만드는 표준 마크업 언어

웹은 모든 os에서 동작하고, 웹 페이지의 소스코드는 누구나 볼 수 있으며 저작권이 없는 순수한 공공재이다.

## 참고

https://www.w3.org/

W3C라는 표준화기구에서 웹의 표준 논의함

https://www.w3schools.com/tags/tag_hn.asp

태그 정의 정리됨

https://www.advancedwebranking.com/seo/html-study/

자주 쓰는 태그 빈도 

## 좋은 공부법

예제와 정의가 있다. 예제를 먼저 보고 공부하는 것이 좋다.

경험을 통해서 추론하는 것은 자기 힘으로 알아내는 것이고, 이론을 통해서 배우는 것은 남의 도움을 받는 것입니다.

## 문법

### 태그

- 강조 표시

```
<strong> ~~ </strong>
```

- 밑줄

~~~
 <u>web</u>
~~~

- 글씨 크기

h1 ~h6까지 있으며,

`<h1>` defines the most important heading. `<h6>` defines the least important heading.

~~~
<h1> </h1>
~~~

- 줄바꿈  `<br> vs <p>`

~~~
<br>
단독으로 쓰이며, 줄바꿈 코드다.
무엇인가를 설명하지 않는 태그들은 감쌀 컨텐츠가 없어서 단독으로 쓴다. img, input, hr, meta 등

<p> ~ </p>
단락 표현
CSS 이용하면 단락의 간격 조정 가능
<p style="margin-top:45px;"> : p태그 위쪽에 45px 만큼의 여백 생김
~~~

### 태그 :: 속성

- 이미지 넣기

img 태그에 src 붙이기

src가 속성임

저작권 구속받지 않는 이미지 -> public domain image 라고 검색 , uplash.com 검색

~~~
<img src="https://s3-ap-northeast-2.amazonaws.com/opentutorials-user-file/module/3135/7648.png">
~~~

이미지의 크기가 원하는 것과 다르다면 -> html img size attribute

width 속성을 이용해 숫자나 % 로 조정

~~~
<img src="https://s3-ap-northeast-2.amazonaws.com/opentutorials-user-file/module/3135/7648.png" width="100%">
~~~

### 태그 :: 목차

p 태그가 a 태그의 부모, a 태그가 p 태그의 자식

~~~
<p>
    <a href="https://opentutorials.org">opentutorials</a>
</p>
~~~

- 목차

`<li> ~ </li>`

~~~
<li>1. HTML</li>
~~~

- 목차 사이에 경계 만들기

`<ul> ~ </ul>`

~~~
<ul>
  <li>1. HTML</li>
  <li>2. CSS</li>
  <li>3. JavaScript</li>
</ul>
<ul>
  <li>egoing</li>
  <li>k8805</li>
  <li>sorialgi</li>
</ul>
~~~

- 목차 li에 순서 부여

`<ol> ~ </ol>`

~~~
<ol>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ol>
~~~







![image](https://user-images.githubusercontent.com/93963499/148503325-b21d6911-0239-402b-95ca-278202592b35.png)

### 웹 페이지 

- 탭 제목 바꾸기

`<title> ~ </title>`

제목 지정

검색엔진이 웹 페이지 분석할 때 가장 중요하게 생각하는 태그 

~~~
<title>WEB1 - html</title>
~~~

- 영어가 아닌 문자 사용

UTF-8 방식을 사용

영어가 아닌 문자가 깨지는 이유는 웹 페이지가 저장된 문자 표현 방식과 웹 브라우저가 웹 페이지를 해석하는 방식이 다를 때 생김

따라서 웹 브라우저에게 웹페이지는 UTF-8로 작성되어 있으므로 UTF-8로 열어줘야 함을 명시해주기

~~~
<title>WEB1 - html</title>
<meta charset="utf-8">
~~~

- 제목과 본문 나누기

`<head> ~ </head> ` 본문 설명

`<body> ~ </body>` 본문

`<!doctype html>` html 로 만들었다는 표시  -> 바로 밑에 `html> ~ </html>`  같이 표시

```
<!doctype html>
<html>
<head>
  <title>WEB1 - html</title>
  <meta charset="utf-8">
</head>
<body>
  <ol>
    <li>HTML</li>
  </ol>
  <h1>HTML</h1>
  <p>Hypertext Markup Language (HTML) is the standard markup language for HTML elements are delineated by tags, written using angle brackets.
  </p>
</body>
</html>
```

### 태그 :: 링크

- 링크

a는 anchor의 약자이고,  href는 **H**yperText **Ref**erence의 약자

`target="_blank"` 링크를 클릭했을 때, 새창에서 페이지가 열리게 되는 속성

`title` 이 링크가 어떤 내용을 담고 있는지 

~~~
<a href="https://www.w3.org/TR/html5/" target="_blank" title="html5 specification">Hypertext Markup Language (HTML)</a>
~~~



https://opentutorials.org/course/3084/18431 다시하기..



### Reference

- 생활코딩