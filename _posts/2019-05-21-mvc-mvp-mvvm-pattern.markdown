---
layout: post
title:  "MVC, MVP, MVVM 비교"
subtitle:   "pattern"
categories: development
tags: pattern
header-img: img/-logo.png
---


MVC, MVP, MVVM 패턴에 대해 알아보자

### MVC (Model + View + Controller)

1. Controller로 사용자의 입력이 들어오면
2. Controller는 Model에게 데이터를 요청
3. Model은 해당 데이터를 보여줄 View를 선택해서 화면에 보여주게 됩니다.

> MVC는 단점이 있습니다. View와 Model이 서로 의존적이라는 점입니다.

<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<!-- posts -->
<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-1778623499634593"
     data-ad-slot="2464814109"
     data-ad-format="auto"
     data-full-width-responsive="true"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

### MVP (Model + View + Presenter)

1. View로 사용자의 입력이 들어오면
2. View는 Presenter에 작업 요청
3. Presenter에서 필요한 데이터를 Model에 요청
4. Model은 Presenter에 필요한 데이터를 응답
5. Presenter는 View에 데이터를 응답
6. View는 Presenter로부터 받은 데이터로 화면에 보여주게 됩니다.

> MVP도 단점이 있습니다. View와 Model은 의존성이 없는 대신 View와 Presenter가 1:1로 강한 의존성을 가지게 됩니다.

### MVVM (Model + View + ViewModel)

1. View에 입력이 들어오면 Command 패턴으로 ViewModel에 명령
2. ViewModel은 필요한 데이터를 Model에 요청
3. Model은 ViewModel에 필요한 데이터를 응답
4. ViewModel은 응답 받은 데이터를 가공해서 저장
5. View는 ViewModel과의 Data Binding으로 인해 갱신

### Command 패턴이란?
> 실행될 기능을 캡슐화함으로써 주어진 여러 기능을 실행할 수 있는 재사용성이 높은 클래스를 설계하는 패턴
