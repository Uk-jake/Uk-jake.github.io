---
title: (Spring)Spring? SpringBoot? 둘이 뭐가 다른거야?
author: Jake
date: 2023-10-08 14:00:00 +0900
categories: [Spring, Spring_Basic]
tags: [Java, Backend, Spring, SpringBoot]
pin: true
math: true
mermaid: true
image:
#  path: jetbrains://idea/navigate/reference?project=Uk-jake.github.io&path=_posts/assets/0828/ChatGPT.png
#  lqip: data:image/webp;base64,UklGRpoAAABXRUJQVlA4WAoAAAAQAAAADwAABwAAQUxQSDIAAAARL0AmbZurmr57yyIiqE8oiG0bejIYEQTgqiDA9vqnsUSI6H+oAERp2HZ65qP/VIAWAFZQOCBCAAAA8AEAnQEqEAAIAAVAfCWkAALp8sF8rgRgAP7o9FDvMCkMde9PK7euH5M1m6VWoDXf2FkP3BqV0ZYbO6NA/VFIAAAA
#  alt: Responsive rendering of Chirpy theme on multiple devices.
---


> 우리는 통상 Backend 개발자가 되기 위해서는 서버를 구축하기위한 언어를 하나 골라야한다. 아마 부트캠프 혹은 국비지원 프로그램만 봐도 우리나라 백엔드 개발자들이 Spring을 얼마나 많이 사용하고 있는지 알 수 있을 것이다. 그래서 너도 나도 Spring을 배우기위해 백엔드 개발 공부를 시작하지만 정작 시작하고 나면 그래서 Spring이 뭔지 초기 설정을 하기 쉽게 도와준다고 SpringBoot를 사용하라는데 그럼 SpringBoot는 무엇인지 도통 하나도 몰랐었던 나의 초창기를 생각하면서 다시한번 Spring에 대해서 그리고 SpringBoot에 대해서 정리하고자 한다.
>

# What is the Spring?

![Untitled](https://github.com/Uk-jake/WebDev2022_/assets/100981076/05cc4258-f5d4-4063-9d24-be1c05852d2a)

위 사진은 Spring 공식 홈페이지의 사진이다. 위 글을 요약하자면

- Spring은 속도, 간결함, 생성성에 초점을 맞춘 Java 프레임 워크이다.
- Spring을 사용하면 시간과 에너지를 줄일 수 있다.

라고 적혀져 있다. 이 글만 보면 Spring을 사용하면 무엇을 빠르게 만들수 있는 것 같은데 Spring에 대해서 조금 더 깊게 알아보자.

## Spring 이란?

- JAVA의 웹 프레임워크로 JAVA 언어를 기반으로 사용한다. JAVA로 다양한 어플리케이션을 만들기 위한 프로그래밍 틀이라 할 수 있다.
- 옛날에 비교하면 지금은 JAVA의 활용도가 높아졌고 따라서 프로젝트 규모도 커졌다. JAVA를 이용한 기술은 JSP, MyBatis, JPA 등 여러가지가 있는데 즉, 이 기술들이 프로젝트에 많이 쓰인다고 할 수 있다. Spring은 이 기술들을 더 편하게 사용하기 위해 만들어진 것이다.
- 프로젝트를 진행하다 보면 아무리 분업을 해도 분명 중복되는 코드가 있기 마련이다. Spring은 이런 **중복코드의 사용률을 줄여주고, 비즈니스 로직을 더 간단**하게 해줄 수 있다.
- Spring을 사용하면 다른 사람의 코드를 참조하여 쓰기 편리한데 이말의 의미는 **오픈소스를 좀더 효율적으로 가져다 쓰기 좋은 구조**라는 것이다.
- 결론적으로 **Spring이란 JAVA 기술들을 더 쉽게 사용할 수 있게 해주는 오픈소스 프레임 워크**이다.

## Spring 주요 특징

사실 Spring을 사용하는데에는 아래에 있는 특징들 때문이라고 할 수 있다.

**1. IoC(Inversion of Control, 제어 반전)**

- 개발자는 JAVA 코딩시 new 연산자, 인터페이스 호출, 데이터 클래스 호출 방식으로 객체를 생성하고 소멸시킨다.
- IoC란 인스턴스 (객체)의 생성부터 소멸까지 **객체 생명주기 관리를 개발자가 하는게 아닌 스피링(컨테이너)가 대신 해주는 것**을 말한다.
- IoC는 개발자가 실수할 수 있는 생명주기 관리를 대신 해준다.
- 프로젝트의 규모가 커질수록 객체와 자원을 이용하는 방법이 더 복잡해지고 어디서 코드가 꼬일지 모르는 것을 Spring의 IoC는 자동으로 관리해준다.
- 즉, **제어권이 개발자가 아닌 IoC에게 있으며** IoC가 개발자의 코드를 호출하여 그 코드로 생명주기를 제어하는 것이다.

**2. DI(Dependency Injection, 의존성 주입)**

- 프로그래밍에서 **구성요소 간의 의존 관계**가 소스코드 내부가 아닌 **외부의 설정파일을 통해 정의**되는 방식이다.
- 코드 재사용을 높여 재사용을 높여 소스코드를 다양한 곳에 사용할 수 있으며 모듈간의 결합도도 낮출 수 있다.
- 쉽게 말하자면 게임 캐릭터라는 하나의 객체가 존재하는데, 그 객체를 더 잘 이용하기 위해서 무기, 방패 등 아이템을 가져와 결합시키는 것이다. 이 객체는 무기와 방패를 뺐다 꼈다 자유자재로 할 수 있으며 아이템을 갈아끼우는데 어떤 상황에 구애받지도 않는다.
- JAVA에서 데이터를 저장하고 가져오는 기능을 외부의 Oracle Database를 사용할 수도 있고, JDBC, iBatis, JPA 등 다른 프레임 워크를 이용해 짤 수도 있다. 이때 Spring을 이용하면 그때마다 **필요한 부분을 뺐다 꼈다 하면서 적절한 상황에 필요한 기능**을 해낼 수 있다.

**3. AOP(Aspect Object Programming, 관점 지향 프로그래밍)**

- 로깅, 트랜잭션, 보안 등 여러 모듈에서 공통적으로 사용하는 **기능을 분리하여 관리** 할 수 있다.
- 각각의 클래스가 있다고 가정하자. 각 클래스들은 서로 코드와 기능들이 중복되는 부분이 많다. 코드가 중복될 경우 실용성과 가독성 및 개발 속도에 좋지 않다. 중복된 코드를 최대한 배제하는 방법은 중복되는 기능들을 전부 빼놓은 뒤 그 기능이 필요할때만 호출하여 쓰면 훨씬 효율성이 좋다.
- 즉, AOP는 **여러 객체에 공통으로 적용할 수 있는 기능을 구분함으로써 재사용성을 높여주는 프로그래밍 기법**이다.

**4. POJO(Plain Old Java Object) 방식**

- POJO는 Java EE를 사용하면서 해당 플랫폼에 종속되어 있는 무거운 객체들을 만드는 것에 반발하여 나타난 용어이다.
- 별도의 프레임 워크 없이 Java EE를 사용할 때에 비해 인터페이스를 직접 구현하거나 상속받을 필요가 없어 기존 라이브러리를 지원하기 용이하고, 객체가 가볍다.
- 즉, **getter/setter를 가진 단순한 자바 오브젝트**를 말한다.

# 그러면 SpringBoot는 무엇인가?

Spring을 사용하면 유용한 Java의 기술들을 사용하여 어플리케이션을 만들 수 있다는 것까지는 알았는데 그러면 SpringBoot는 무엇이지?

![위 그림은 Spring 공식 홈페이지에 나온 SpringBoot의 설명이다.](https://github.com/Uk-jake/WebDev2022_/assets/100981076/19591635-80cf-47df-967a-25a306e18a03)

위 그림은 Spring Boot 공식 홈페이지의 나온 설명이다.

> 스프링부트는 너가 단지 실행시킬 수 있도록 스프링 기반의 어플리케이션을 쉽게 만들어준다.
>

스프링은 기존 기술의 복잡성을 크게 줄인 프레임워크이지만 스프링을 사용하기 위해서는 여러가지 사항을들을 주의해야한다. 하지만 Spring Boot를 사용하면 필요한 설정 없이 내가 추가하고 싶은 기능들만 선택하면 초기설정을 알아서 다 해주는 프레임 워크이다.

## Spring Boot의 특징

- **Auto-Configuration**: 자동으로 필요한 설정을 해준다.
- **내장 서버**: Tomcat, Jetty 등의 웹 서버를 내장하고 있어 별도의 웹 서버가 필요 없다.
- **의존성 관리**: **`starter`**를 통해 필요한 라이브러리를 쉽게 추가할 수 있다.
- **생산성 향상**: 다양한 플러그인과 라이브러리를 쉽게 연동할 수 있어 개발 속도가 빠르다.

Spring Boot는 아래 링크에서 사용할 수 있다.

[](https://start.spring.io/)

![SpringBoot의 .jar 구조](https://github.com/Uk-jake/WebDev2022_/assets/100981076/c8c7d178-3abc-4b6b-8148-3dc5485d6fba)

그리고 SpringBoot의 jar파일은 위 그림과 같이 code와 Tomcat파일이 함께 존재한다고 한다.

### 주요 내용 정리

- 스프링은 엔터프라이즈용 Java 애플리케이션 개발을 편하게 할 수 있게 해주는 오픈소스 경량급 애플리케이션 프레임워크다.
- 스프링은 POJO 프로그래밍을 지향하는 특징을 가지며, 그를 위해 IoC/DI, AOP, PSA를 지원한다.
- IoC는 객체 간의 의존 관계를 개발자가 아닌 스프링이 맺어주는 것을 의미한다.
- DI는 의존 객체를 특정 클래스에서 직접 생성하는 것이 아니라, 외부로부터 주입해주는 것을 의미한다.
- AOP는 애플리케이션 전반에 걸쳐 공통적으로 적용되는 코드들을 비즈니스 로직으로부터 분리해내는 것을 의미한다.
- PSA는 특정 기술과 관련된 서비스들을 추상화하여 일관된 방식으로 사용할 수 있도록 한 것을 의미한다.
- 스프링 부트는 스프링 애플리케이션을 만들 때에 필요한 초기 설정을 간편하게 해주는 프레임워크다.
- Spring Initializr를 사용하면 스프링 프로젝트를 편리하게 생성할 수 있다.
