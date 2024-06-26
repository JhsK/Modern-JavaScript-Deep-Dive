## 13.1 스코프란?

스코프란 식별자의 유효 범위이다. → 모든 식별자(변수 이름, 함수 이름, 클래스 이름 등)는 자신이 선언된 위치에 의해 다른 코드가 식별자 자신을 참조할 수 있는 유효 범위가 결정된다. 이를 스코프라 한다.

- 스코프는 네임스페이스다.
  - 네임스페이스란? 동일한 이름을 가진 변수나 함수가 다른 네임스페이스 내에서 각각 독립적으로 존재할 수 있도록 합니다.

## 13.2 스코프의 종류

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/bf1ec4e6-0fed-4f24-ad18-6abe8bd7fe6d/30e47a91-f5fd-4c6e-8db5-0c01d0f0cf52/Untitled.png)

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/bf1ec4e6-0fed-4f24-ad18-6abe8bd7fe6d/a27654be-f4a4-4756-8acc-a8ecd21c56a3/Untitled.png)

### 지역과 지역 스코프

지역이란 함수 몸체 내부를 말하며, 지역은 지역 스코프를 만든다. 지역에 변수를 선언하면 지역 스코프를 갖는 지역 변수가 된다. 지역 변수는 자신이 선언된 지역과 하위 지역(중첩 함수)에서만 참조할 수 있다. 다시 말해 지역 변수는 자신의 **지역 변수는 지역 스코프와 하위 지역 스코프에서 유효하다.**

## 13.3 스코프 체인

<aside>
💡

- 스코프 체인을 통해 변수를 참조하는 코드의 스코프에서 시작하여
- **상위 스코프 방향으로 이동하며 선언된 변수를 검색** 한다.> 절대 하위 스코프로 내려가면서 식별자를 검색하는 일은 없다.
- 이를 통해 사위 스코프에서 선언한 변수를 하위 스코프에서도 참조할 수 있다.
</aside>

## 13.5 렉시컬 스코프

<aside>
💡

자바스크립트는 렉시컬 스코프를 따르므로,

- 함수를 어디서 호출했는지가 아니라,
- 함수를 어디서 **정의** 했는지에 따라서 **상위 스코프** 를 결정한다.
- 함수가 호출된 위치는 상위 스코프 결정에 어떠한 영향도 주지 않는다.

이처럼 함수의 상위 스코프는 함수 정의가 실행될 때 정적으로 결정된다.

</aside>
