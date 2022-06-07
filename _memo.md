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

otf to woff2: https://kombu.kanejaku.org/
일반: Pretendard
눈누: IBMPlexSansKR, SpoqaHanSansNeo, MinSans

fallback: -apple-system, BlinkMacSystemFont, system-ui, Roboto, 'Helvetica Neue', 'Segoe UI', 'Apple SD Gothic Neo', 'Noto Sans KR', 'Malgun Gothic', sans-serif
// "Times New Roman", serif

1. @font-face + variable 지정

in _font.scss
@font-face {
  font-family: 'name';
  src: url('url') format('woff');
  or src: local('name'), url('#{$asset_url}/fonts/name.woff2') format('woff2-variations');
  font-weight: normal;
  font-style: normal;
}

in _variables.scss
$font-family: "name";

2. import in variable
@import url('https://cdn.jsdelivr.net/gh/orioncactus/pretendard/dist/web/static/pretendard.css');
$font-family: Pretendard;

3. Adobe fonts

in default.html's <head>
<script>
  (function(d) {
    var config = {
      kitId: 'crv1tlb',
      scriptTimeout: 3000,
      async: true
    },
    h=d.documentElement,t=setTimeout(function(){h.className=h.className.replace(/\bwf-loading\b/g,"")+" wf-inactive";},config.scriptTimeout),tk=d.createElement("script"),f=false,s=d.getElementsByTagName("script")[0],a;h.className+=" wf-loading";tk.src='https://use.typekit.net/'+config.kitId+'.js';tk.async=true;tk.onload=tk.onreadystatechange=function(){a=this.readyState;if(f||a&&a!="complete"&&a!="loaded")return;f=true;clearTimeout(t);try{Typekit.load(config)}catch(e){}};s.parentNode.insertBefore(tk,s)
  })(document);
</script>

in _variables.scss
$font-family: "name";

in _fonts.scss
@font-face {
  font-family: "sandoll-jebi2", sans-serif;
  font-weight: 300;
  font-style: block;
}