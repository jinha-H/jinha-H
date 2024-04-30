![header](https://capsule-render.vercel.app/api?type=waving&color=timeAuto&section=header&height=130&text=Welcome👻&animation=blink&fontSize=80&fontAlignY=70&fontColor=514E72&)
# *"Core JavaScript"* by 정재남
2024-1 `사물인터넷` 수업에서 사용된 교재입니다.  
`2024.03.~2024.06` 동안 진행할 **예제**에 대한 comment 입니다.
## Ch.1
* **1-1** 변수 선언(var)
* **1-2** 변수 선언과 해당 변수에 데이터 할당 과정을 2줄 혹은 1줄로 표현 가능.
* **1-3** 불변성: 기본형 데이터는 모두 불변값으로 예제와 같이 문자열 값도 한 번 만든 값을 바꿀 수 없으며, 숫자 값도 변경 불가능.
* **1-4** 참조형 데이터 할당: identifier 영역에 data 영역의 상수 및 변수를 할당.
* **1-5** 참조형 데이터의 property 재할당: 참조형 데이터에 할당되어 있는 데이터영역의 값을 재할당.
* **1-6** 중첩된 참조형 데이터(객체)의 property 할당
* **1-7** 변수 복사 비교: 기본형 데이터와 참조형 데이터의 차이 비교
* **1-8** 변수 복사 이후 값 변경 결과 비교: 객체의 property 변경 시 기본형 데이터는 값이 달라지지만, 참조형 데이터의 값은 달라지지 않는다.
* **1-10** 객체의 가변성에 따른 문제점: 정보를 변경하여도 두 변수가 동일하게 나오는 문제점으로 인해, 정보가 바뀐 시점에 바뀌기 전의 정보와 바뀐 후의 정보의 차이를 가시적으로 보여주는 기능은 1-10 코드에서는 어려움.
* **1-11** 객체의 가변성에 따른 문제점 해결 방법: 변경 전과 후에 서로 다른 객체를 바라보게 하여 해결. 그러나, 대상 객체에 정보가 많을수록 변경할 정보가 많아지므로 수고가 증가할 것.
* **1-12** 얕은 복사(기존 정보를 복사하여 새로운 객체를 반환하는 함수)
* **1-13** copyObject를 이용한 객체 복사
* **1-14** 중첩된 객체에 대한 얕은 복사
* **1-15** user.urls 프로퍼티에 대해서도 불변 객체 만들기
* **1-16** 객체의 깊은 복사를 수행하는 범용 함수
* **1-17** 깊은 복사에 대한 확인
* **1-18** JSON을 활용한 간단한 깊은 복사
* **1-19** 자동으로 undefined 부여하는 경우
* **1-20** undefined와 array
* **1-21** 빈 요소와 배열의 순회
* **1-22** undefined와 null의 비교

## Ch.2
* **2-1** 실행 컨텍스트와 콜 스택: 어떤 순서로 쌓이고, 코드 실행에 관여하는 순서 확인.
* **2-2** 매개변수와 변수에 대한 Hoisting(1)-원본 코드
* **2-3** 매개변수와 변수에 대한 Hoisting(2)-매개변수를 변수 선언/할당과 같다고 간주하여 변환한 상태
* **2-4** 매개변수와 변수에 대한 Hoisting(3)-호이스팅을 마친 상태
* **2-5** 함수 선언의 Hoisting(1)-원본 코드
* **2-6** 함수 선언의 Hoisting(2)-호이스팅을 마친 상
* **2-7** 함수 선언의 Hoisting(3)-함수 선언문을 함수 표현식으로 바꾼 코드
* **2-8** 함수를 정의하는 세 가지 방식-1.함수 선언문 2.익명 함수 표현식 3.기명 함수 표현식
* **2-9** 함수 선언문과 함수 표현식(1)-원본 코드
* **2-10** 함수 선언문과 함수 표현식(2)-Hoisting을 마친 상태
* **2-11** 함수 선언문의 위험성.
* **2-12** 상대적으로 함수 표현식이 안전함을 보여줌.
* **2-13** Scope chain : JavaScript는 전역공간을 제외하면 오직 함수에 의해서만 스코프가 형성됨. 따라서, 여러 스코프에서 동일한 식별자를 선언한 경우 무조건 스코프 체인 상에서 가장 먼저 발견된 식별자에게만 접근 가능함.

## Ch.3
* **3-1** 전역 공간에서의 this(browser 환경)
* **3-2** 전역 공간에서의 this(Node.js 환경)
* **3-3** 전역 변수와 전역 객체(1)-전역공간에서 선언한 변수에 데이터 할당할 경우, 모두(window 및 this) 데이터 출력.(전역공간에서의 this는 전역객체를 의미하기 때문)
* **3-4** 전역 변수와 전역 객체(2)
* **3-5** 전역 변수와 전역 객체(3)-delete에 관한 내용
* **3-6** 함수로서 호출, method로서 호출 비교(함수 앞에 .(점)의 유무에 따른 간단한 비교도 가능)
* **3-7** method로서 호출 - 점 표기법과 대괄호 표기법
* **3-8** method 내부에서의 this
* **3-9** 내부 함수에서의 this
* **3-10** 내부 함수에서의 this를 우회하는 방법-outer scope에서 self(편하게 지정) 라는 변수에 this를 저장한 상태에서 호출한 innerFunc2의 경우 self에는 객체 obj가 출력됨.
* **3-11** this를 바인딩하지 않는 함수(화살표 함수)
* **3-12** callback 함수 내부에서의 this
* **3-13** 생성자 함수 : 생성자는 구체적인 instance를 만들기 위한 일종의 틀. new 명령어와 함께 함수를 호출하면 해당 함수가 생성자로서 동작하게 됨.
* **3-14** call 메서드(1)-메서드의 호출 주체인 함수를 즉시 실행하는 명령어(임의의 객체를 this로 지정할 수 있음)
* **3-15** call 메서드(2)
* **3-16** apply 메서드 : call 메서드와 기능적으로 동일하지만, call 메서드는 첫 인자 제외 모든 인자들을 호출할 함수의 매개변수로 지정, but apply 메서드는 두 번째 인자를 배열로 받아 그 배열의 요소들을 호출할 함수의 매개변수로 지정함.
* **3-17** call/apply 메서드 활용 1-1) 유사 배열객체에 배열 메서드를 적용한 예시
* **3-18** call/apply 메서드 활용 1-2) arguments, NodeList에 배열 메서드를 적용한 예시
* **3-19** call/apply 메서드 활용 1-3) 문자열에 배열 메서드를 적용한 예시
* **3-20** call/apply 메서드 활용 1-4) ES6의 Array.From 메서드
* **3-21** call/apply 메서드 활용 2) 생성자 내부에서 다른 생성자 호출
* **3-22** call/apply 메서드 활용 3-1) 최대 최소 값을 구하는 코드 구현
* **3-23** call/apply 메서드 활용 3-2) 여러 인수를 받는 메서드(Math.max/Math.min)에 apply를 적용
* **3-24** call/apply 메서드 활용 3-3) ES6의 펼치기 연산자 활용
* **3-25** bind 메서드 - this 지정과 부분 적용 함수 구현
