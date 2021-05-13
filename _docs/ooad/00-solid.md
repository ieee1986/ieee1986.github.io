---
title: "SOLID"
permalink: /docs/ooad/solid/
excerpt: "ko.wikipedia.org"
last_modified_at: 2021-04-20
redirect_from:
  - /theme-setup/
toc: true
---
### SOLID (객체 지향 설계)

#### SRP 단일 책임 원칙
- Single responsibility principle
- 한 __클래스는 하나의 책임__ 만 가져야 한다.
- ex) Guitar 클래스의 market, type, model, backWood, topWood 와 같은 특성 정보군을 GuitarSpec 으로 정의

#### OCP 개방-폐쇄 원칙
- Open/closed principle
- 소프트웨어의 구성요소는 확장에는 열려 있으나 변경에는 닫혀 있어야 한다.
- __요구사항 변경/추가에 기존 요소는 수정되지 않아야__ 한다.
- ex) Guitar 클래스와 GuitarSpec 클래스, Violin 클래스와 ViolinSpec 클래스가 존재할 경우 Guitar와 Violin을 추상화한 인터페이스를 생성하고, GuitarSpec 과 ViolinSpec을 추상화한 인터페이스를 생성하여 이용한다.

#### LSP 리스코프 치환 원칙
- Liskov substitution principle
- 객체는 하위 타입의 인스턴스로 바꿀 수 있어야 한다. <-> 서브타입은 상위 타입으로 교체될 수 있어야 한다.
- __조직도, 계층도가 아니라 분류도여야 한다.__
- ex) LSP 위반 사례: 할아버지 - 아버지 - 딸
- ex) LSP 구현 사례: 동물 - 포유류 - 고래

#### ISP 인터페이스 분리 원칙
- Interface segregation principle
- 특정 클라이언트를 위한 인터페이스 여러 개가 범용 인터페이스 하나보다 낫다.
- __인터페이스의 단일 책임__ 을 강조한다.
- 범용 인터페이스에서 사용하지 않는 기능을 구현하지 않아야 한다.
- ex) 컴포넌트는 사용할 이벤트의 리스너 인터페이스만 구현한다.

#### DIP 의존관계 역전 원칙
- Dependency Inversion
- 프로그래머는 __추상화에 의존해야지, 구체화에 의존하면 안된다__
- 의존성 주입은 이 원칙을 따르는 방법중 하나이다.
- 실제 사용 관계는 바뀌지 않고, 추상화를 매개로 관계를 갖는다.
- 자신보다 변하기 쉬운 것에 의존하지 않는 규칙으로, 추상화 될 수록 변하지 않을 가능성이 크다.
