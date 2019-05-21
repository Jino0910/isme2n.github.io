---
layout: post
title:  "cocoapods, carthage 비교"
subtitle:   "etc"
categories: development
tags: etc cocoapods carthage
header-img: img/ios-logo.png
---


cocoapods, carthage에 대해 알아보자

## cocoapods

**장점**
- 일반적으로 많이 쓰인다
- 안정성이 있다
- 모든 설정이 자동화 되어 있다

**단점**
- 오픈소스를 많이 사용한다면 컴파일이 느려진다
- pod update시 pods프로젝트와 내프로젝트에 모두 영향을 끼친다
- ruby로 만들어 져있어 ruby버전과 패키지 관리자(gem, bundle)를 신경써야한다

## carthage

**장점**
- 미리 빌드후 생성되는 framework를 프로젝트에 사용하기 때문에 매번 라이브러리를 빌드해야 하는 cocoapods 보다 빌드 시간이 단축된다.

**단점**
- 커뮤니티가 작다


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
