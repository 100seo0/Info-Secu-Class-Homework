### 성공적인 코딩 인터뷰를 위한 코딩 인터뷰 정복하기 – 코딩 테스트

#### 객체지향 프로그래밍 (OOP) 개념

1. Class

Object의 template이고 data fields와 methods를 가지고 있음

Object를 만들기 위한 설계도 또는 틀

2. Object

   class의 instance(설계도를 바탕으로 **구현된 구체적인 실체**)

3. Encapsulation(캡슐화)

   클래스에 보안 제공

4. Inheritance(상속)

   코드의 재사용성을 높임

   부모가 가지고 있는 method, field를 따로 선언하지 않아도 됨

5. Polymorphism

   자바에서는 오버로딩과 오버라이딩으로 표현

   같은 이름이나 다르게 행동

   ​	오버로딩(Overloading) : 같은 이름의 메소드를 여러 개 가지면서 **매개변수의 유형과 개수가 다름**

   ```java
   void print() {}
   void print(String data) {}
   ```

   ​	오버라이딩(Overriding) : 상위 클래스가 가지고 있는 **메소드를 하위 클래스가 재정의 해서 사용**

   ```java
   @Override
   public void run() {
   }
   ```

6. Abstraction

   가상 클래스

   구현을 하지 않으나 부모를 가지고 있는 자식 클래스는 그 안에서 구현 해야함

   추상 클래슬를 설계하여 개발자들의 필드명, 메소드명 통일시킬 수 있다.

