**JavaScript 개념 정리 회의록**

## 김예림

• typeof null이 'object'로 나오는 이유를 학습.
• https://witch.work/ko/posts/javascript-why-typeof-null-is-object

## 김지윤

• **호이스팅 개념 정리**
• var, let, const 모두 호이스팅되지만 **초기화되는 시점이 다름**.
• TDZ(Temporal Dead Zone) 개념을 명확히 이해함.
• 변수의 객체화 과정에서 초기화 시점이 다르기 때문에 참조 여부가 달라짐.

## 김진명

• **기본 개념 학습**
• 선언, 할당, 초기화 개념을 명확하게 파악.
• **데이터 타입의 필요성**
• 이진수 값을 어떻게 해석하는지 학습.

## 노현호

• **NaN 개념 학습**
• 비교했을 때 자기 자신과도 일치하지 않는 값이라는 점을 새롭게 알게 됨.
• **TDZ(Temporal Dead Zone) 개념 정리**
• https://ccomccomhan.tistory.com/288

## 박재형

• **호이스팅과 TDZ 관련 개념 정리**
• 선언 시 메모리 공간 할당이 이루어지지만, 값이 초기화되지 않으면 TDZ에 머무름.
• let과 const의 TDZ로 인해 할당 전 참조 시 **ReferenceError** 발생.
• var는 undefined로 초기화됨 → 호이스팅 시 ReferenceError가 발생하지 않음.
• **JS의 에러 처리 방식**
• High-level에서 안정성을 추구하기 위해 undefined 사용.
• **초기화 과정의 중요성**
• 메모리 공간 확보 후 초기화하는 과정에서 **쓰레기 값 방지** 및 안정성 확보.

## 소재훈

• **JavaScript 기본 개념 학습**
• var, let, const 키워드 개념 학습.
• String 객체와 원시 타입 차이 이해.
• 깊은 복사, 얕은 복사 개념 정리.
https://f-lab.kr/insight/understanding-javascript-variable-declaration-and-tdz-20240828

## 유제원

• **ES6 개념 학습**
• Symbol 개념 학습.
• JSON과의 차이점을 구별하는 용도로 사용 가능.
• 글로벌 심볼을 활용해 전역적으로 사용 가능.

## 윤혜원

• **var, let, const 개념 정리**
• **삼항 연산자 개념 학습**
• **null과 undefined 차이 정리**

```js
- null: "값이 없음"을 개발자가 의도적으로 설정.
- undefined: "값이 할당되지 않음", 변수가 선언되었지만 값이 없을 때 자동 부여됨.
```

## 장민호

• **TDZ(Temporal Dead Zone) 개념 정리**
• **JavaScript의 호이스팅 개념 정리**
• **Node.js와 런타임 개념 학습**
• 모듈 시스템을 통해 코드 관리가 용이.
• **JavaScript의 숫자 연산**
• Number.EPSILON을 활용한 **부동소수점 오차 감소** 개념 학습.
• **V8 엔진 개념 학습**
• V8은 **JavaScript 인터프리팅 + JIT 컴파일 기능 포함**.

## 지민성

• **메모리 주소 개념 학습**

```js
console.log([10, 20] === [10, 20]); // false (다른 메모리 주소)
```

• **var 지양 이유**
• 호이스팅 및 TDZ 문제로 인해 사용을 피하는 것이 좋음.
• **선언형 프로그래밍 권장**
• 구조 분해 할당을 활용해 가독성을 높이는 것이 좋음.
• **ESLint 도입 이유 이해**
• **Infinity 전역 변수 개념 학습**
• **typeof vs instanceof 차이점**

```js
typeof new Date(); // "object" (구별 불가)
new Date() instanceof Date; // true (구별 가능)
```

• **isNaN() 함수 학습**
• 내부적으로 **형 변환이 발생**하는 경우가 있음.
• **코드 스타일 개선**
• if-else보다 **early return**이 가독성 측면에서 유리함.
• switch 문은 **유지보수에 유리**.
