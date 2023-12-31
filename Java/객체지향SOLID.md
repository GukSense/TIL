## SOLID 
좋은 객체지향 설계의 5가지 원리를 말한다.
- SRP: 단일 책임 원칙
- OCP: 개방-폐쇄 원칙
- LSP: 리스코프 치환 원칙
- ISP: 인터페이스 분리 원칙
- DIP: 의존관계 역전 원칙

### SRP 단일 책임 원칙
- 한 클래스는 하나의 책임만 가져야한다.
  -  하나의 책임이라는것은 모호하다. 클 수 도있고 작을 수 도있다. 문맥과 상황에 따라 다르다.
- **중요한 기준은 변경**  변경이 있을 때 파급효과가 적다면 단일 책임 원칙을 잘 따른것.

### OCP 개방-폐쇄 원칙
- **확장에는 열려**있으나 **변경에는 닫혀**있어야한다.
- 다형성을 잘 활용해야한다.

### LSP 리스코프 치환 원칙
- 프로그램의 객체는 프로그램의 정확성을 깨트리지 않으면서 하위타입의 인스턴스로 바꿀 수 있어야한다.
  - 다형성에서 하위클래스는 인터페이스의 규약을 지켜야한다. 단순히 컴파일에 성공하는것을 넘어서는 이야기. EX) 자동차 인터페이스의 악셀 기능은 앞으로 가기위한 기능. 뒤로 가게 구현하면 LSP 위반이라는 소리.  
### ISP 인터페이스 분리 원칙
- 특정 클라이언트를 위한 인터페이스 여러개가 범용 인터페이스 하나보다 낫다.
- 자동차 인터페이스 : 운전인터페이스 정비 인터페이스로 분리
- 사용자 클라이언트 : 운전자 클라이언트, 정비사 클라이언트로 분리
  - 이런식으로 분리하며 정비인터페이스 자체가 변해도 운전자 클라이언트는 영향을 받지 않음.
- 인터페이스가 명확해지고, 대체가능성이 높아진다.    
### DIP 의존관계 역전 원칙
- 프로그래머는 추상화에 의존해야지 구체화에 의존해서는 안된다.
- 클라이언트코드는 구현클래스에 의존하지말고 인터페이스에 의존해야한다.
- 구현체에 의존하면 변경이 아주 어려워진다. 
