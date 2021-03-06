---
title: "잘 설계된 프로그램이 세상을 뒤흔든다."
permalink: /docs/ooad/well-designed-program/
excerpt: "Object-Oriented Analysis & Design"
last_modified_at: 2021-04-22
redirect_from:
  - /theme-setup/
toc: true
---
#### 위대한 소프트웨어란 ?

1. 고객이 원하는 기능을 수행해야 한다.
2. 잘 설계되어 있고, 잘 코딩 되어 있고, 유지보수와 재사용, 확장이 쉽다.

#### 위대한 소프트웨어를 만드는 3단계

1. 고객이 원하는 기능을 하도록 만들자.
 - 요구 사항을 잘 수집하고 분석해야 한다.
2. 객체지향의 기본 원리를 적용해서 유연한 소프트웨어를 만들자.
 - 제대로 동작하는 프로그램을 가지고, 내부 구조가 실제로 잘 구성되어 있는지 확인한다.
3. 유지보수와 재사용이 쉬운 디자인을 위해 노력하자.
 - 디자인 패턴과 원리를 적용한다.

#### 소스코드의 문제를 해결하면서 새로운 문제를 만들지 말자.

#### 잘못 사용된 객체 예제

1. 객체가 비행기인 경우 이륙하고 착륙해야 하지만, 비행기표를 받지는 말아야 한다.
2. 객체가 값이 없거나 null 인 속성을 가진채로 사용하면, 객체가 하나 이상의 일을 하고 있을 가능성이 있다.
3. Guitar, Inventory 에서 Inventory.search(Guitar guitar) 와 같은 경우.
  - GuitarSpec 이 생성 되어야 한다. Guitar 와의 중복 코드를 GuitarSpec 에 정의하고, Guitar 가 GuitarSpec을 참조하게 하면 중복을 피할 수 있다.

#### 중복 코드를 볼 때마다 캡슐화 할 곳이 있는지 확인하자.

1. 캡슐화의 개념은 프로그램의 일부의 정보를 다른 부분으로부터 보호하는 것.
2. 클래스에서 행위를 캡슐화 할 경우, 클래스가 변하지 않고도 행위를 변경할 수 있다.
3. 변화 가능성이 높은 부분을 그렇지 않은 부분으로부터 분리하여 캡슐화 하자.

#### Object-Oriented Analysis & Design 는 위대한 소프트웨어를 작성하는 방법에 관한 것

1. 고객은 프로그램이 동작할 때 만족스러워 한다.
2. 고객은 프로그램이 계속 잘 동작할 때 만족스러워 한다.
3. 고객은 프로그램이 업그레이드가 가능할 때 만족스러워 한다.
4. 프로그래머는 자신의 프로그램이 재사용될 수 있을 때 만족스러워 한다.
5. 프로그래머는 자신의 프로그램이 유연할 때 만족스러워 한다.

#### 4, 5의 경우로 만족한적이 있는가?
