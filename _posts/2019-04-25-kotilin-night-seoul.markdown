---
layout: post
title:  "Kotlin Night 서울"
subtitle:   "Kotlin"
categories: development
tags: Kotlin
---

Kotlin Night 서울 참석 후기입니다.

일시 : 2019년 4월 8일(월) 18:00-22:00
장소 : 소노펠리체 컨벤션 (삼성역)

## 인공지능이 프로그래머를 대체할까? by 김상균
---

> 나는 무엇을 하고 있을까? 구글검색을 통해 프로그래머가 인공지능으로 대체 될까? 라는 주제의 직업검색도가 상대적으로 높다.

### Question

- AI가 내 직업을 대체하면, 나는 무엇을 해서 돈을 벌까?
- AI가 대체하지 못하는 직업/학과가 무엇인가요?

### 설문링크(#kotilin)
<https://www.sli.do/>

## 이펙티브 자바와 코틀린 by 전경주
---

> Effective Java는 효율적이고 잘 설계된 Java 프로그램을 구현하기 위한 지침들을 소개하는 책입니다. Kotlin에서는 이 지침들이 잘 적용될 수 있는 설계를 갖추고 있는데요, Kotlin Reference 문서에서는 설명을 뒷받침하기 위해 이 책을 인용하기도 합니다. 세션에서는 "이펙티브 자바" 책의 규칙들을 짚어가면서, Kotlin에 어떻게 반영되었는지, 혹은 어떻게 적용될수 있는지에 대해 공유합니다.

- Kotlin은 Java base로 호환성을 생각하며 만들어졌다
- 상속보다는 컴포지션을 사용 (새로운클래스를 만들고 기존 클래스를 필드로 사용, delegate, protocol, generic을 이용)

## 자바 개발자 관점의 - 왜 코틀린인가? by 강현식(cj848@hanmail.net)
---

> 자바 개발자들이 자바를 사용하면서 불편함을 느꼈던 부분을 자바 예제 코드와 코틀린 예제 코드를 통해 비교하고 장점에 대해서 소개하며 왜 자바 개발자가 코틀린으로 프로젝트를 바꿔야 하는지에 대한 이유를 보여줄 예정입니다.

- kakaopay Firm Banking gateway
- 2017년 5월 Google I/O에서 Google 공식 Android 언어로 지정
- JDK 6 이상부터 지원
- NullPointerException(Kotlin에선 거의 불가)
- 옵셔널
- const: static
- ?: true 일경우만 pass
- it > this와 유사
- 확장함수(extension functions), operater 노랑색으로 표현되는 함수들로 언어에서 자동으로 만들어줌
- 타입에 ?가 붙으면 null이 가능 없으면 null 불가능(var check: String?), (val check: String)

## Kotlin을 활용한 우아한 코드 만들기 by 이수호
---

>  FLO 에 실제 적용된 Kotlin 코드를 예제로 high order function, extension function, function literals with receivers, DSL 등을 활용하여 코드를 우아하게 만들기 위한 방법에 대해 소개합니다.

- 간결성

## Kotlin + AWS Lambda와 API Gateway by 허재위
---

> Kotlin과 AWS SAM(서버리스 애플리케이션 모델)을 이용하여 간단한 API를 만들고 배포합니다. 빌드하고 배포하는 스크립트 역시 Kotlin(Gradle + Kotlin DSL)으로 작성해봅니다.

- SAM (serverless application model)을(cli) 이용해 aws lambda, gateway api
- build script 역시 kotlin DSL
- CLI 앱을 통해 /greeting -> lambda function
- 라이브 코딩
- gralde "aws.sam"
- 반복 작업들을 gradle plugin으로 만들어서 처리하도록 plugin을 생성
- rxjava
- client와 server가 공통으로 model을 사용할 수 있음

## Github (Daniel Hwang gnawhleinad@github.com)
---

> GitHub Enterprise Hooks (push한 작업에 동작)

- 본인이 스스로 우선순위를 세우고 동료와 공유
- 굉장히 투명하게 일함
- 엔지니어 67%가 해외 각지에서 일하고 있음
- 비동시적인 업무환경

## Java를 베이스로 만든 Kotlin의 기능
---

- 데이터 클래스
- null 안정성
- 델리게이트
- 클래스 익스텐션
- Companion 객체와 스마트 캐스팅
- 컬렉션 함수
- 컨트롤 제어 구조
- 오퍼레이터 오버로딩
