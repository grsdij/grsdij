## Post 헤더

---
title: 
author: arte
categories: essay
layout: post
---

## 각주

각주 위치[^1]

[^1]: 각주 내용

## 링크

[연결할 주소](https://www.google.com)

## 요약문 제외

<!-- excerpt_separator -->

## figure 사용

<figure>
  <img alt="" src="" />
  <figcaption>
    캡션 내용 <a href="">링크</a> 캡션 내용 끝.
  </figcaption>
</figure>

## 구분선

<hr>

## 유튜브 삽입

<iframe width="929" height="480" src="https://www.youtube.com/embed/zKij45MIuZE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## 이미지 삽입

<img data-action="zoom" src='{{ "/assets/images/test.jpeg" | relative_url }}' alt="TEST">

![TEST]({{"/assets/images/test.jpeg"| relative_url}})

## 폰트 관련

@font-face {
  font-family: 'Pretendard Varialbe';
  font-weight: 45 920;
  font-style: normal;
  font-display: block;
  src: local('Pretendard'), url('#{$asset_url}/fonts/PretendardVariable.woff2') format('woff2-variations');
}

@font-face {
  font-family: 'SpoqaHanSansNeo-Light';
  src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_2108@1.1/SpoqaHanSansNeo-Light.woff') format('woff');
  font-weight: normal;
  font-style: normal;
}

@font-face {
  font-family: 'IBMPlexSansKR-Light';
  src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_20-07@1.0/IBMPlexSansKR-Light.woff') format('woff');
  font-weight: normal;
  font-style: normal;
}

@font-face {
  font-family: 'MinSans-Light';
  src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_2201-2@1.0/MinSans-Light.woff') format('woff');
  font-weight: normal;
  font-style: normal;
}
