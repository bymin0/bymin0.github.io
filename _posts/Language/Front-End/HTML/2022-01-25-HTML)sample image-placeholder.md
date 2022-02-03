---
title: HTML)Sample image-placeholder
date: 2022-01-25 23:55:55 +0900
categories: [Language, Front-End]
tags: [HTML, img]
---

# img tag
- 이미지 삽입 태그
- 사용법<br>

```html
<img src="이미지주소" alt="src오류시 나오는 내용">
```

## ▶ src
- 넷상의 이미지 주소를 가져올 때

```html
<!-- 이미지주소 변경되면 에러! -->
<img src="https://images.pexels.com/photos/2449543/pexels-photo-2449543.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260"> 
```

- 결과
 - ![error](https://images.pexels.com/photos/2449543/pexels-photo-2449543.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260)<br>
Aaron Burden 님의 사진, 출처: [Pexels](https://www.pexels.com/ko-kr/photo/2449543/)

- 컴퓨터에 저장되어 있는 이미지를 가져올 때

```html
<!-- 경로 설정 주의! -->
<img src="../../../assets/imgs/html_01_00.jpg">
```

- 결과
  - <img src="../../../assets/imgs/html_01_00.jpg"><br>
Bekir Donmez 님의 사진, 출처: [Pexels](https://www.pexels.com/ko-kr/photo/9995685/)
## ▶ alt(이미지 오류)
- ```html
  <img src="" alt="이미지 없다">
  ```

- ![이미지 없다](../../../assets/imgs/html_01_010.png)

# 샘플 이미지 사용하기
- https://via.placeholder.com
- 주로 임시로 이미지의 크기, 위치 등을 설정할 때 사용

## 사용방법

- ```html
  <img src="https://via.placeholder.com/200" alt="200x200">
  <!-- 200 x 200 샘플 이미지 생성 -->
  ```

- 결과 : <br>
  <img src="https://via.placeholder.com/200" alt="200x200">

## 가로 세로 다른 크기 설정
- ```html
  <img src="https://via.placeholder.com/200x300" alt="200x300">
  ```

  - 가로x세로
- 결과 : <br>
  <img src="https://via.placeholder.com/200x300" alt="200x300">

## 확장자 지정(png, jpg, jpeg, gif)
- ```html
  <!-- jpg -->
  <img src="https://via.placeholder.com/200x300.jpg">
  <!-- png -->
  <img src="https://via.placeholder.com/200x300.png">
  <!-- gif -->
  <img src="https://via.placeholder.com/200x300.gif">
  ```

- 결과 : <br>
  ![02](../../../assets/imgs/html_01_02.png)
## 이미지 내부 텍스트 입력
- ```html
  <img src="https://via.placeholder.com/200?text=this+is+test">
  ```

- 띄어쓰기 부호 : +
  - hello,+world \>> hello, world

- 결과 : <br>
  <img src="https://via.placeholder.com/200?text=this+is+test" alt="error">

## 이미지 색상, 글자 색상 지정
- ```html
  <img src="https://via.placeholder.com/200/000000/ffffff?text=img+color,+txt+color">
  ```

  - placeholder주소/이미지크기/이미지색상/폰트색상?텍스트
  - 색상 : hex color code 사용
- 결과 : <br>
  <img src="https://via.placeholder.com/300x100/000000/ffffff?text=img+color,+txt+color">
