# 3.4 백엔드 프레임워크

## 3.4.1 라이브러리와 프레임워크

**라이브러리(Library)** : 개발하는데 필요한 기능을 미리 구현해놓은 코드의 모음. 제사용이 가능한 기능을 라이브러리로 만들어두면 필요한 곳에서 호출해 사용할 수 있음.

**프레임워크(Framework)** : 복잡한 문제를 해결하거나 서술하는 데 사용되는 기본 구조로, 그 이름에서 유추할 수 있듯이 뼈대 혹은 골조를 의미함. 개발에서 프레임워크란 개발에 필요한 뼈대, 즉 일정한 형태와 기능을 제공하는 틀임.

<br />

:spiral_notepad: 라이브러리와 프레임워크의 프로그래밍 작성 방식에서의 차이

:small_blue_diamond: 라이브러리 : 개발자가 코드의 흐름을 직접 제어함. 어떤 코드가 필요할지 개발자가 직접 판단하고 해당 라이브러리를 호출해 사용함.

:small_blue_diamond: 프레임워크 : 개발자가 주어진 코드의 흐름 속에서 프로그래밍함. 개발자가 직접 일정한 로직과 틀을 만들어 기능을 구현하는 라이브러리와 달리 이미 짜여 있는 틀 안에서 개발자가 원하는 부분을 작성함.

<br />

## 3.4.2 Express.js : 자바스크립트 기반

Node.js는 모든 종류의 서버 측 도구와 프로그램을 자바스크립트로 만드는 데 이용하는 런타임 환경임. Node.js를 사용하면 웹 브라우저 밖에서도 자바스크립트 코드가 동작하기 때문에 Node.js만으로 백엔드 개발을 할 수 있음.

**Express.js(익스프레스)** : Node.js가 제공하는 API를 바탕으로 백엔드 개발을 할 수 있도록 만들어진 프레임워크.

<br />

:spiral_notepad: **Express.js 장점**

:one: 프레임워크 자체가 경량화돼 간단하고 빠르게 웹 서버를 만들 수 있음.

:two: 유연성이 뛰어나 필요한 기능만 선택해 사용할 수 있음.

:three: 다양한 미들웨어(Middleware)와 플러그인(Plugin)을 지원.

**미들웨어** : 각종 조정과 중계 역할을 하는 소프트웨어. 클라이언트의 요청과 서버의 응답 사이에 위치.

**플러그인** : 기존 소프트웨어에 추가 프로그램을 설치해 특정 기능을 수행할 수 있도록 해주는 소프트웨어 모듈.

:four: RESTful API를 쉽고 간단하게 구현할 수 있음.

**RESTful API** : 두 컴퓨터 간에 HTTP 통신으로 데이터를 주고받는 방법을 설계한 것.

:five: 관련 커뮤니티가 활성화돼 있어 문제를 쉽게 해결할 수 있음.

<br />

:spiral_notepad: **Express.js 단점**

:one: Node.js를 경량화해 만든 프레임워크라고급 기능이나 대규모 프로젝트를 개발하기에 부족함.

:two: 프로젝트의 규모가 커질수록 코드의 구조가 복잡해질 수 있음.

:three: Node.js 기반의 서버를 구축하기 때문에 멀티스레드를 지원하지 않음.

:four: 공식적으로는 세션 관리, 데이터베이스 연결 등과 같은 기능을 지원하지 않음. 세션 관리, 데이터베이스 연결 등을 구현하려면 별도의 서드파티 라이브러리(Third Party Library, 개인 개발자나 프로젝트 팀 또는 업체가 개발한 라이브러리)를 사용해야 함.

<br />

## 3.4.3 NestJS : 타입스크립트 기반

**NestJS(네스트)** : 타입스크립트를 우선적으로 지원하고 자바스크립트도 사용 가능한 프레임워크로, Express.js의 기능을 이어받아 보완 및 확장된 기능을 제공.

데이터베이스, ORM, 각종 설정, 유효성 검사 등 수많은 기본 기능을 제공하고, 필요한 라이브러리를 쉽게 설치해 확장할 수 있음.

의존성 주입(DI, Dependency Injection), 제어 역전(IoC, Inversion of Control)과 같은 객체지향 개념을 사용함.

<br />

:spiral_notepad: **NestJS의 장점**

:one: ​타입스크립트를 사용하기 때문에 정적 타입 검사를 함으로써 코드 예측성이 높아져 코드의 안정성이 향상됨.

:two: 모듈화와 의존성 주입을 지원해 모듈 간의 결합도를 낮추고 코드의 재사용성을 높일 수 있음.

:three: 향후 확장하기 쉬운 마이크로서비스 아키텍처를 구현하기 위한 기능이 내장돼 있음.

<br />

:spiral_notepad: **NestJS의 단점**

:one: 많은 설정 옵션과 다양한 기능을 제공하기 때문에 초기 설정이 다소 복잡함.

:two: Express.js보다 무겁기 때문에 속도가 느림.

<br />

## 3.4.4 스프링 : 자바 기반

**스프링(Spring)** : 자바 기반의 백엔드 프레임워크

비즈니스 로직 : 제공하는 서비스를 코드로 구현한 것으로, 사용자의 요구 사항을 충족하고 해결하기 위한 실질적인 코드를 작성하는 과정.

스프링은 **POJO(Plan Old Java Object)**을 지향함. POJO는 '오래된 방식의 간단한 자바 객체' 임.이는 순수하게 자바만 이용해 만든 객체를 사용하겠다는 뜻.

스프링은 POJO를 지향하기 위해 :one:**의존성 주입(DI, Dependency Injection)**, :two: **제어 역전(IoC, Inversion of Control)**, :three: **AOP(Aspect-Oriented Programming)**, :four: **PSA(Portable Service Abstraction)**을 지원함.

<br />

 ## 3.4.5 스프링 부트 : 자바 기반

**스트링 부트(Spring Boot)**는 개발자가 스프링을 사용할 때 실행 환경이나 의존성 관리 설정에 들이는 시간과 에너지를 아껴 비즈니스 로직에 좀 더 집중할 수 있게 해줌. 또한 스프링 부트는 내부에 웹 애플리케이션 서버(WAS)인 톰캣을 가지고 있음. 스프링을 사용하는 경우 톰캣을 별도로 설치한 후 연동해야 하지만, 스프링 부트는 톰캣이 내장돼 있어 별도로 설치하는 과정 없이 바로 사용할 수 있음.