---
layout: post
title:  "[웹폰트]웹폰트의 장점과 문제점"
subtitle:   "웹폰트의 장점과 문제점"
categories: devlog
tags: web
comments: true

---

웹폰트를 사용하다가 문제가 생겨서 보류하기로 했다. 여러가지 우회법들이 있지만, 별도의 노력이 많이 든다. 결과적으론 `Lato`폰트로 내 욕심과 현실 사이에서 합의를 봤다.

## 웹폰트의 장점

---

웹 폰트의 가장 큰 장점은 아래와 같다.

- 모든 플랫폼과 브라우저에서 동일한 경험을 제공한다.

또한 아마 요즘엔 이런일이 거의 없겠지만, 이미지로 폰트를 대신했다면 아래와 같은 큰 장점들이 있다. (가능하다면 그냥 프론트엔드 개발자를 고용하자.)

- 검색엔진 최적화
- 해상도 변화에 유동적
- 이미지를 줄여 접근성과 경험 향상
- 유지보수와 관리가 용이하다.

이런 장점에도 불구하고 웹폰트의 사용을 고려하게 만드는 문제점들이 몇가지 있다.

<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
     style="display:block; text-align:center;"
     data-ad-format="fluid"
     data-ad-layout="in-article"
     data-ad-client="ca-pub-1778623499634593"
     data-ad-slot="3873336698"></ins>
<script>
     (adsbygoogle = window.adsbygoogle || []).push({});
</script>

## 웹폰트의 문제

---

### 용량

한글 웹폰트는 영문 웹폰트에비해 용량이 크다. 한글폰트는 완성형이기때문에 경량형으로 잡아도 최소 2,300자 정도이다. 경량화가 잘 된 한글폰트의 경우 용량으로 치면 약300KB정도 된다. 영문의 경우 100KB가 되지 않는 것에 비해 꽤 차이가 난다. 압축률이 높은 woff2로 표현된 `spoqa han sans`는 300KB 정도인 반면, 영문폰트인 `Lato`는 13KB에 불과하다. 폰트를 메모리에 저장한다고 해도, 블로그의 특성상 외부유입이 많다고 보았을 때 웹폰트로 초기 로딩에 소요되는 시간이 길어지는 건 좋지 않다.

### 확장성

이건 나의 경우는 별로 신경쓰지 않은 사안이다. 앞서 이야기한 것처럼 용량문제로 한글 웹폰트는 경량화를 대부분 거치는데, 이 과정에서 자주쓰지 않는 글자들이 빠지게 된다. 대부분 커버가 되겠지만, 만약 다양한 사람들이 활동하는 커뮤니티 사이트를 운영한다면 웹폰트는 사용하지 않는것이 좋다.  

### FOIT : Flash Of Invisible Text

글자가 보이지 않다가 보이는 현상을 이야기한다. FOIT 현상은 웹폰트가 다운로드 되기 전까지 글자를 표시하지 않고 다운로드가 완료되면 표시되기 때문에 발생한다. 특히 한국어 웹폰트는 용량이 커서, 꽤 오랜시간 글자가 나오지 않는 경우가 종종 발생한다. 이런 경우 사용자들의 경험에 부정적 영향을 미칠 수 있다.

### FOUT : Flash Of Unstyled Text

글꼴이 깜빡이면서 바뀌는 현상이다. 글자가 기본 글꼴로 표현되었다가 웹폰트 다운로드가 완료되면 폰트가 바뀌면서 깜빡이게 된다. 이 현상은 간혹 레이아웃에 영향을 미치는 경우도 있다.

## 마치며
---

웹폰트는 문제도 많지만 장점도 많다.
