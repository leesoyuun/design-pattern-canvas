## 디자인 패턴 with canvas
## SOLID 원칙
### Single Responsibility Principle(SRP)
단일책임 원칙
- 한 객체는 하나의 책임만 가져야한다. (여기서 책임 == 변경의 이유)
- 그러나 객체가 많아질 때에는 지켜지지 않는 경우가 있음
- 단일 책임 원칙은 프로그램의 유지보수성을 높이기 위한 설계 기법임
### Open Closed Principle(OCP)
개방 폐쇄 원칙
- 확장에 대해서는 열려있고 변경에 있어서는 닫혀있어야함
- 새로운 기능을 추가할 때 기존의 코드가 추가되어서는 안된다.
### Liskov Substitution Principle(LSP)
리스코프 치환원칙
- 자식클래스는 "언제나" 부모 클래스의 역할을 대체할 수 있어야한다.
- 부모 클래스의 자리에 자식 클래스를 넣고 타입 에러가 나나 확인해보면 됨
### Interface Segregation Principle(ISP)
인터페이스 분리 원칙
- 인터페이스를 각각 사용에 맞게 끔 잘 분리해야한다.
- 클래스는 자신이 사용하지 않는 인터페이스는 구현하지 말아야 한다.
- 인터페이스의 단일 책임 원칙
- 인터페이스를 쪼개서 여러 개로 만들고, 필요한 만큼 implements

=> 인터페이스를 한번 구성하였으면 가급적 수정하면안된다.

### Dependency Inversion Principle(DIP)
의존성 역전 원칙
- 어떤 클래스를 참조하여 사용해야하는 상황이 생기면 그 Class를 직접 참조하는 것이 아니라 대상의 상위요소를 참조하라는 원칙
- 추상성이 높은 클래스와 의존 관계를 맺는다
- 상속 대신 합성을 하자
- interface, abstract class를 매개변수로 받자

=> 지향점 : 각 클래스간의 결합도를 낮추는 것

## Gof의 디자인 패턴
## 생성(creational patterns)
### 싱글턴(Singleton)
하나의 인스턴스만 존재함을 보장
- 생성자도 private으로(자바스크립트에서는 symbol 사용해서 생성자 호출 막기)
- 단일 책임 원칙 위반!
- 강결합으로 인해 테스트하기 어려움
![Alt text](image.png)


