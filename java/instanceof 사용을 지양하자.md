# instanceof 사용을 지양하자 
최근에 관련된 글을 읽어서 정리 해본다.
## instanceof가 무엇인가?

A instance B 꼴로 사용하는 연산자이다.

B값이 A 객체의 인스턴스이면 True
아니라면 False를 반환한다.
## 그렇다면 왜 지양해야 하는가?

### 1. 캡슐화
* 데이터 은닉에 목적이 있는 

### 2. OCP (Open Closed Principle) 위반
* OCP란 OOP의 원칙중 하나로 
    
    객체의 확장 가능성은 열려있되(open) 변형의 가능성은 닫혀있어야(closed) 한다는 원칙이다.    
* instacneof를 사용해서 코드를 작성하게 된다면 객체의 변형 가능성이 커지게 된다.

### 3. SRP (Single Responsibility Principle) 위반

