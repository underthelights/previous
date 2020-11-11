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
```mermaid
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
 
본 수업을 효과적으로 수행하기 위해서는 웹애플리케이션에 대한 전반적인 이해가 필요합니다. 이를 위해서 준비된 수업은 아래 링크를 통해서 접근하실 수 있습니다. 
</body>
</html>

# 6. 웹사이트 만들기

### index.html

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

### 1. html
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

# 7. 개발도구

atom (추천 확장기능 emmet)
sublime text (추천 확장기능 emmet)
bracket

# 8. HTML의 변천사와 통계
http://www.martinrinehart.com/frontend-engineering/engineers/html/html-tag-history.html
https://www.advancedwebranking.com/html/

# 주요태그
# 1. 단락 - p
# 2. 줄바꿈 - br
# 3. 이미지 - img
# 4. 표 - table
# 5. 입력양식 - form
## 5.1. 텍스트 입력
## 5.2. 선택
## 5.3. 버튼
## 5.4. 데이터 전송 - hidden
## 5.5. 컨트롤의 제목 - label
## 5.6. method
## 5.7. 파일 업로드
# 6. 정보로서의 HTML
## 6.1. 글꼴 - font (퇴출됨)
## 6.2. meta
## 6.3. 의미론적 태그
## 6.4. 검색엔진 최적화
# 7. 웹개발자도구
# 8. 모바일 지원 (viewport)
# 9. 외부문서삽입 - iframe

# HTML5
# 1. 비디오 - video
# 2. Can I use
# 3. HTML5의 입력양식
## 3.1. HTML5 입력양식의 속성들
## 3.2. HTML5 입력 값 체크
