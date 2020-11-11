---
layout: article
title: HTML basic
key: 100011
tags: HTML Frontend
category: HTML Frontend
date: 2020-11-11 09:36:00 +08:00
modify_date: 2020-11-11 12:30:00 +08:00
picture_frame: shadow
---

**생활코딩 html 수업에서 학습한 내용을 정리한 노트입니다.**  
https://opentutorials.org/course/2039/10932
<!--more-->


# 2. Hypertext, 속성
```{.html}
<h1>오늘의 명언</h1>  
우리 모두는 <strong>자신의 힘</strong>으로 발견한 내용을 가장 쉽게 익힌다.  
(<a target="_blank" href="https://ko.wikipedia.org/wiki/%EB%8F%84%EB%84%90%EB%93%9C_%EC%BB%A4%EB%88%84%EC%8A%A4" title="전설적인 프로그래머">도널드 커누스</a>)  
```

# 3. 태그의 중첩과 목록
```mermaid
<ol>  
  <li>기술소개</li>  
  <li>기본문법</li>  
  <li>하이퍼텍스트와 속성</li>  
  <li>리스트와 태그의 중첩</li>  
</ol>  
<ul>  
  <li>최진혁</li>  
  <li>최유빈</li>  
  <li>한이람</li>  
  <li>한이은</li>  
</ul>  
```
# 4. 문서의 구조
```mermaid
<html>  
<head>  
  <title>HTML - 수업소개</title>  
  <meta charset="utf-8">  
</head>  
<body>  
<h1>HTML</h1>  
<ol>  
  <li>기술소개</li>  
  <li>기본문법</li>  
  <li>하이퍼텍스트와 속성</li>  
  <li>리스트와 태그의 중첩</li>  
</ol>  
 
<h2>선행학습</h2>  
 
</body>  
</html>  
```

# 5. DOCTYPE
```mermaid
<!DOCTYPE html>   
<html>   
<head>  
  <title>HTML - 수업소개</title>  
  <meta charset="utf-8">  
</head>  
<body>  
<h1>HTML</h1>  
<ol>  
  <li>기술소개</li>  
  <li>기본문법</li>  
  <li>하이퍼텍스트와 속성</li>  
  <li>리스트와 태그의 중첩</li>  
</ol>  
 
<h2>선행학습</h2>  
 

</body>  
</html>  
```
본 수업을 효과적으로 수행하기 위해서는 웹애플리케이션에 대한 전반적인 이해가 필요합니다. 이를 위해서 준비된 수업은 아래 링크를 통해서 접근하실 수 있습니다. 

# 6. 웹사이트 만들기

### index.html
```
<!DOCTYPE html>
<html>
<head>
  <title>HTML - 수업소개</title>
  <meta charset="utf-8">
</head>
<body>
<h1><a href="index.html">HTML</a></h1>
<ol>
  <li><a href="1.html">기술소개</a></li>
  <li><a href="2.html">기본문법<a/></li>
  <li><a href="3.html">하이퍼텍스트와 속성</a></li>
  <li><a href="4.html">리스트와 태그의 중첩</a></li>
</ol>
 
<h2>선행학습</h2>
 
</body>
</html>
```
### 1. html
```
<!DOCTYPE html>  
<html>  
<head>  
  <title>HTML - 수업소개</title>  
  <meta charset="utf-8">  
</head>  
<body>  
<h1><a href="index.html">HTML</a></h1>  
<ol>  
  <li><a href="1.html">기술소개</a></li>  
  <li><a href="2.html">기본문법<a/></li>  
  <li><a href="3.html">하이퍼텍스트와 속성</a></li>  
  <li><a href="4.html">리스트와 태그의 중첩</a></li>  
</ol>  
 
<h2>기술소개</h2>   
HTML은 HyperText Markup Language의 약자로서 웹페이지를 만드는 언어입니다.  
</body>  
</html>  
```
# 7. 개발도구

atom (추천 확장기능 emmet)   
sublime text (추천 확장기능 emmet)   
bracket   

# 8. HTML의 변천사와 통계
http://www.martinrinehart.com/frontend-engineering/engineers/html/html-tag-history.html   
https://www.advancedwebranking.com/html/   

# 주요태그
# 1. 단락 - p
```
<html>
    <head><meta charset="utf-8"></head>
    <body>
 
<p>HyperText Markup Language, commonly referred to as HTML, is the standard markup language used to create web pages. Along with CSS, and JavaScript, HTML is a cornerstone technology, used by most websites to create visually engaging webpages, user interfaces for web applications, and user interfaces for many mobile applications.[1] Web browsers can read HTML files and render them into visible or audible web pages. HTML describes the structure of a website semantically along with cues for presentation, making it a markup language, rather than a programming language.</p>
 
<p>HTML elements form the building blocks of all websites. HTML allows images and objects to be embedded and can be used to create interactive forms. It provides a means to create structured documents by denoting structural semantics for text such as headings, paragraphs, lists, links, quotes and other items.</p>
 
<p>The language is written in the form of HTML elements consisting of tags enclosed in angle brackets . Browsers do not display the HTML tags and scripts, but use them to interpret the content of the page.</p>
    </body>
</html>
```
# 2. 줄바꿈 - br
```
<html>
<head><meta charset="utf-8"></head>
<body>
HyperText Markup Language, commonly referred to as HTML, is the standard markup language used to create web pages. Along with CSS, and JavaScript, HTML is a cornerstone technology, used by most websites to create visually engaging webpages, user interfaces for web applications, and user interfaces for many mobile applications.[1] Web browsers can read HTML files and render them into visible or audible web pages. HTML describes the structure of a website semantically along with cues for presentation, making it a markup language, rather than a programming language.<br><br><br>
 
HTML elements form the building blocks of all websites. HTML allows images and objects to be embedded and can be used to create interactive forms. It provides a means to create structured documents by denoting structural semantics for text such as headings, paragraphs, lists, links, quotes and other items.<br><br><br>
 
The language is written in the form of HTML elements consisting of tags enclosed in angle brackets. Browsers do not display the HTML tags and scripts, but use them to interpret the content of the page<br><br><br>
</body>
</html>
```
# 3. 이미지 - img
```
<html>
<body>
    <img src="img.jpg" height="300" alt="산 이미지" title="산 이미지">
</body>
</html>
```
# 4. 표 - table
```
<html>
<head><meta charset="utf-8"></head>
<body>
<table border="2">
    <tr>
        <td>이름</td>     <td>성별</td>   <td>주소</td>
    </tr>
    <tr>
        <td>최진혁</td>  <td>남</td>      <td >청주</td>
    </tr>
    <tr>
        <td>최유빈</td>  <td>여</td>      <td>청주</td>
    </tr>
</table>
</body>
</html>
```
# 5. 입력양식 - form
```
<html>
<head><meta charset="utf-8"></head>
<body>
<table border="2">
    <tr>
        <td>이름</td>     <td>성별</td>   <td>주소</td>
    </tr>
    <tr>
        <td>최진혁</td>  <td>남</td>      <td >청주</td>
    </tr>
    <tr>
        <td>최유빈</td>  <td>여</td>      <td>청주</td>
    </tr>
</table>
</body>
</html>
```
## 5.1. 텍스트 입력
```
<html>
<head>
    <meta charset="utf-8">
</head>
<body>
    <form action="">
        <p>text : <input type="text" name="id" value="default value"></p>
        <p>password : <input type="password" name="pwd" value="default value"></p>
        <p>textarea :
            <textarea cols="50" rows="2">default value</textarea>
        </p>
    </form>
</body>
</html>
```
## 5.2. 선택
```
<html>
    <head>
        <meta charset="utf-8">
    </head>
    <body>
        <form action="http://localhost/color.php">
            <h1>색상</h1>
            <select name="color">
                <option value="red">붉은색</option>
                <option value="black">검은색</option>
                <option value="blue">파란색</option>
            </select>
            <h1>색상2 (다중선택)</h1>
            <select name="color2" multiple>
                <option value="red">붉은색</option>
                <option value="black">검은색</option>
                <option value="blue">파란색</option>
            </select>
            <input type="submit">
        </form>
    </body>
</html>
```
## 5.3. 버튼
```
<html>
<head><meta charset="utf-8"></head>
<body>
    <form action="http://localhost/form.php">
        <input type="text">
        <input type="submit" value="전송">
        <input type="button" value="버튼" onclick="alert('hello world')">
        <input type="reset">
    </form>
</body>
</html>
```
## 5.4. 데이터 전송 - hidden
```
<html>
    <head>
        <meta charset="utf-8">
    </head>
    <body>
        <form action="http://localhost/hidden.php">
            <input type="text" name="id">
            <input type="hidden" name="hide" value="egoing">
            <input type="submit">
        </form>
    </body>
</html>
```
<html>
    <head>
        <meta charset="utf-8">
    </head>
    <body>
        <form action="http://localhost/hidden.php">
            <input type="text" name="id">
            <input type="hidden" name="hide" value="egoing">
            <input type="submit">
        </form>
    </body>
</html>
## 5.5. 컨트롤의 제목 - label
```
<html>
    <head>
        <meta charset="utf-8">
    </head>
    <body>
        <form action="http://localhost/hidden.php">
            <input type="text" name="id">
            <input type="hidden" name="hide" value="egoing">
            <input type="submit">
        </form>
    </body>
</html>
```
<html>
    <head>
        <meta charset="utf-8">
    </head>
    <body>
        <form action="http://localhost/hidden.php">
            <input type="text" name="id">
            <input type="hidden" name="hide" value="egoing">
            <input type="submit">
        </form>
    </body>
</html>
## 5.6. method
```
<html>
    <head>
        <meta charset="utf-8">
    </head>
    <body>
        <form action="http://localhost/method.php" method="post">
            <input type="text" name="id">
            <input type="password" name="pwd">
            <input type="submit">
        </form>
    </body>
</html>
```
<html>
    <head>
        <meta charset="utf-8">
    </head>
    <body>
        <form action="http://localhost/method.php" method="post">
            <input type="text" name="id">
            <input type="password" name="pwd">
            <input type="submit">
        </form>
    </body>
</html>

## 5.7. 파일 업로드
```
<html>
    <head>
        <meta charset="utf-8">
    </head>
    <body>
        <form action="http://localhost/upload.php" method="post" enctype="multipart/form-data">
            <input type="file" name="profile">
            <input type="submit">
        </form>
    </body>
</html>
```
<html>
    <head>
        <meta charset="utf-8">
    </head>
    <body>
        <form action="http://localhost/upload.php" method="post" enctype="multipart/form-data">
            <input type="file" name="profile">
            <input type="submit">
        </form>
    </body>
</html>
# 6. 정보로서의 HTML
본 수업의 하위에서는 HTML을 보다 좋은 정보로 만들기 위한 방법들과 생각할 문제들을 다루고 있습니다.

## 6.1. 글꼴 - font (퇴출됨)
```
```
## 6.2. meta
```
```
## 6.3. 의미론적 태그
```
```
목적
문서의 정보를 보다 잘 표현하기 위해서는 의미에 맞는 태그를 잘 사용해야 합니다. 특히 HTML5에서는 웹페이지에서 통상 많이 사용하는 구조에 의미를 분명히 부여하기 위해서 의미론적 태그(semantic element)를 새롭게 정의해서 제공하고 있습니다. 그 목록은 아래와 같습니다. 

article	본문
aside	광고와 같이 페이지의 내용과는 관계가 적은 내용들
details	기본적으로 표시되지 화면에 표시되지 않는 정보들을 정의
figure	삽화나 다이어그램과 같은 부가적인 요소를 정의
footer	화면의 하단에 위치하는 사이트나 문서의 전체적인 정보를 정의
header	화면의 상단에 위치하는 사이트나 문서의 전체적인 정보를 정의
main	문서에서 가장 중심이 되는 컨텐츠를 정의
mark	참조나 하이라이트 표시를 필요로 하는 문자를 정의
nav	문서의 네비게이션 항목을 정의
section	문서의 구획들을 정의 (참고)
time	시간을 정의

## 6.4. 검색엔진 최적화
http://static.googleusercontent.com/media/www.google.com/ko//intl/ko/webmasters/docs/search-engine-optimization-starter-guide-ko.pdf
```
```
# 7. 웹개발자도구
웹개발자도구는 웹 개발을 하는데 필요한 여러가지 기능을 모아둔 도구들로 웹브라우저별로 비슷한 기능의 도구를 제공하고 있습니다. 여기서는 HTML 개발과 관련된 부분에 초점을 맞춰서 크롬 개발자 도구를 살펴봅니다. 아래 링크는 크롬 개발자 도구에 대한 자세한 수업으로 연결됩니다. 

https://opentutorials.org/module/306/2865
```
```
# 8. 모바일 지원 (viewport)
```
<!DOCTYPE html>
<html>
<head>
  <title>HTML - 수업소개</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
<h1><a href="index.html">HTML</a></h1>
<ol>
  <li><a href="1.html">기술소개</a></li>
  <li><a href="2.html">기본문법<a/></li>
  <li><a href="3.html">하이퍼텍스트와 속성</a></li>
  <li><a href="4.html">리스트와 태그의 중첩</a></li>
</ol>
 
<h2>선행학습</h2>
 
본 수업을 효과적으로 수행하기 위해서는 웹애플리케이션에 대한 전반적인 이해가 필요합니다. 이를 위해서 준비된 수업은 아래 링크를 통해서 접근하실 수 있습니다.
</body>
</html>
```
<!DOCTYPE html>
<html>
<head>
  <title>HTML - 수업소개</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
<h1><a href="index.html">HTML</a></h1>
<ol>
  <li><a href="1.html">기술소개</a></li>
  <li><a href="2.html">기본문법<a/></li>
  <li><a href="3.html">하이퍼텍스트와 속성</a></li>
  <li><a href="4.html">리스트와 태그의 중첩</a></li>
</ol>
 
<h2>선행학습</h2>
 
본 수업을 효과적으로 수행하기 위해서는 웹애플리케이션에 대한 전반적인 이해가 필요합니다. 이를 위해서 준비된 수업은 아래 링크를 통해서 접근하실 수 있습니다.
</body>
</html>

# 9. 외부문서삽입 - iframe
목적
 웹페이지에 다른 웹페이지를 삽입하는 방법인 아이프래임은 참 편리하면서도 위험한 방법입니다. 왜냐면 신뢰할 수 없는 사이트에서 악성코드 같은 것을 포함하고 있다면 삽입된 외부소스에서 악성코드가 실행될 수 있기 때문이죠. 이런 문제를 해소하기 위해서 HTML의 최신 버전인 HTML5에서는 샌드박스라는 것을 도입했습니다. 아이프래임으로 삽입된 웹페이지에서 자바스크립트 등이 실행되지 않도록 하는 방법인데요. 아이패래임이 무엇인지, 사용법, 그리고 보안을 개선할 수 있는 새로운 방법을 소개합니다.

# HTML5
현시점에서 최신 웹 기술인 HTML에서 추가된 기능들을 알아봅니다. 


# 1. 비디오 - video
목적
웹페이지에 비디오를 삽입하기 위한 태그인 video의 사용법을 알아봅니다.

샘플 영상 파일
http://techslides.com/sample-webm-ogg-and-mp4-video-files-for-html5​

# 2. Can I use
목적
새롭게 도입된 기술은 오래된 웹브라우저에서 동작하지 않습니다. 결국 얼마나 많은 웹브라우저가 이 기술을 사용할 수 있는가에 따라서 신기술의 도입 여부를 결정해야 합니다. Can I use는 이런 결정을 할 때 도움을 주는 서비스입니다. 

# 3. HTML5의 입력양식
input types: 
color  
date 
datetime 
datetime-local  
email 
month 
number
range
search
tel
time
url
week

## 3.1. HTML5 입력양식의 속성들
```
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
    </head>
    <body>
        <form action="login.php" autocomplete="on">
            <input type="text" name="id" placeholder="id를 입력해주세요." autofocus>
            <input type="password" name="password" autocomplete="off" placeholder="비밀번호를 입력해주세요.">
            <input type="submit">
        </form>
    </body>
</html>
```
## 3.2. HTML5 입력 값 체크
```
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
    </head>
    <body>
        <form action="register.php">
            <input type="text" name="id" placeholder="아이디를 입력" required pattern="[a-zA-Z].+[0-9]">
            <input type="email" name="email" placeholder="이메일 입력">
            <input type="submit">
        </form>
    </body>
</html>
```
https://opentutorials.org/course/909/5142
