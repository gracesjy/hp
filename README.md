---
layout: home
title: Raymond Development areas of interest
permalink: /
---

Raymond 개발 관심 분야 !

## Big Data Analysis Enabler(BDAE) for Oracle Database
#1. 개요
이것은 홀로 기획하고, 개발한 개인 작품입니다.<br>
Oracle R Enterprise 라는 처음 접했을 때

#2. 활용

<br>

이것은 Oracle R Enterprise 를 고객사의 분석가들과 함께 검토하면서 시작된 것으로 다음의 문제점을 보완하기 위해서 만들기 시작했습니다.

    1. R 보다, Python 이 되었으면 한다.
    2. 많은 알고리즘보다, 개발한 알고리즘을 쉽게 넣고 커스터마이징 할 수 있었으면 한다.
    3. 간단하게 알고리즘을 생성,저장,변경 등을 할 수 있는 GUI 가 제공되었으면 한다.
    4. 분석 이외에 Oracle Database 의 전처리를 최대한 손쉽게 할 수 있었으면 한다.
    5. 빠른 성능을 위한 개선 사항이 반영 될 수 있었으면 한다.

초창기 만들 때에는 Python 엔진을 직접 빌드해야 했었고, 다양한 Python 버전에 대응하기 힘들었지만 지금은 Anaconda 를 이용하여 이러한 작업들이 손쉬워졌으며 R 까지 설치가 용이해졌습니다.<br>

Oracle In-Database 기술을 사용하기 때문에 일반적이 어플리케이션이 아니며 Shared Library(.so) 형태를 띄고 있고, Oracle Database 가 필요 시 자동으로 실행시켜 주는 방식입니다.<br>

구성은 Shared Library (C/C++), Oracle PL/SQL, Function, Type, View 등으로 구성되어 있으며 Embedded SQL 을 위한 별도의 테이블 함수를 제공합니다.


## OPC-UA with prosys SDK

This is an implementation of OPC-UA, an international standard protocol for IOT.  
It is no different from making and delivering it alone. Originally, open source from the Eclipse Milo project was used, 
but delivery of this open source was difficult due to insufficient implementation of important Alarm and Event parts.
So I implemented it using prosys.   PLC communication is also very clean and verified because it uses commercial products.  
For reference, it is implemented in JAVA.

## More

Please Refer to side menu for my personal solutions.
