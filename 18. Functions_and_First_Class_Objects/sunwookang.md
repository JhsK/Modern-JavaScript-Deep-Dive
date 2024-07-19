## 일급 객체

1. 무명의 리터럴로 생성할 수 있다. → 함수 이름 없이 사용
2. 변수나 자료구조에 저장할 수 있다.
3. 함수의 매개변수에 전달할 수 있다.
4. 함수의 반환값으로 사용할 수 있다.

자바스크립트의 함수는 위 모든 조건을 만족하므로 일급 객체.

함수를 객체와 동일하게 사용 가능

특징

- 함수의 매개변수에 전달
- 함수의 반환값으로 사용

⇒ 함수형 프로그래밍 가능

## 함수 객체의 프로퍼티

함수도 객체이므로 프로퍼티를 가짐

함수이기에 함수 고유의 프로퍼티를 가짐: arguments, caller, length, name, prototype

arguments

- 함수 호출 시 전달된 인수들의 정보. iterable한 유사 배열 객체
- 지역 변수로 사용
- 가변 인자 함수를 구현할 때 유용
- 요즘은 Rest 파라미터 많이 사용

caller

- 함수 자신을 호출한 함수

length

- 매개변수의 개수

name

- 함수의 이름
- 익명 함수는 함수 객체를 가리키는 변수 이름

__proto__ 접근자 (더블 언더스코더 프로토 → 던더 프로토)

- 모든 객체는 [[Prototype]]이라는 내부 슬롯을 가짐
- [[Prototype]]은 상속을 구현하는 프로토타입 객체
- __proto__ 프로퍼티는 [[Prototype]]이 가리키는 프로토타입 객체에 접근하기 위해 사용
    - 직접 접근 불가. __proto__를 통해 간접적으로 프로토타입 객체에 접근

prototype 프로퍼티

- 생성자 함수로 호출할 수 있는 함수 객체
- constructor만이 소유하는 프로퍼티
- 생성자 함수로 호출될 때 생성자 함수가 생성할 인스턴스의 프로토타입 객체