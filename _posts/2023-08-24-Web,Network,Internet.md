---
title: (네트워크) Web, Network, Internet 기초 개념 정리
author: Jake
date: 2023-08-24 18:00:00 +0900
categories: [Network, Basic]
tags: [Network, Web, Internet]
pin: true
math: true
mermaid: true
image:
#  path: /commons/devices-mockup.png
#  lqip: data:image/webp;base64,UklGRpoAAABXRUJQVlA4WAoAAAAQAAAADwAABwAAQUxQSDIAAAARL0AmbZurmr57yyIiqE8oiG0bejIYEQTgqiDA9vqnsUSI6H+oAERp2HZ65qP/VIAWAFZQOCBCAAAA8AEAnQEqEAAIAAVAfCWkAALp8sF8rgRgAP7o9FDvMCkMde9PK7euH5M1m6VWoDXf2FkP3BqV0ZYbO6NA/VFIAAAA
#  alt: Responsive rendering of Chirpy theme on multiple devices.
---

# 요점 정리

<aside>
💡 웹은 인터넷을 통해 연결된 컴퓨터 네트워크 상에서 정보를 공유하고 표시하는 방법이다. 즉, 여러 개의 네트워크가 모여 인터넷이 형성되고 인터넷 서비스 중 하나가 웹이다.

</aside>

## 1. 웹(Web)이란?
### 1) 웹의 정의
- World Wide Web 줄여서 WWW 또는 웹이라고 함.
- 웹은 팀 버너스 리박사가 고안한 시스템으로 멀리 떨어져 있는 동료들 끼리 지식을 공유하기 위해 만듬.
- 웹은 인터넷에서 운영되는 서비스 중 하나로 웹과 인터넷은 다른 개념이다.

### 2) 웹의 특징
- 인터넷상의 정보를 하이퍼텍스트 방식과 멀티미디어 환경에서 검색할 수 있게 해주는 정보 검색 시스템이다.
- HTTP 프로토콜을 사용하며, HTML 문서를 연결하여 다양한 콘텐츠를 제공한다.
- 많은 사람들이 정보를 쉽게 공유하고 접근할 수 있도록 하는 것을 목적으로 한다.

### 3) 웹의 구조
웹은 사용하기 위해 클릭하는 웹 브라우저와 웹페이지의 요청을 응답하는 웹 서버로 나뉜다. 여기서 웹 브라우저는 클라이언트라고 불리며 주로 인터넷을 사용하는 사람들을 의미하며 웹 서버는 서버로 불린다.

![Client-Sever](https://github.com/Uk-jake/ModifyReadme/assets/100981076/47a9f2c6-c0f0-437f-987a-c983972a00bb)

- 클라이언트는 서버에게 요청을 하고 서버는 클라이언트의 요청에 알맞는 응답을 제공한다.

## 2. 네트워크(Network)란?
### 1) 네트워크의 정의
- Net + Work의 합성어로써 컴퓨터들이 통신 기술을 이용하여 그물망처럼 연결된 통신 이용 형태를 의미한다.
- 노드들이 데이터를 공유할 수 있게 하는 디지털 전기통신망.
  - 노드란 네트워크에 속한 컴퓨터 또는 통신 장비를 뜻한다.
- 각종 통신 장비들이 서로 연결되어 데이터를 교환하며, 정보를 주고 받는 통신망이다.

### 2) 네트워크의 종류
![Network](https://github.com/Uk-jake/ModifyReadme/assets/100981076/e7305c8b-a6cd-431c-b25a-45e3312d5d67)
)

- PAN(Personal Area Network) : 가장 작은 규모의 네트워크, 개인 네트워크
- LAN(Local Area Network) : 근거리 영역 네트워크
- MAN(Metropolitan Area Network) : 대도시 영역 네트워크
- WAN(Wide Area Network) : 광대역 네트워크

### 3) 네트워크 통신 방식
- 유니 캐스트 : 특정 대상이랑 1:1 통신
- 멀티 캐스트 : 특정 다수와 1:N 으로 통신
- 브로드 캐스트 : 네트워크에 있는 모든 대상과 통신

### 4) 네트워크의 장단점
### 장점
- 네트워크 데이터 통신을 통한 방대한 자료를 공유할 수 있음.
- 사진, 음악, 영상 등의 디지털 미디어를 볼 수 있음.
- 프로세스 분배를 통한 성능 향상

### 단점
- 바이러스나, 악성코드로 인한 해킹으로 개정정보 유출 피해, 보안상의 문제
- 데이터 변조 가능

## 3. 인터넷(Internet)이란?
### 1) 인터넷의 개념
- 여러 통신망을 하나로 연결한다는 의미 ‘인터 네트워크’라는 말에서 시작되었음.
- 전 세계 컴퓨터들을 하나로 연결하는 거대한 컴퓨터 통신망을 의미.
### 2) 인터넷의 구성
- 위에서 언급한 네트워크가 전 세계적으로 수없이 많이 모여서 이루어진 일종의 컴퓨터 네트워크 시스템이다.
- 즉 여러 네트워크가 모여 인터넷이 된 것이다.
### 3) 인터넷의 특징
- 서로 동시에 참여할 수 있는 쌍방향 통신을 제공
- 시간과 장소를 제약받지 않고 언제든지 사용 가능
- 익명성 제공
