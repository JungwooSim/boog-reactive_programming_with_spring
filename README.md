## 01. Reactive Programming

### Reactive System 이란?

클라이언트 요청에 즉각적으로 응답함으로써 지연 시간을 최소화하는 시스템

### The Reactive Manifesto (리액티브 선언문) 에서 지향하는 바는 무엇인가?

<img src="/img/1-1.png" width="600px;">

빠른 응답성을 바탕으로 유지보수와 확장이 용이한 시스템

Reactive Manifesto : [https://www.reactivemanifesto.org](https://www.reactivemanifesto.org/)

Reactive Manifesto 용어 : https://www.reactivemanifesto.org/ko/glossary

### Reactive Programming 이란?

Reactive System 을 구축하는데 필요한 program model

**설계 원칙**

- 비동기 메시지 기반 통신으로 동작해야 함
- 탄력적이고 회복성을 지녀야 함
- 높은 응답성을 지녀야 함
- 유지보수와 확장이 용이해야 함

### Reactive Programming 의 특징

- declarative programming
    - c, java 는 명령형 프로그래밍이다.
      즉, 실행할 동작을 구체적으로 명시하는 프로그래밍 코드 형태
    - 선언형 프로그래밍 방식은 실행할 동작을 구체적으로 명시하지 않고 이러이러한 동작을 하겠다고 목표만 선언한다
- data streams 와 the propagation of change
    - data streams : 데이터가 지속적으로 발생한다는 의미
    - the propagation of change : 지속적으로 데이터가 발생할 때마다 이것을 변화하는 이벤트로 보고, 이 이벤트를 발생시키면서 데이터를 계속적으로 전달하는 것을 의미

### Reactive Programming 구성

- Publisher : 입력으로 들어오는 데이터를 Subscriber 에 제공하는 역할
- Subscriber : Publisher 로부터 전달받은 데이터를 사용하는 역할
- Data Source : Publisher 의 입력으로 전달되는 데이터를 의미
- Operator : Publisher 와 Subscriber 중간에서 데이터를 가공하는 역할