## 📍 21일차 11.23.화.(실시간 강의) (클린코드와 타입스크립트)

이번주는 `클린코드`와 `typescript`의 `타입`, `클래스`, `인터페이스`, `Generic`, `Decorator`에 대해서 배웠다. 엘리스 엔지니어 SW트랙을 신청할 당시 제일 기대가 되었던 커리큘럼이 이번주차에 배우는 내용이었는데, 벌써 그 내용을 듣게 된다니.. 이전보다 더욱 열심히 들어야겠다. 여느때와 마찬가지로 이론수업과 실습수업으로 나뉘었는데, 실습수업은 김병철 코치님이 가르쳐주셨다. 처음에는 누군지 잘 몰랐는데 알고리즘계에서 꽤 유명한 분이셨다. 개발자 오픈채팅방에 코딩테스트 대비 순서에 대해 물어보면 항상 <a href='https://github.com/tony9402/baekjoon'>tony9402 - 코딩테스트 대비 문제집</a>부터 풀라는 얘기가 많았는데 그 레포지터리 컨트리뷰터의 2번째(<a href='https://github.com/VSFe'>VSfe</a>)분이셨다. 😲😲 저번 이고잉님이 가르쳐주실때도 신기했는데 이번에도 엄청 신기했다.. 공부 의지가 한껏 솟아오르는 계기가 되었다.

### ❏ 클린코드란

1. 비즈니스 전문가 → 분석가(제품관리자 / 서비스 기획자 / 프로그래머) → 프로그래머 → 컴퓨터
2. 좌측 방향은 목적 / 추상적, 우측 방향은 수단 / 구체적
3. 시간이 갈수록 코드를 쓰는것보다 읽는 비중이 늘어난다.(코드 가독성의 중요성이 늘어남)
4. 코드 재사용(반복되는 문제의 풀이는 재사용 가능, SW 개발 비용 절감)

### 💡 테스트 기법

1. 수동 테스트

-   품질 담당자가 UI를 사용해 기능 검증
-   사람의 손으로 일일이 테스트한다.(인건비 증가)
-   소프트웨어 회귀(시간에 따라 기능이 많아지면, 추가한 기능과 기존의 기능과의 충돌로 인해 기존의 있던 코드조차 실행이 안되는 현상이 발생한다.)

2. 인수 테스트

-   배치된 시스템을 대상으로 검증
-   전체 시스템 이상 여부 신뢰도가 높음
-   높은 비용(작성 / 관리 / 실행 비용)
-   피드백 품질이 낮음(현상을 드러나지만 원인은 숨겨짐)
-   테스터가 품질 외부를 살펴본다.

3. 자동 테스트

-   기능을 검증하는 코드를 작성
-   테스트 코드 작성 비용이 소비되지만 실행 비용이 낮고 결과의 신뢰도가 높음
-   테스트 코드 작성과 관리가 프로그래머 역량에 크게 영향을 받는다.

4. 단위 테스트

-   시스템 일부(하위 시스템)를 대상으로 검증
-   낮은 비용
-   높은 피드백 품질
-   전체 시스템 이상 여부 신뢰도가 낮음
-   단위끼리 오류가 나는 경우가 있다.
-   테스터가 프로그램의 기능을 살펴본다.

### ❏ 타입스크립트의 역사

1. ES2015부터 모듈 스펙을 제공하기 시작: 프로젝트의 규모 증가, 개발환경이 복잡해짐, `npm` 의 등장, 번들러 등장(Webpack 등등) 주석제거 / 파일압축 / 어글리파이, 트랜스파일러 등장 (Babel, Typescript 등등)
2. `TS` 는 `JS` 의 모든 기능을 기본으로 제공한다. (슈퍼셋), 명시적인 데이터에 대한 유형 설명
3. 자바스크립트보다 타입에 대한 추가적인 정보를 얻을 수 있다.
4. 안정성 있는 코드를 작성하기 위하여 별도의 타입체크가 필요함
5. 예상치 못한 오류가 발생할 수 있음
6. 타입 체크를 위해 코드가 길어지는 문제 발생
7. 실제 코드를 실행을 해보기 전까지 오류 체크 불가
8. 실제 서비스 단계가 아닌 컴파일러 과정에서 오류를 확인할 수 있다.(디버깅, 새로고침 과정까지 가지 않아도 확인 가능함) 보다 안전한 프로그래밍 환경을 제공받을 수 있다.

```
JS
 - 인터프리터 언어(한줄 한줄 실행)
 - 스크립팅 언어
 - 컴파일러 필요 없음
 - 객체 지향적이지 않음, 프로토타입 기반

TS
 - 컴파일 언어
 - 객체 지향 프로그래밍 언어
 - 컴파일러 필요
 - 클래스 기반, 상속, 인터페이스, 수정자 사용 가능
```

### ❏ typescript의 type알아보기

1. 인터페이스의 경우, 컴파일하는 과정에서 인터페이스끼리 전부 합쳐지고 해당 인터페이스에 대응하는 객체를 생성해주는 과정을 거칩니다. (JS의 호이스팅을 떠올릴 수 있지만, 실제 동작과정은 약간 다릅니다. 일반적으로 인터페이스, 클래스 등의 정의는 최상단에 고정하고 하단에 추가하거나 수정하는 것은 지양하는 편 입니다.)

```typescript
// 타입 유틸리티
// 1. Tuple: 튜플, 보다 엄격하게 타입을 정의하고 싶을 때 사용
let x : [number, string];
x = [27, "AYW"];

// enum
enum Color {
	Red, Green, Blue
}

console.log(Color)
👉🏽 { 0: 'Red', 1: 'Green', 2: 'Blue', Red: 0, Green: 1, Blue: 2 }

 - 값을 할당해주지 않으면 0, 1, 2가 들어간다.

enum Color {
	Red = 2, Green, Blue
  }

console.log(Color[2])
👉🏽 Red

// any
let num: any = "123";

// void: 함수가 리턴하는 값이 없을 때 사용하는 타입
function warnUser(): void{
  console.log("This is my warning message")
}

function temp(age: number): number{
  return age;
}

// null
let none: null = null;

// undefined
let done: undefined = undefined;

// never
function error(message: string): never{
  throw new Error(message);
}

function infiniteLoop(): never {
  while(true){
    /* 기능 */
  }
}

// 타입 별칭
let x: number = 10;
let xPositina: number = 10;

type YesOrNo = string;
type YesOrNoDetail = "Y" | "N";

let sayMe: YesOrNo = "HI";
let sayYou: YesOrNoDetail = "Y"

// 인자가 없고 리턴 값이 string 타입인 type 지정
type FooFunction = () => string;
let temp: FooFunction = () => {
  return "temp"
}

// interface

type Name = "AYW";

interface IUser{
  id: number;
  name: Name;
  email: string;
  age: number;
}

const myInfo: IUser = {
    id: 1,
    name: "AYW",
    email: "any",
    age: 27
}

// interface는 속성 값끼리 합칠 수 있다.
interface IUser{
  id: number;
  name: Name;
  email: string;
  age: number;
}

interface IUser {address: string}

// type 별칭은 불가능하다.
type IUser{
  id: number;
  name: Name;
  email: string;
  age: number;
}

type IUser {address: string}
👉🏽 Error. Duplicate identifier 'IUser'.

// keyof: 타입에 있는 속성값들을 하나의 타입으로 묶는다.
interface User {
    id: number;
    name: string;
    age: number;
    gender: "male" | "female";
}

type UserKey = keyof User;
// 'id' | 'name' | 'age' | 'gender'

const uk: UserKey = "name"
console.log(uk)
```

### ❏ type utility 알아보기

1. `typescript`는 일반적인 타입 변환을 쉽게 하기 위해서 몇 가지 유틸리티 타입을 제공합니다. 이러한 유틸리티는 전역으로 사용 가능합니다.

```typescript

// Partial<T>: type 집합의 모든 프로퍼티를 선택적으로 타입을 생성한다.
// Partial 대신 ?를 써도 된다.
interface User {
    id: number;
    name: string;
    age: number;
    gender: 'male' | 'female'
}

let admin: Partial<User> = {
    id: 1,
    name: "AYW",
}

console.log(admin);

// Readonly<T>: 처음 설정한 값외에 속성을 수정 할 수 없다. 재할당 금지
interface User {
    id: number;
    name: string;
    age: number;
    gender: 'male' | 'female'
}

let admin: Readonly<User> = {
    id: 1,
    name: "AYW",
    age: 27,
    gender: "male"
}

admin.id = 3;
console.log(admin)

👉🏽 Cannot assign to 'id' because it is a read-only property.

// Readonly
interface User {
    id: number;
    name: string;
    age: number;
    readonly gender: 'male' | 'female'
}

let admin: User = {
    id: 1,
    name: "AYW",
    age: 27,
    gender: "male"
}

admin.id = 3;
admin.gender = "female";  // error
console.log(admin)
👉🏽 Cannot assign to 'gender' because it is a read-only property.

// Record<K, T>: 개체의 속성과 타입을 정의할 때 사용하는 메소드
type Grade = "1" | "2" | "3" | "4";
type Score = "A" | "B" | "C" | "D";

const score: Record<Grade, Score> = {
    1: "A",
    2: "B",
    3: "C",
    4: "D",
}

console.log(score)

// Record<K, T>: 타입의 프로퍼티 키의 집합으로 타입을 생성한다. 개체의 속성과 타입을 정의할 때 사용하는 메소드
interface User {
    id: number;
    name: string;
    age: number;
}

function isValid(user: User){
    const result: Record<keyof User, boolean> = {
        id: user.id > 0,
        name: user.name !== '',
        age: user.age > 0,
    }
    return result;
}

// Pick<T, K>: Type에서의 Key값을 선택하여 새로 type으로 정하는 기능
interface User {
    id: number;
    name: string;
    age: number;
    gender: "male" | "female";
}

const admin: Pick<User, "id"|"name"> = {
    id : 0,
    name: "TED"
}

console.log(admin)

// Omit<T, K>: Type에서의 Key값을 선택하여 사용하지 못하게 한다.
interface User {
    id: number;
    name: string;
    age: number;
    gender: "male" | "female";
}

const admin: Omit<User, "id"|"name"> = {
    age: 27,
    gender: "male"
}

console.log(admin)

// Exclude<T1, U>: 속성 대신 Type의 key 값을 제외한다.
type T1 = string | number | boolean;
type T2 = Exclude<T1, number | string>;

let isNum: T2 = 3;
👉🏽 Type 'number' is not assignable to type 'T2'.

let isNum: T2 = true;

// NonNullable<T>: undefined와 null 타입을 제거한다.
type T1 = string | null | undefined | void;
type T2 = NonNullable<T1>;

let empty: T2 = null;
👉🏽 Type 'null' is not assignable to type 'T2'.
let empty: T2 = "Hi";

// Parameters<T>: 함수 타입을 인자로 받아서 튜플타입으로 리턴해주는 문법
type T0 = Parameters<() => string>;  // []
type T1 = Parameters<(s: string) => void>;  // [string]
type T2 = Parameters<(s: string, i: number) => number>

let T1Arr: T1 = ["123"];

// ReturnType<T>: return type값을 정의하는 문법
type T0 = ReturnType<() => string>;

function returnString(): T0{
    return "123"
}

type T7 = ReturnType<any> // any
type T8 = ReturnType<never> // any

// Required<T>: partial과 반대되는 기능으로 type집합의 모든 프로퍼티를 필수로 설정한다.
interface User {
    id: number;
    name?: string
}

let admin: Required<User> = {
    id: 1,
}

👉🏽 Property 'name' is missing in type '{ id: number; }' but required in type 'Required<User>'.

let admin: Required<User> = {
    id: 1,
		name: "AYW"
}
```

### ❏ 타입스크립트의 함수

1. 일급객체(first-class object): 함수를 변수로 선언하고, 함수에 인자를 함수로 넘길 수 있고, 함수의 리턴값을 함수로 설정할 수 있는 것을 일급객체라 부릅니다. `JS` 와 `TS` 는 모두 일급객체입니다.
2. 일급객체의 특징 때문에 고차함수, 콜백함수를 만들 수 있다.

```ts
// 함수 자체를 값으로 저장한다.
let sum = function (a, b) {
    return a + b;
};

function ul(child) {
    return `<ul>${child}</ul>`;
}

// 함수를 리턴할 수 있다.
function makeLi(container, contents) {
    const liList = [];

    for (const content of contents) {
        liList.push(`<li>${content}</li>`);
    }

    return container(liList.join(""));
}

// 함수를 함수의 인자로 넣어줄 수 있다.
const htmlUl = makeLi(ul, ["월", "화", "수", "목", "금", "토", "일"]);
```

3. 함수의 선언문, 선언식

```ts
// 함수 선언문
function sum(a, b) {
    return a + b;
}

// 함수 표현식
const myFunc = function (a, b) {
    return a + b;
};
```

4. 함수의 가변인자

```ts
function sum(a, b) {
    return a + b;
}

const abcSum = sum(10, 20, 30);

// 가변 인자식
function sum() {
    let s = 0;
    for (let i = 0; i < arguments.length; i++) {
        s += arguments[i];
    }
    return s;
}

// arguments
function sum(...args) {
    let s = 0;
    for (let i = 0; i < args.length; i++) {
        s += args[i];
    }
    return s;
}
```

4. 함수 호출

```ts
// call과 apply는 인자를 하나씩 넘겨주냐 배열로 넘겨주냐의 차이
sum(10, 20, 30, 40);
// 컨텍스트 null
sum.call(null, 10, 20, 30, 40);

arr = [10, 20, 30, 40];
sum.apply(null, arr);
```

5. 함수의 종류

```ts
// 즉시 실행 함수
(function () {
    console.log(123);
});

// 일반함수와 화살표함수의 차이:  컨텍스트의 차이점
const sumV2 = (a, b, ...args) => {};

const ten = () => 100;
const hundred = (x) => 100 + x;

// 생성기 함수(generate function): 함수를 한번에 실행시키는 것이 아니라 텀을 두고 실행할 때
function* gen() {
    yield 10;
    yield 20;
    return 30;
}

const g = gen();

console.log(g.next()); // 10
console.log(g.next()); // 20
console.log(g.next()); // 30
```

6. 함수 작성시 반환 타입 명시 권장(필수는 아님, `TS` 컴파일러는 방정식의 한쪽에만 타입이 있더라도 타입을 추론할 수 있다.)
7. 매개변수와 인수의 타입이 호환 가능하게 작성, 인수 타입의 전달이 잘못된 경우 오류 발생

```ts
// 함수를 안전하게 만들 수 있다.
interface MathFn {
    (a: number, b: number): number;
    operator: string;
};

const sum: MathFn = (a, b) => a + b;
sum.operator = "+";

1. void: 반환값이 없는 함수입니다. (그냥 출력하거나, 상태를 바꿀 때 자주 씁니다.)
2. never: 함수가 종료되지 않습니다. (무한루프를 돌거나, Error를 띄울 때 사용합니다.)
```

8. 함수의 매개변수: 함수에 주어진 인자의 개수는 함수가 기대하는 매개변수의 수와 일치해야 함

```ts
function sum(a: number, b:number, type?: string): number{
    return a+b;
}

let sumAge = sum(2, 3, "ted");

function buildName(firstName: string, lastName="Smith") {
    return firstName + ' ' + lastName;
}

let result1 = buildName("Bob");
let result2 = buildName("Bob", undefined);
let result3 = buildName("Bob", 'Ted');
console.log(result1)
👉🏽 "Bob Smith"


[LOG]: "Bob Smith"
[LOG]: "Bob Ted"

console.log(result2)
console.log(result3)

undefined가 넘어가면 lastName이 없다고 판단되지만, null이 들어가면 lastName이 있다고 판단을 합니다.
(undefined는 값 자체가 없다고 판단하나, null은 값은 있는데 의미없는 특별한 값이 들어있다고 보시면 좋을 것 같아요.)
+ undefined는 미리 선언된 global variable이나, null은 키워드입니다.
```

### ❏ 객체 지향 프로그래밍(OOP)

1. `OOP` 는 컴퓨터 프로그램을 객체의 모임으로 파악하려는 프로그래밍 패러다임
2. 프로그램을 유연하고, 변경이 용이하고, 개발과 보수를 간편하게 만든다, 직관적인 코드 분석이 가능해진다.
3. 클래스 요소: 필드(field), 생성자(constructor, 객체가 처음 생성될 때 호출, 멤버 변수 초기화), 메소드(method)
4. 인스턴스: `new` 연산자에 의해서 생성된 객체

```ts
class Person {
    name: string;
    constructor(name: string) {
        this.name = name;
    }
    say() {
        return `Hello, ${this.name}!`;
    }
}

let person = new Person("AYW");
console.log(person.say());
```

### ❏ 클래스 만들기

1. 생성자의 매개변수에 `public` 과 같은 접근 제한자를 붙이면 해당 매개변수의 이름을 가진 속성이 클래스에 선언된 것처럼 동작합니다.

```ts
// public 접근 제한자
class Information {
  constructor(public name: string, public age: number){}
}

const myInfo = new Information("AYW", 27);
console.log(myInfo)
👉🏽 { name: 'AYW', age: 27 }

// this
class Information {
    name: string;
    age: number
  constructor(name: string, age: number){
    this.name = name;
    this.age = age;
  }
}

const myInfo = new Information("AYW", 27);
console.log(myInfo)
👉🏽 { name: 'AYW', age: 27 }
```

### ❏ 클래스 상속받기

1. 부모 클래스를 상속받는 키워드: `extends`

```ts
class AYW extends Information{
  constructor(public name: string, public age: number, gender: "male" | "female"){
    super(name, age)
  }

  sayHello(): void {
    console.log(`제 이름은 ${this.name}입니다.`)
  }
}

const myInfo: AYW = new AYW("AYW", 27, "male")
console.log(myInfo);
👉🏽 AYW { name: 'AYW', age: 27 }

myInfo.sayHello();
👉🏽 제 이름은 AYW입니다.
```

### ❏ 추상 클래스

1. 추상 클래스는 자신의 속성이나 메서드 앞에 `abstract`를 붙여 나를 상속하는 다른 클래스에서 이 속성이나 메서드를 구현하게 합니다.

```ts
abstract class Information {
    name: string;
    age: number;
    constructor(name: string, age: number) {
        this.name = name;
        this.age = age;
    }

    abstract sayHello(): void;
}

class AYW extends Information {
    constructor(
        public name: string,
        public age: number,
        gender: "male" | "female"
    ) {
        super(name, age);
    }

    sayHello(): void {
        console.log(`제 이름은 ${this.name}입니다.`);
    }
}

const myInfo: AYW = new AYW("AYW", 27, "male");
console.log(myInfo);
👉🏽 AYW { name: 'AYW', age: 27 }

myInfo.sayHello();
👉🏽 제 이름은 AYW입니다.
```

---

## 📍 22일차 11.24.수.(온라인 강의)

오늘은 어제 배웠던 내용을 강의를 통해 다시 한번 배우는 시간을 가졌다. 클린코드, 타입스크립트 정의, `type`, `utility` 등등에 대해서 다시 배워보자.

### ❏ 클린코드란

1. 클린 코드란 말 그대로 깨끗하게 작성된 코드를 의미합니다. 깨끗하게 작성된 코드란 직접적이고 단순하여 읽기가 쉽고, 코드 작성자가 아닌 누가 보더라도 의도가 명확히 드러나는 코드입니다. 이러한 코드는 가독성이 좋고, 의존성을 최대한 줄여 유지보수가 쉬운 특징이 있습니다.
2. 프로그래머는 작성 기한을 맞추기 위해서 나쁜 코드를 양산할 수밖에 없다고 생각합니다. 하지만 나쁜 코드를 양산하면 결국 기한을 맞추지 못합니다. 오히려 엉망진창인 코드 때문에 개발 속도가 느려지고 결국 기한을 놓칩니다. 기한을 맞추는 유일한 방법은 언제나 코드를 최대한 깨끗하게 유지하는 것입니다.

### ❏ 클린코드와 타입스크립트

1. 자바스크립트는 타입이 없기 때문에 실행 후에 타입 에러를 확인할 수 있습니다. 반면 타입스크립트는 같은 코드에 대해 아래와 같이 실행을 하기 전에, 미리 에러를 확인할 수 있습니다. 자바스크립트의 런타임 단계에서 발생하는 타입 에러를 타입스크립트에서는 컴파일 단계에서 미리 확인하고 고칠 수 있다. 만약, 런타임 단계에서 발생하는 에러로 인해 프로그램이 멈추면, 운영되는 서비스에 큰 차질이 생길 수 있다. 타입스크립트를 사용하면 에러를 미리 방지할 수 있다.
2. 타입을 정의함으로써 개발자의 실수를 줄일 수 있고, 명시된 타입을 보고 해당 변수의 자료형이 무엇인지 쉽게 이해할 수 있다. 결과적으로 어던 용도로 코드가 작성되었고, 무엇을 의미하는지 파악하기 훨씬 용이하기 때문에 유지보수에 유리하고 자연스럽게 개발 속도도 빨라지게 된다.

### ❏ 타입스크립트란?

1. `microsoft` 에서 개발한 오픈 소스 언어
2. 자바스크립트의 상위 집합, JS의 한계를 해결
3. 타입스크립트를 실행하려면 자바스크립트로 변환하는 컴파일과정이 필요하다.
4. 동적타입을 정적으로 사용가능
5. 타입 유추로 타입 제어 가능
6. 컴파일 시점에 오류 포착 가능
7. JS에서 찾을 수 없는 추가코드 기능 제공

```typescript
// JS
let a;
a = 1;
a = "b";

const sum = (a, b) => {
    return a + b;
};

sum(1, "2"); // 12

// TS
let a: number;
a = 1;
b = "b"; // Error(컴파일 시점)

const sum = (a: number, b: number) => {
    return a + b;
};

sum(1, 2); // 12
```

### ❏ 타입스크립트의 기본 Type

1. JS코드에 변수 함수 등의 type 정의 가능
2. 타입 표기(type annotation)을 사용한다.
3. 기본자료형(primitive type): `string`, `boolean`, `number`, `null`, `undefined`, `symbol(ES6)`

```typescript
// string
let str: string = "hi";

// boolean
let isSucceeded: boolean = true;

// number: 2진수, 8진수, 10진수, 16진수 사용 가능
let decimal: number = 6;
let hex: number = 0xf00d;
let binary: number = 0b1010;
let octal: number = 0o744;

console.log(decimal, hex, binary, octal); // 6 61453 10 484

// null
let n: null = null;

// undefined
let u: undefined = undefined;
```

4. 참조자료형(reference type): object, array, function

```typescript
// 객체, 배열, 함수 등과 같은 Object 형식의 타입, 메모리에 값을 주소로 저장하고, 출력시 메모리 주소와 일치하는 값을 출력
// object
function create(o: object): void {}

create({ prop: 0 }); // object
create([1, 2, 3]); // array
create("string"); // error
create(false); // error
create(42); // error

// array
let arr1: number[] = [1, 2, 3];
let arr2: Array<number> = [1, 2, 33];
```

5. 추가 제공 자료형: tuple, enum, any, void, never

```typescript
// tuple: 길이와 각 요소의 타입이 정해진 배열을 저장하는 타입
let arr: [string, number] = ["Hi", 122];
arr[1].concat("1")  // Error: 'number' does not have 'concat'
arr[3] = "hello"  // Error: Property '3' does not exist on type [string, number]

// enum: 특정 값들의 집합을 저장하는 타입
enum Car {BUS, TAXI, SUV};
let bus: Car = Car.BUS;
let taxi: string = Car[2];

console.log(bus, taxi)
👉🏽 0 "SUV"

enum Car {BUS = 2, TAXI, SUV};
let bus: Car = Car.BUS;
let taxi: string = Car[3];

console.log(bus, taxi)
👉🏽 2 "TAXI"

// any: 모든 타입 저장 가능, 컴파일 중 타입 검사를 하지 않음
let str: any = "hi";
let num: any = 1;
let arr: any = [1, 2, 3];

// void: 보통 함수에서 반환 값이 없을 때 설정하는 타입
let unknown: void = undefined;
function sayHi(): void {
  console.log("hi")
}

// never: 절대 발생할 수 없는 타입, 종료되지 않는 함수, 항상 오류를 발생시키는 함수
function neverEnd():never {
  while(true){}
}

function neverEnd():never {  // Error: A function returning 'never' cannot have a reachable end point.
  while(true){break}
}

function error(message: string):never{
  throw new Error(message)
}
```

### ❏ 타입스크립트의 Utility

1. Typescript는 공통 타입 변환을 용이하게 하기 위해 유틸리티 타입을 제공한다.
2. 유틸리티 타입은 전역으로 사용 가능하다
3. `Partial<T>`, `Readonly<T>`, `Record<T>`, `Pick<T, K>`, `Omit<T, K>`, `Exclude<T, U>`. `Extract<T, U>`, `NonNullable<T>`, `Parameters<T>` , `ConstructorParameters<T>`, `ReturnType<T>`, `Required<T>`
4. 제네릭이란 어떤 함수나 클래스가 사용할 타입을 생성 단계가 아닌 사용 단계에서 정의하는 프로그래밍 기법입니다.

```typescript
// Partial<T>: 프로퍼티를 선택적으로 만드는 타입을 구성한다.
interface Todo {
  title: string;
  description: string;
}

function updateTodo(todo: Todo, fieldsToUpdate: Partial<Todo>){
  return {...todo, ...fieldsToUpdate}
}

const todo1: Todo = {
  title: 'organize desk',
  description: 'clear clutter'
}

const todo2 = updateTodo(todo1, {description: 'throw out trash'})

console.log(todo1, todo2)
👉🏽 { title: 'organize desk', description: 'clear clutter' } { title: 'organize desk', description: 'throw out trash' }

// Readonly<T>: 프로퍼티를 읽기 전용으로 설정한다.
interface Todo {
  title: string;
}

const todo1: Readonly<Todo> = {
  title: 'organize desk',
}

todo1.title = "Hello" // Error: Cannot assign to 'title' because it is a read-only property.

// Record<T>: 프로퍼티의 집합 K로 타입을 구성한다. 타입의 프로퍼티들을 다른 타입에 매핑시키는데 사용한다.
interface PageInfo {
  title: string;
}

type Page = "home" | "about" | "contact";

const x: Record<Page, PageInfo> = {
  about: {title: 'about'},
  contact: {title: 'contact'},
  home: {subTitle: 'home'}  // Error: Type '{ subTitle: string; }' is not assignable to type 'PageInfo'.  Object literal may only specify known properties, and 'subTitle' does not exist in type 'PageInfo'
}

// Pick<T, K>: 프로퍼티 K의 집합을 선택해 타입을 구성한다.
interface Todo {
  title: string;
  description: string;
  completed: boolean
}

type TodoPreview = Pick<Todo, "title" | "completed">;

const todo: TodoPreview = {
  title: 'clean room',
  completed: true,
  description: 'desc'  // Error: Type '{ title: string; completed: true; description: string; }' is not assignable to type 'TodoPreview'. Object literal may only specify known properties, and 'description' does not exist in type 'TodoPreview'
}

// Omit<T, K>: 모든 프로퍼티를 선택한 다음 K를 제거한 타입을 구성한다.
interface Todo {
  title: string;
  description: string;
  completed: boolean
}

type TodoPreview = Omit<Todo, "description">;

const todo: TodoPreview = {
  title: 'clean room',
  completed: true,
  description: 'desc'  // Error: Type '{ title: string; completed: true; description: string; }' is not assignable to type 'TodoPreview'.
}

// Exclude<T, U> : 타입 T에서 U와 겹치는 타입을 제외한 타입을 구성합니다.
// Extract<T, U> : 타입 T에서 U와 겹치는 타입만 포함하여 타입을 구성합니다.
// NonNllable<T> : T 타입에서 null과 undefined를 제외한 타입을 구성합니다.
// Parameter<T> : 함수 타입 T의 매개변수의 타입들의 튜플로 타입을 구성합니다.
// ConstructorParameters<T> : 클래스의 생성자를 비롯한 생성자 타입의 모든 매개변수 타입을 추출합니다.
// ReturnType<T> : 함수 T가 반환한 타입으로 타입을 구성합니다.
// Required<T> : 타입 T의 모든 프로퍼티가 필수로 설정된 타입을 구성합니다.
```

### ❏ 함수 사용하기

1. 함수를 정의 할 때 사용되는 변수는 매개변수이고 호출 할 때 사용되는 값은 인수라고 한다.

```typescript
function add(x, y) {
    // 매개변수
    return x + y;
}

add(2, 5); // 인수
```

2. 일급객체(first-class object): 다른 객체들에 일반적으로 적용 가능한 연산을 모두 지원하는 객체

```typescript
1. 다른 함수에 매개변수로 제공할 수 있다.
2. 함수에서 반환이 가능하다
3. 변수에 함수를 할당할 수 있다.
```

3. 함수 선언식, 함수 표현식

```typescript
// 함수 선언식
function world(name) {}

// 함수 표현식
const hi = function (name) {};

// 함수 생성자는 되도록 사용을 권하지 않는다
let world5 = new Function();
```

4. `TS` 에서 함수 작성시 반환 타입을 추론하도록 하는걸 권장한다.
5. `TS` 컴파일러는 방정식의 한쪽에만 타입이 있어도 타입추론이 가능한데, 이를 `contextual typing` 이라고 부른다. 이를 통해 프로그램에서 타입을 유지하기 위한 노력을 줄일 수 있다.

### ❏ 함수의 매개변수

1. 기본 매개변수: 함수에 주어진 인자의 수는 함수가 기대하는 매개변수의 수와 일치해야 한다.

```typescript
function buildName(firstName: string, lastName: string) {
    return firstName + lastName;
}

let result1 = buildName("a", "b");
let result2 = buildName("a", "b", "c"); // Error: Expected 2 arguments, but got 3.
```

2. 선택적 매개변수: `JS` 에서는 인수가 없으면 `undefined` 로 선언이된다. `TS` 에서는 변수명 뒤에 `?` 를 사용하면 변수를 선택적으로 사용할 수 있다.
3. 기본-초기화 매개변수: `TS` 에서 값을 제공하지 않거나, `undefined` 로 했을 때 매개변수의 값 할당 가능

```typescript
function buildName(firstName: string, lastName: string = "TED") {
    return firstName + lastName;
}

let result1 = buildName("a"); // aTED
let result1 = buildName("a", undefined); // aTED
let result1 = buildName("a", "morning"); // amorning
```

4. 나머지 매개변수: `...` 을 넣어주어 매개변수의 수를 무한으로 취급할 수 있다. 아무것도 넘겨주지 않으면 `[]` 이 할당된다.

```typescript
function buildName(firstName: string, ...lastName: string[]) {
    return firstName + lastName;
}

let result1 = buildName("a", "SON", "Ted"); // aSON,Ted
```

### ❏ OOP

1. 객체 지향 프로그래밍: 컴퓨터 프로그램을 객체의 모임으로 파악하려는 프로그래밍 패러다임이다. 객체들은 서로 메세지를 주고 받으며 데이터를 처리할 수 있다.
2. 장점: 프로그램을 유연하고, 변경이 용이하게 만들어지며, 개발과 보수를 간편하게 만든다, 직관적인 코드 분석을 가능하게 한다.
3. 중요한 특성: 강한 응집력과 약한 결합력을 지향한다.

### ❏ Class

1. 클래스의 요소: 멤버, 필드, 생성자, 메소드
2. 인스턴스: `new` 연산자에 의해 생성된 객체

```typescript
class Person {
    name: string;
    constructor(name: string) {
        this.name = name;
    }

    say() {
        return "Hello, My name is " + this.name;
    }
}

let person = new Person("TED");
console.log(person); // Person { name: 'TED' }
```

### ❏ Class 접근 제어자

1. 속성, 메소드로의 접근을 제한하기 위해 사용한다.
2. `public`, `protected`, `private`
3. `Java` 와 다르게 `package` 개념이 없어 `default` 접근 제어자는 없다.
4. `public`: 프로그램 내 선언된 멤버들이 자유롭게 접근할 수 있다. 기본적으로 `public` 으로 선언된다. 명시적으로 `public` 선언도 가능하다.

```typescript
class Person {
    public name: string;
    constructor(name: string) {
        this.name = name;
    }
}

let a = new Person("TED").name;
console.log(a); // TED
```

5. `private` :멤버가 포함된 클래스 외부에서 접근을 막는다.

```typescript
class Person {
    private name: string;
    constructor(name: string) {
        this.name = name;
    }
}

new Person("TED").name; // Error: Property 'name' is private and only accessible within class 'Person'.
```

6. `protected`: 멤버가 포함될 클래스와 그 하위 클래스 외부에서의 접근을 막는다. (내부에서는 접근이 가능하지만, 외부에서의 접근은 불가하다)

```typescript
class Person {
    protected name: string;
    constructor(name: string) {
        this.name = name;
    }
}

class Employee extends Person {
    private department: string;

    constructor(name: string, department: string) {
        super(name);
        this.department = department;
    }

    public getElevatorPitch() {
        return `good.`;
    }
}

let howard = new Employee("Howard", "sales");
console.log(howard.name); // Error: Property 'name' is protected and only accessible within class 'Person' and its subclasses.
```

### ❏ Class 상속

1. 상속을 이용하여 존재하는 클래스를 확장해 새로운 클래스를 생성할 수 있다. `extends`
2. 파생된 클래스는 하위클래스(subclass), 기초 클래스는 상위 클래스(super class)라고 부른다.

```typescript
class Animal {
    move(distanceInMeters: number) {
        console.log(`Animal moved ${distanceInMeters}m.`);
    }
}

class Dog extends Animal {
    makeSound() {
        console.log(`멍멍`);
    }
}

const dog = new Dog();
dog.move(10);
```

### ❏ Getters & Setters

1. 비공개로 설정하려는 속성은 `private` 로 설정하고, 속성값을 읽고 수정하는 `getter/setter` 함수를 사용한다.
2. `class` 에 직접 적용하는것을 막고, 함수를 사용해 값을 받아오거나 수정한다. 속성에 직접 접근해 수정하면 데이터 무결성이 깨질 수 있다. (캡슐화 권장)
3. 각 객체의 멤버에 접근하는 방법을 세밀하게 제어할 수 있다.

```typescript
class Person {
    private _name: string;

    get name() {
        return this._name;
    }

    set name(name: string) {
        if (name.length > 10) {
            throw new Error("name too long");
        }
        this._name = name;
    }
}

let person = new Person();
console.log(person.name); // undefined

person.name = "TED";
console.log(person.name); // TED

person.name = "TEDTEDTEDTEDTED"; // throw Error
```

### ❏ Readonly

1. 읽기만 가능한 속성을 선언하기 위해 사용한다. (변경 할 수 없다.)
2. 선언될 때나 생성자에서 값을 설정하면 이후 수정할 수 없다.

```typescript
class Person {
    readonly age: number = 20;
    constructor(age: number) {
        this.age = age;
    }
}

let person = new Person(10);
person.age = 30; // Error: Cannot assign to 'age' because it is a read-only property
```

### ❏ static

1. 전역 멤버를 선언할 때 사용한다. (전역멤버: 객체마다 할당되지 않고, 클래스의 모든 객체가 공유하는 멤버)
2. 인스턴스가 아닌 클래스 자체에서 보이는 전역 멤버를 생성한다.
3. 범용적으로 사용되는 값에 설정한다.
4. `클래스명.` 을 앞에 붙여 `static` 멤버에 접근할 수 있다.
5. `ES6` 에서 메소드 전용 속성에는 선언이 안되었으나, `TS` 에서는 사용가능하다.

```typescript
class Grid {
    static origin = { x: 0, y: 0 };
    calculateDistanceFromOrigin(point: { x: number; y: number }) {
        let xDist = point.x - Grid.origin.x;
        let yDist = point.y - Grid.origin.y;
        return Math.sqrt(xDist * xDist + yDist * yDist) / this.scale;
    }
    constructor(public scale: number) {}
}

let grid1 = new Grid(1.0); // 1x scale
let grid2 = new Grid(5.0); // 5x scale

console.log(grid1.calculateDistanceFromOrigin({ x: 10, y: 10 })); // 14.142135623730951
console.log(grid2.calculateDistanceFromOrigin({ x: 10, y: 10 })); // 2.8284271247461903
```

### ❏ 추상클래스

1. 다른 클래스들이 파생될 수 있는 기초클래스
2. 직접 인스턴스화 될 수 없다.
3. `abstract` 키워드는 추상 클래스나 추상 메소드를 정의하는데 사용된다.
4. 추상 메소드는 클래스에는 구현되어 있지 않고, 파생된 자식 클래스에서 구현해야 한다.

```typescript
abstract class Animal {
    protected name: string;

    constructor(name: string) {
        this.name = name;
    }

    abstract makeSound(): void;
    move(): void {
        console.log("move !!");
    }
}

class Dog extends Animal {
    constructor(name: string) {
        super(name); // 파생된 클래스의 생성자는 반드시 super()를 호출
    }

    makeSound(): void {
        console.log(this.name + "멍멍");
    }
}

const animal = new Animal("animal"); // Error: Cannot create an instance of an abstract class.
const dog = new Dog("진돗개"); // Dog { name: '진돗개' }
```

### 💡 추상 클래스를 활용한 디자인 패턴

1. 프로그램의 일부분을 서브 클래스로 캡슐화해 전체 구조를 바꾸지 않고 특정 단계의 기능을 바꾸는 것
2. 전체적인 알고리즘은 상위 클래스에서 구현하고, 다른 부분은 하위 클래스에서 구현한다.
3. 전체 구조는 유사하지만, 부분적으로 다른 구문에서 작성된 메소드의 코드 중복을 최소화 할 수 있다.

```typescript
abstract class Parent {
  public do(){
    console.log("Parent에서 실행 - 상") ;
    this.hook();
    console.log("Parent에서 실행 - 하");
  }

  abstract hook(): void;
}

class Child extends Parent {
  hook(): void {
    console.log("child")
  }
}

const child = new Child();
child.do();

👉🏽
Parent에서 실행 - 상
child
Parent에서 실행 - 하
```

---

## 📍 23일차 11.25.목(실시간 강의)

오늘은 `interface`, `generic` 문법에 대해서 배웠다.

### ❏ Interface

1. 타입 체크를 위해 사용되며 변수, 함수, 클래스에 사용 가능
2. 직접 인스턴스를 생성할 수 없음. 모든 메소드는 추상 메소드다. (이때 `abstract` 키워드를 사용하지 않는다)
3. 선언만 존재한다. (JS로 변환되면 인터페이서는 사라진다.)
4. `interface` 간에 `extends` 를 사용하여 다중 상속 가능(class와 비슷)
5. 추상 클래스와 다른점: 추상 `class`는 전체적인 구조, `interface`는 프로그래머 간의 협업 개발을 할 때 사용
6. 함수의 매개변수(파라미터로)로 사용
7. `API` 응답에서 데이터의 구조를 결정할 때 사용

```typescript
// 키 값을 다음처럼 정해주면 키 값은 제한이 없다.
interface User {
    [grade: number]: "A" | "B" | "C" | "D";
}

let user: User = {
    1: "A",
    2: "B",
    5: "D",
};
```

8. 선택적 프로퍼티(?): `?`가 붙는 경우는 반드시 구현되지 않고 선택가능

```typescript
// 키 값을 다음처럼 정해주면 키 값은 제한이 없다.
interface User {
    1: string;
    2?: string;
    5: string;
}

let user: User = {
    1: "A",
    5: "D",
};
```

9. 클래스 선언문의 `implements` 를 붙여서 사용 가능(인터페이스를 구현하는 클래스의 일관성을 유지할 수 있는 장점을 가짐)

```typescript
// 모든 메소드는 추상 메소드여야 한다.
// 인터페이스에서 정의한 타입은 클래스 안에서도 모두 적용해야한다.
interface ITodo {
    id: number;
    content: string;
    completed: boolean;
    sayHello(): void;
}

class Todo implements ITodo {
    constructor(
        public id: number,
        public content: string,
        public completed: boolean
    ) {}

    sayHello() {
        console.log(`안녕하세요!!`);
    }
}

const today = new Todo(1, "TED", true); // 인스턴스
console.log(today); // Todo { id: 1, content: 'TED', completed: true }
today.sayHello(); // 안녕하세요!!
```

9. 함수와 변수에서도 덕타입이 적용된다.(덕 타이핑: 타입 체크에서 중요한 것은 값을 실제 가지고 있느냐에 관한 것, 인터페이스에서 정의한 프로퍼티나 메소드를 가지고 있다면 그 인터페이스를 구현한 것으로 여김 덕 타이핑 또는 구조적타이핑이라 부름)

```typescript
type IPerson = {
    name: string;
};

function sayHello(person: IPerson): void {
    console.log(`Hello ${person.name}`);
}

const me = { name: "TED", age: 27 };
sayHello(me);
```

### ❏ 디자인패턴

1. 생성패턴: 객체를 생성하는데 관련한 패턴
2. 구조패턴: 프로그램의 구조에 관련한 패턴
3. 행위패턴: 반복적으로 사용되는 객체들의 상호작용 패턴

```typescript
// 전략 패턴
interface Weapon {
    attack: () => void;
}

class Sword implements Weapon {
    public attack() {
        console.log("검 공격");
    }
}

class Spear implements Weapon {
    public attack() {
        console.log("창 공격");
    }
}

class Bow implements Weapon {
    public attack() {
        console.log("활 공격");
    }
}

class GameUser {
    private weapon: Weapon | null = null;

    public setWeapon(weapon: Weapon) {
        this.weapon = weapon;
    }

    public attack() {
        if (this.weapon === null) {
            console.log("맨손 공격");
        } else {
            this.weapon.attack();
        }
    }
}

const testUser = new GameUser();
testUser.setWeapon(new Spear());
testUser.attack(); // 창

testUser.setWeapon(new Bow());
testUser.attack(); // 활 공격

testUser.setWeapon(new Sword());
testUser.attack(); // 검 공격

testUser.setWeapon(null);
testUser.attack(); // 맨손 공격
```

### ❏ 제네릭(Generic)

1. 데이터타입을 일반화 함
2. 자료형을 정하지 않고 여러 타입을 사용할 수 있게 한다.(범용적인 함수를 쓰고 싶을 때?, 여러가지 타입을 사용하고 싶을 때)
3. 재사용성이 높은 함수를 만들어줄때 사용됨
4. 한가지 타입보다 여러가지 타입에서 동작하는 함수를 생성한다.

```typescript
// class 문법에서의 제네릭
class Stack<T> {
    private data: T[] = [];

    constructor() {}

    push(item: T): void {
        this.data.push(item);
    }

    pop(): T | undefined {
        return this.data.pop();
    }
}

// 인스턴스의 타입을 유연하게 설정할 수 있다.
const numberStack = new Stack<number>();
const stringStack = new Stack<string>();
numberStack.push(1);
stringStack.push("a");

// 함수에서의 제네릭
function getSize<T>(arr: T[]): number {
    return arr.length;
}

const arr1 = [1, 2, 3];
getSize<number>(arr1);

const arr2 = ["a", "b", "c"];
getSize<string>(arr2);
```

5. 제네릭한 변수를 추가하고 싶을 때 `<T, U>`

```typescript
// 1
function toPair<T, U>(a: T, b: U): [T, U] {
    return [a, b];
}

toPair<number, string>(1, "1");
toPair<string, boolean>("Hello", true);

// 2
function logText<T>(text: T[]): number {
    return text.length;
}

// 3
interface Mobile<T> {
    name: string;
    price: number;
    option: T;
}

let myInfo: Mobile<boolean> = {
    name: "TED",
    price: 6000,
    option: true,
};

let yourInfo: Mobile<object> = {
    name: "TED",
    price: 6000,
    option: {
        age: 28,
        color: "orange",
    },
};

// 함수에서의 제네릭
// <T>는 text의 인자는 T로 받고 리턴값도 T 타입으로 해준다.
interface GenericLogTextFn {
    <T>(text: T): T;
}

interface GenericLogTextFn<T> {
    (text: T): T;
}

function logText<T>(text: T): T {
    return text;
}

let myString: GenericLogTextFn<string> = logText;
console.log(myString);

interface Mobile<T> {
    name: string;
    price: number;
    option: T;
}

interface OptionType {
    color: string;
    coupon: boolean;
}

const m1: Mobile<OptionType> = {
    name: "s21",
    price: 1000,
    option: { color: "red", coupon: false },
};

// 제네릭 상속
interface User {
    name: string;
    age: number;
}

interface Book {
    price: number;
}

let user: User = { name: "a", age: 10 };
let book: Book = { price: 3000 };

function showName<T extends { name: string }>(data: T) {
    return data.name;
}
```

### ❏ Non-null assertion operator

1. `Null` 이 아닌 어선셜 연산자는 피연산자가 `null` 이 아니라고 컴파일러에게 전달하여 일시적으로 `Null` 제약조건을 완화합니다. 권장하지 않는 문법이고 대신 `&&` 을 사용한다.

### ❏ Union type

```typescript
// example1
function getAge(age: number | string) {
    return typeof age === "number" ? age.toFixed() : age;
}

const myAge = getAge(28);
console.log(myAge);

const yourAge = getAge("25");
console.log(yourAge);

// union 기호
interface Person {
    name: string;
    age: number;
}

interface Developer {
    name: string;
    skill: string;
}

// 겹치는 속성만 사용 가능
function introduce(someone: Person | Developer) {
    someone.name;
    someone.age; // Error
    someone.skill; // Error
}

// 모든 속성 사용 가능
function introduce(someone: Person & Developer) {
    someone.name;
    someone.age; // 사용 가능
    someone.skill; // 사용 가능
}
```

### ❏ 제약 조건(constraints / keyof)

1. 제네릭 타입에 어느정도 힌트를 주고 제약을 걸기 위해 사용, 최소한 `length` 속성이 있어야 에러가 나지 않는다

```typescript
interface LengthWise {
  length: number;
}

interface Rect {
  length: number;
  area: number;
}

function logText1<T extends LengthWise | Rect>(text: T){
  console.log(text.length);
  console.log(text.area);  // 공통되는 속성이 아니므로 Error가 난다.
}

function logText1<T extends LengthWise & Rect>(text: T){
  console.log(text.length);
  console.log(text.area);  // 모든 속성 사용 가능하므로 Error가 나지 않는다.
```

### ❏ keyof를 사용한 제약

1. 객체의 속성을 제약하고 싶을 때 사용

```typescript
// 객체 안에서의 속성만 사용하는 문법
function getProperty<T, O extends keyof T>(obj: T, key: O) {
    return obj[key];
}

let obj = { a: 1, b: 2, c: 3 };
// 'a' | 'b' | 'c'
console.log(getProperty(obj, "c"));
```

### ❏ 기타 기능 및 개념

1. Type Assertion: 타입 추론기능은 강력하지만 한계 존재, 타입단언(type assertion)은 타입스크립트가 추정하지 못하는 부분까지 개발자가 선언하는것
2. as

```typescript
let a;
a = 10;
a = "abc";
let b = a;

b = a as string;

interface Person {
    name: string;
    age: number;
}

interface Developer {
    name: string;
    skill: string;
}

function introduce(someone: Person | Developer) {
    someone.name;
    (someone as Person).age;
    (someone as Developer).skill;
}
```

3. typeGuard

```typescript
// 함수
function doSomeThing(id: string | number) {
    if (typeof id === "string") {
        console.log(id.trim());
    } else {
        console.log(id);
    }
}

// 클래스
class Diner {}
class Merchant {}

function doSomething(user: Diner | Merchant) {
    if (user instanceof Diner) {
    } else {
    }
}

// 메소드
interface Bird {
    fly(): string;
}

interface Fish {
    swim(): number;
}

function doSomething(animal: Fish | Bird) {
    if ("swim" in animal) {
        console.log((animal as Fish).swim());
    } else {
        console.log((animal as Bird).fly());
    }
}

doSomething({
    swim: () => {
        return 82;
    },
});

doSomething({
    fly: () => {
        return "Hello";
    },
});

// 타입 확인
function isFish(animal: Fish | Bird): animal is Fish {
    return (animal as Fish).swim !== undefined;
}

function doSomething(animal: Fish | Bird) {
    if (isFish(animal)) {
        animal.swim();
    } else {
        animal.fly();
    }
}
```

### ❏ 실습

1. 클래스 vs 추상클래스: 어떤 메서드는 그냥 구현해도 되고, 어떤 메서드는 정의 되지 않은 메서드 일 수 있다.(사용하려면 상속이 필요하다)
2. 인터페이스: 추상클래스와 달리 `abstract` 를 사용하지 않음. 구성되는 것의 타입만 명시해서(생성자나 메서드 구현을 작성할 필요가 없다.) (하나의 interface에 여러 데이터가 뭉치지 않도록 분산시킬 수 있기 때문에 다중상속이 가능하다.)
3. `interface` vs `type` vs `abstract`

```typescript
// 인터페이스: 상속이 가능하며, 다중 상속도 가능하다. 내부에서 메서드 구현을 할 수 없다.
interface Test {
	name: string;
	id: number;
	introduce(): void;
}

// 상속이 불가능하다. 내부에서 메서드 구현을 할 수 없다.
type Test {
	name: string;
	id: number;
	introduce(): void;
}

// 클래스이기 대문에 상속은 가능하지만, 다중 상속은 불가하다. 원하는 메서드는 구현을 할 수 있다.
abstract class Test {
	name: string;
	id: number;
  abstractintroduce(): void;
}
```

4. `T extends number | string` : 2개 이상 상속이 가능함.
5. `interface` 활용 예시: 데이터베이스 조작(로그인, 게시물, 등등)
6. ORM: SQL문을 대신해서 내가 알고있는 프로그래밍 언어로 DB로 조작하는 방법(나중에 SQL문으로 변환된다)

### ❏ Generic

1. 선언한 시점에 타입을 사용하는것이 아니라 사용 할 때 모든 타입을 마음대로 넣을 수 있다.
2. 타입에 제한을 걸기 위해 `<T extends string | number>` 처럼 사용할 수 있다.

### ❏ 자바스크립트의 동적인 타입 예시

1. `true == "true"`: `false` abstract equality composition (피연산자에 `number` 씌우고 비교한다)
2. `010-03=5`, 0붙어서 8진수가 된다. (16진수는 ox, 2진수는 ob)
3. `1+'1' = '11'`(`+` 는 문자열 우선순위), `11-'1' = 10`(`-` 는 `Number`만 지원한다.)
4. `0/0=NaN` , 숫자로 취급하지 않는다.
5. `1 / 0 > 10 * 1000 = true` : True, infinity는 표현 범위를 넘어서면 취급한다
6. `true++=>Error` : 값에다가 붙이는게 아니라 변수에다 선언해야한다.
7. `1+2+"3" = 33`

---

## 📍 24일차 11.26.금(온라인 강의)

오늘은 `interface`와 `generic`에 대한 개념을 강의로 배웠다.

### ❏ Interface란?

1. 일반적으로 변수, 함수, 클래스에 타입 체크를 위해 사용된다.
2. 직접 인스턴스를 생성할 수 없고, 모든 메소드가 추상 메소드이다.
3. 추상 클래스의 추상 메소드와 달리 `abstract` 키워드는 사용할 수 없다.
4. `ES6` 는 인터페이스를 지원하지 않지만, `Typescript` 는 인터페이스를 지원한다.
5. 정의한 프로퍼티 값을 누락하거나, 정의하지 않는 값을 인수로 전달하면 컴파일시 에러가 발생한다.

### ❏ interface를 사용하는 이유

1. 타입의 이름을 짓고 코드 안의 계약을 정의한다.
2. 프로젝트 외부에서 사용하는 코드의 계약을 정의하는 강력한 방법이다.

```typescript
interface Person {
    name: string;
}

function sayName(obj: Person) {
    console.log(obj.name);
}

let person = { name: "june" };
sayName(person);
```

### ❏ Properties

1. 컴파일러는 프로퍼티의 두 가지 요소를 검사한다. (필수요소 프로퍼티의 유무, 프로퍼티 타입)
2. 아래 예약어로 프로퍼티를 세밀하게 컨트롤 할 수 있다.(?, readonly)

### ❏ Optional Properties

1. 프로퍼티 선언 시 이름 끝에 `?` 를 붙여 표시한다.
2. 인터페이스에 속하지 않는 프로퍼티의 사용을 방지하면서, 사용 가능한 프로퍼티를 기술할 때 사용한다.
3. 객체 안의 몇 개의 프로퍼티만 채워 함수에 전달하는 `option bags` 같은 패턴에 유용하다.

### ❏ Readonly Properties

1. 객체가 처음 생성될 때만 값 설정이 가능하고, 이후 수정이 불가능하다.
2. 프로퍼티 이름 앞에 `readonly` 를 붙여 사용한다.

```typescript
interface Point {
    readonly x: number;
    readonly y: number;
}

let point: Point = { x: 10, y: 20 };
point.x = 5; // Error: Cannot assign to 'x' because it is a read-only property.
```

3. readonly 와 const 의 공통점: 생성 후 배열을 변경하지 않음을 보장한다. 변수에는 const, 프로퍼티에는 readonly 를 사용한다.

### ❏ interface Type

1. TS에서 인터페이스는 함수, 클래스에서 사용할 수 있다.

```typescript
// function type: 함수의 인자 타입, 반환값 타입 정의
interface CountStar {
    (star: string[]): number;
}

const myStars = ["*", "*", "*"];

const getCountStar: CountStar = (stars) => {
    return stars.length;
};

console.log(getCountStar(myStars));

// class type: 클래스가 특정 계약을 충족하도록 명시적으로 강제한다.
interface Animal {
    makeSound(): void;
}

class Dog implements Animal {
    makeSound(): void {
        console.log("멍멍");
    }
}
```

2. 인터페이스와 클래스는 인터페이스간의 확장이 가능하다.

```typescript
interface Animal {
    makeSound(): void;
}

interface Dog extends Animal {
    speed: number;
}

class Bulldog implements Dog {
    makeSound(): void {
        console.log("멍멍");
    }
}
```

3. hybrid type: JS 의 클로저를 TS 로 구현한 문법

```typescript
interface Counter {
    (start: number): string;
    interval: number;
    reset(): void;
}

function getCounter(): Counter {
    let counter = function (start: number) {} as Counter;
    counter.interval = 123;
    counter.reset = function () {};
    return counter;
}

let c = getCounter();
c(10);
c.reset();
c.interval = 5.0;
```

### ❏ 디자인패턴

1. 객체가 할 수 있는 행위들을 전략으로 만들어두고, 동적으로 행위의 수정이 필요한 경우 전략을 바꾸는 것만으로 수정이 가능하도록 만든 패턴이다.
2. 하단의 코드를 살펴보면 메소드를 직접 변경하는것이 아니라 새로운 `interface` 를 생성하고 해당 `interface` 를 적용하면 `Pay` 메소드를 구현할 수 있다.

### ❏ 제네릭이란?

1. 정적 `type` 언어는 클래스나 함수를 정의 할 때 `type` 을 선언해야 한다.
2. `Generic` 은 코드를 작성할 때가 아니라 코드가 수행될 때 타입을 명시한다. 코드를 작성할 때 식별자를 써서 아직 정해지지 않은 타입을 표시한다. (일반적인 식별자는 `T`, `U`, `V` 를 사용한다.)

### ❏ 제네릭을 사용하는 이유

1. 재 사용성이 높은 함수와 클래스를 생성할 수 있다.(여러 타입에서 동작가능, 코드의 가독성 향상)
2. 예상치 못한 오류를 쉽게 포착한다. (`any` : 타입을 체크하지 않아 관련 메소드의 힌트를 얻지 못한다. 컴파일 시 컴파일러가 오류를 찾지 못한다.)
3. `Generic` 은 타입을 체크해 컴파일러가 오류를 찾을 수 있다.
4. `any` 를 지양하고 다양한 타입을 사용하려면 `Generic` 혹은 `Union` 문법을 권장한다.

### ❏ Generic으로 함수와 클래스 만들기

```typescript
// function
function sort<T>(items: T[]) {
    return items.sort();
}

const numbers: number[] = [1, 3, 2];
const strings: string[] = ["a", "b", "c"];

sort<number>(numbers);
sort<string>(strings);

// class
// stack
class Stack<T> {
    protected data: T[] = [];

    push(item: T) {
        this.data.push(item);
    }

    pop(): T | undefined {
        return this.data.pop();
    }
}

const stack = new Stack();
console.log(stack);
stack.push(1);
stack.pop();

// queue
class Queue<T> {
    private data: Array<T> = [];
    // 제네릭을 활용하여 push()와 pop() 메소드를 구현해주세요.
    push(item: T) {
        this.data.push(item);
    }

    pop(): T | undefined {
        return this.data.pop();
    }
}

const numberQueue = new Queue<number>(); // nunberQueue안에 구성된 타입은 number 형이다.

numberQueue.push(0);
console.log(numberQueue.pop());
```

### ❏ Union

1. `|` 을 사용하여 두 개 이상의 타입을 선언하는 방식
2. `union` 과 `generic` 은 모두 여러 타입을 다룰 수 있다. (`union` 은 공통된 메소드만 사용가능하다, 리턴값은 선언된 `union` 타입으로 지정된다.)

```typescript
// Union
const printMessage = (message: string | number) => {
    return message;
};

const message1 = printMessage(1322);
const message2 = printMessage("hellow");

// Generic
const printMessage = <T>(message: T) => {
    return message;
};

const message1 = printMessage<number>(1322);
const message2 = printMessage<string>("hellow");
```

### ❏ 제약조건(constraints / keyof)

1. 원하지 않는 속성에 접근하는 것을 막기 위해 `Generic` 에 제약조건을 사용한다.
2. `Constraints`: 특정 타입들로만 동작하는 `Generic` 함수를 만들 때 사용한다.
3. `Keyof`: 두 객체를 비교할 때 사용한다.

```typescript
// constraints: Generic T에 제약 조건을 설정한다.(string | number)
// 제약 조건을 벗어나는 타입을 선언하면 에러가 발생한다
const printMessage = <T extends string | number>(message: T) => {
    return message;
};

printMessage<number>(1322);
printMessage<string>("hello");
printMessage<boolean>(true); // Error: Type 'boolean' does not satisfy the constraint 'string | number'

// keyof: 두 객체를 비교할 때 사용한다.
// U의 값인 `not in obj` 가 `T`의 키 값 중 존재하지 않기 때문에 오류가 발생한다.
const printMessage = <T extends object, U extends keyof T>(obj: T, key: U) => {
    return obj[key];
};

console.log(printMessage({ a: 1, b: 2, c: 3 }, "a"));
console.log(printMessage({ a: 1, b: 2, c: 3 }, "not in obj")); // Error: Argument of type '"not in obj"' is not assignable to parameter of type '"a" | "b" | "c"'.
```

### ❏ 디자인 패턴

1. `Factory Pattern`: 객체를 생성하는 인터페이스만 미리 정의하고 인스턴스를 만들 클래스의 결정은 서브 클래스가 내리는 패턴
2. 여러개의 서브 클래스를 가진 슈퍼 클래스가 있을 때, 입력에 따라 하나의 서브 클래스의 인스턴스를 반환한다.

---

## 📍 25일차 11.27.토(온라인 강의)

오늘은 `typescript` 심화 그리고 `decorator`에 대해서 배웠다. 지금까지의 프로젝트를 하면서 많이 접해보지 않아 내용이 어렵게 느껴졌다. 나중에 기억에 잘 남으려면 실전에서 많이 사용해야겠지??

### ❏ Union Type, Intersection type

1. 기존 타입, 인터페이스의 변경은 이미 그 타입을 사용하고 있는 코드에 똑같은 변경을 가해줘야 한다. 만약, 해당 타입을 쓰는 모든 코드에 변경을 가하지 않고 특정 코드만 자유롭게 타입을 확장하고 싶을 땐 어떻게 해야할까?

```typescript
// Animal 인터페이스에 메소드를 추가하게 되면 해당 인터페이스를 implements하는 다른 class들에도 동일한 메소드를 추가해야 한다.
interface Animal {
    eat: () => void;
    sleep: () => void;
}

class Dog implements Animal {
    eat() {}
    sleep() {}
}

class Cat implements Animal {
    eat() {}
    sleep() {}
}
```

2. 그럴때는 `Intersection(And)`, : A타입이면서 B타입 `Union(Or)` A타입, B타입 둘 중 하나를 사용한다.

### ❏ Union

1. `|` 부호를 사용한다.

```typescript
// one의 타입은 string과 number 둘 중 하나
let one: string | number;
```

2. 여러 타입 중 하나가 올 것이라고 가정할 때 사용한다. 단, 인터페이스에 유니온 타입을 사용하는 경우 인터페이스는 유니온 타입을 확장하지 못함. 이럴 때는 `type` 과 `&` 를 사용해야 한다.

```typescript
// 에러 케이스
type A = string | number;

interface StrOrNum extends A {
    // Error: An interface can only extend an object type or intersection of object types with statically known members.
    a: string;
}

// 정상 케이스(유니온 타입의 확장)
type A = { a: string & (string | number) };

interface StrOrNum extends A {
    a: string;
}
```

3. Union Type 주의할 점: 동시에 여러 타입이 될 수 없다.

```typescript
// Human인지 Dog인지 확신할 수 없어서 컴파일 단계에서 에러
type Human = {
    think: () => void;
};

type Dog = {
    bark: () => void;
};

declare function getEliceType(): Human | Dog;

const elice = getEliceType();
elice.think(); // Error: Property 'think' does not exist on type 'Human | Dog'. Property 'think' does not exist on type 'Dog'.
elice.bark(); // Error: Property 'bark' does not exist on type 'Human | Dog'. Property 'bark' does not exist on type 'Human'.
```

### ❏ Intersection type

1. `&` 사용
2. `A` 타입이면서 `B` 타입이라는 의미

```typescript
type Human = {
    think: () => void;
};

type Developer = {
    work: () => void;
};

const elice: Human & Developer = {
    think() {
        console.log("I'm thinking");
    },
    work() {
        console.log("I'm working");
    },
};
```

3. `Intersection type` 은 기존 타입을 대체하지 않으면서, 기존 타입에 새로운 필드를 추가하고 싶을 때 사용한다.

```typescript
// Student 메서드를 추가하고 싶을 때
// 전
type Human = {
    think: () => void;
};

type Developer = {
    work: () => void;
};

const elice: Human & Developer & Student = {
    think() {
        console.log("I'm thinking");
    },
    work() {
        console.log("I'm working");
    },
};

// 후
type Student = {
    study: () => void;
};

const elice: Human & Developer & Student = {
    think() {
        console.log("I'm thinking");
    },
    work() {
        console.log("I'm working");
    },
    study() {
        console.log("I'm studying");
    },
};
```

4. 각 타입에 겹치는 필드가 있다면 어떨까?

```typescript
// 타입이 같을 때
type Developer = {
    output: string;
    develop: () => void;
};

type Designer = {
    output: string;
    design: () => void;
};

const 개자이너: Developer & Designer = {
    output: "띠용",
    develop() {
        console.log("I'm working");
    },
    design() {
        console.log("I'm working");
    },
};

// 타입이 다를 때
type Developer = {
    output: number;
    develop: () => void;
};

type Designer = {
    output: string;
    design: () => void;
};

const 띠용: Developer & Designer = {
    output: "며용", // Error: Type 'string' is not assignable to type 'never'.
    develop() {
        console.log("I'm working");
    },
    design() {
        console.log("I'm working");
    },
};

// 타입이 포함관계 일 때
type Developer = {
    output: number;
    develop: () => void;
};

type Designer = {
    output: number | string;
    design: () => void;
};

const 띠용: Developer & Designer = {
    // output : "며용",  Error: Type 'string' is not assignable to type 'number'.
    output: 28,
    develop() {
        console.log("I'm working");
    },
    design() {
        console.log("I'm working");
    },
};
```

### ❏ Type Guard

1. 데이터의 타입을 알 수 없거나, 될 수 있는 타입이 여러 개라고 가정할 때 조건문을 통해 데이터의 타입을 좁혀나가는 것
2. 데이터의 타입에 따라 대응하여 에러를 최소화 할 수 있음. 타입을 통해 가드하는 코드, 방어적인 코드를 짤 수 있음

```typescript
// Human인지 Dog인지 확신할 수 없어서 컴파일 단계에서 에러
type Human = {
    think: () => void;
};

type Dog = {
    bark: () => void;
};

declare function getEliceType(): Human | Dog;

const elice = getEliceType();
elice.think(); // Error: Property 'think' does not exist on type 'Human | Dog'. Property 'think' does not exist on type 'Dog'.
elice.bark(); // Error: Property 'bark' does not exist on type 'Human | Dog'. Property 'bark' does not exist on type 'Human'.

// 타입스크립트가 타입을 추론할 수 있도록 단서를 줘보면 어떨까
type Human = {
    think: () => void;
};

type Dog = {
    tail: string;
    bark: () => void;
};

declare function getEliceType(): Human | Dog;

const elice = getEliceType();

if ("tail" in elice) {
    elice.bark();
} else {
    elice.think();
}
```

3. 구별된 유니온으로 타입 가드하는 방법: 조건문을 통해 어떤 타입인지 추론한다.

```typescript
// 서버에서 오는 응답 또는 함수의 결과가 여러 갈래로 나뉠 때 사용
type SuccessResponse = {
    status: true;
    data: any;
};

type FailureResponse = {
    status: false;
    error: Error;
};

type CustomResponse = SuccessResponse | FailureResponse;

declare function getData(): CustomResponse;

const response: CustomResponse = getData();

if (response.status) {
    console.log(response.data);
} else if (response.status === false) {
    console.log(response.error);
}
```

4. `instanceof`: `TS` 에서 클래스도 타입이다. 객체가 어떤 클래스의 객체인지 구별할 때 사용하는 연산자

```typescript
class Developer {
    develop() {
        console.log("I'm working");
    }
}

class Designer {
    design() {
        console.log("I'm working");
    }
}

const work = (worker: Developer | Designer) => {
    if (worker instanceof Designer) {
        worker.design();
    } else if (worker instanceof Developer) {
        worker.develop();
    }
};
```

5. `typeof` : 데이터의 타입을 반환하는 연산자 (`data==null` 동등연산자를 사용하면 `null`, `undefined` 둘다 체크한다. 그러나, `null` 과 `undefined` 는 따로 체크하는 습관을 기르자, )

```typescript
const add = (arg?: number) => {
    if (typeof arg === "undefined") {
        return 0;
    }
    return arg + arg;
};
```

6. `in` : 오브젝트의 `key`중에 문자열 `A` 가 존재하는지 확인할 때

```typescript
// 문자열 A는 key(field, property 이름)을 의미한다.
type Human = {
    think: () => void;
};

type Dog = {
    tail: string;
    bark: () => void;
};

declare function getEliceType(): Human | Dog;

const elice = getEliceType();

if ("tail" in elice) {
    elice.bark();
} else {
    elice.think();
}
```

7. `switch-case`, `else-if`

```typescript
type Action = "click" | "hover" | "scroll";

// switch
const doPhotoAction = (action: Action) => {
    switch (action) {
        case "click":
            showPhoto();
            break;
        case "hover":
            zoomInPhoto();
            break;
        case "scroll":
            loadPhotoMore();
            break;
    }
};

// if
const doPhotoAction = (action: Action) => {
    if (action === "click") {
        showPhoto();
    } else if (action === "hover") {
        zoomInPhoto();
    } else {
        loadPhotoMore();
    }
};
```

8. `type-guard` 에 유용한 오픈소스

```typescript
// yarn add @sindersorhus/is
import is from "@sindresorhus/is";

const getString = (arg?: string) => {
    if (is.nullOrUndefined(arg)) {
        return "";
    }

    if (is.emptyStringOrWhiteSpace(arg)) {
        return "";
    }

    return arg;
};
```

### ❏ Optional Chaning

1. 접근하는 객체의 프로퍼티가 `null` 또는 `undefined` 일 수 있는 `optional property` 인 경우 `if` 문을 사용하지 않고 넘어가게 하는 체이닝 방법
2. `es2020` 에서 추가된 문법이며, 객체가 `null` 또는 `undefined` 이면 `undefined` 를 리턴, 그렇지 않은 경우 데이터 값을 리턴
3. `&&` 와 `?.` 의 차이점: `&&` 는 `falsy` 한 값 체크, `?.` 는 `null` 과 `undefined` 만 체크

```typescript
// 값이 있을 때만 반환한다.
type Cat = {
	sitDown?: () => void;
}

function trainCat(cat: Cat){
	cat.sitDown?.();
}

// 분기처리 optional Chaining
type Tail = {
	살랑살랑: () => void;
}

type Human = {
	call: (dogName: string) => void;
]

type Dog = {
	name: string;
	tail?: Tail;
	주인?: Human;
}

function petDog(dog: Dog){
	dog.주인?.call(dog.name);
	dog.tail?.살랑살랑();
}

// optional chaining refactory
// 전
function petDog(dog?: Dog) {
  if (dog && dog.tail && dog.tail.살랑살랑) {
    dog.tail.살랑살랑();
  }
}

// 후
function petDog(dog?: Dog) {
	dog?.tail?.살랑살랑?.();
}
```

### ❏ Nullish Coalescing Operator

1. `es2020` 에서 추가된 문법이며, 좌항이 `null`, `undefined` 인 경우에만 `B` 를 리턴
2. `A ?? B`: `falsy` 값을 그대로 리턴하고 싶은 경우 사용

```typescript
// price가 0인 경우 -1 반환
function getPrice1(product: { price?: number }) {
    return product.price || -1;
}

// price가 0인 경우 0 반환
function getPrice2(product: { price?: number }) {
    return product.price ?? -1;
}

console.log(0 ?? -1); // 0
console.log(0 || -1); // -1
```

3. falsy한 값(false로 평가되는 값) 0과 empty string(‘’)이 올 수 있는 변수에 **`||`** 를 쓰면 0, ‘’를 false로 인식하기 때문에 의도치 못한 결과를 초래할 수 있습니다. 실무에서 흔하게 저지르는 실수이기도 합니다. default 값을 지정해줄 때는 **`||`** 이 아니라 **`??`**을 쓰는 것을 권장합니다.

### ❏ Function overloading

1. 파라미터의 타입만 다르고 비슷한 코드가 반복되고 있는 상황, 코드의 중복을 줄이고 재사용성을 높일때 사용
2. 파라미터의 형태가 다양한 여러 케이스에 대응하는 같은 이름을 가진 함수를 만드는 것, 함수의 다형성을 지원하는 것
3. 함수의 이름이 같아야한다. 매개변수의 순서는 같아야한다. 반환 타입이 같아야 한다. `function` 키워드로만 가능하다,
4. 함수 오버로딩의 타입 선언부는 런타임에서 제거되고 구현부만 남기때문에, 실제 구현, 정의하는 함수는 하나여야만 한다.

```typescript
// 매개변수가 같을 때
class User {
    constructor(private id: string) {}

    setId(id: string): void;
    setId(id: number): void;
    setId(id: string | number): void {
        this.id = typeof id === "number" ? id.toString() : id;
    }
}

// 매개변수의 개수가 다를 때(순서만 지켜주면 된다.)
class User {
    constructor(private id: string) {}

    setId(id: string): void;
    setId(id: number, radix: number): void;
    setId(id: string | number, radix?: number): void {
        this.id = typeof id === "number" ? id.toString(radix) : id;
    }
}
```

제네릭은 사용하는 시점(제네릭, 인터페이스, 클래스 등등), 함수 오버로딩은 타입을 선언하는 시점(함수, 메서드)

### ❏ Type assertion

1. 타입스크립트가 추론하지 못하는 타입을 `as keyword` 를 통해 명시해주는 것
2. `type casting`: 데이터의 타입을 변환, `type assertion` : 데이터의 타입을 명시

```typescript
let someValue: unknown = "this is a string";

// 꺽쇠괄호는 react JSX가 인식을 잘 못함.
let strLength: number = (<string>someValue).length;

// as태그
let strLength: number = (someValue as string).length;
```

3. 타입단언: 타입스크립트가 개발자의 말만 믿고 `Duck` 타입으로 인식하여 빈 객체임에도 에러를 뱉지 않음
4. 타입선언: 객체 프로퍼티를 모두 채우도록 강제하기 대문에 실수를 저지를 위험이 낮음

```typescript
type Duck = {
	quack: () => void;
}

const duck: {} as Duck;

function add(x: string, y: string) {
  return (x as unknown as number) + (y as unknown as number)
}

const result = add('1', '2')
console.log(result)
```

### ❏ Index Signatrue

1. 객체의 특정 `value` 에 접근할 때 그 `value` 의 `key` 를 문자열로 인덱싱해 참조하는 방법
2. 객체의 프로퍼티들을 명확하게 알 수 없을 때 사용한다.
3. 어떤 타입이 올지 알 수 있다면 정확하게 타입을 정의하는것이 실수를 방지할 수 있다.
4. 인덱스 시그니처만 사용할 시, 타입을 표시해준 빈 객체에 에러가 나지 않습니다.

```typescript
type ArrStr = {
    [key: string]: string | number;
};

// HTTP headers
type HttpHeaders = {
    [key: string]: string;
};

type HttpHeaders = Record<string, string>;

const headers: HttpHeaders = {
    Host: "elice.io",
    Connection: "keep-alive",
    Accept: "*/*",
    "Access-Control-Request-Method": "GET",
    "Access-Control-Request-Headers": "authorization",
    "User-Agent":
        "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/95.0.4638.69 Safari/537.36",
    "Sec-Fetch-Mode": "cors",
    "Sec-Fetch-Site": "same-site",
    "Sec-Fetch-Dest": "empty",
    "Accept-Language": "ko-KR,ko;q=0.9,en-US;q=0.8,en;q=0.7",
};

console.log(headers["Host"]); // elice.io
```

### ❏ Decorator

1. 함수가 한 가지 일만하면서 가독성을 높이고 반복되는 코드를 줄일 때 사용한다.
2. 함수를 감싸는 함수: 기존 함수를 바꾸지 않고 함수를 관찰, 수정, 재정의(오버라이딩)할 수 있는 함수
3. `babel` 플러그인을 사용해서 데코레이터 기능을 사용한다. `tsconfig.json` 에 `experimentDecorator` 옵션을 `true` 로 설정해줘야 한다.
4. 단일책임원칙 하에 함수의 기능을 확장할 수 있다.
5. `JS` `stage2` 에 있는 기능이므로, `TS` 에서는 실험적 기능으로써 사용 가능.

### ❏ 데코레이터를 쓰기 전 알아야 할 자바스크립트 개념

1. 일급객체
2. 클로저: 외부함수의 실행이 끝나도 내부함수에서 외부함수의 `context` 에 접근할 수 있는 것
3. 고차함수: 함수를 파라미터로 받아 반환하는 함수.

### ❏ 고차 함수의 용도

1. 커링: 함수의 매개변수를 받는 시점을 늦출 때
2. 함수의 실행 시점을 미룰 때(`jest - expect`, `react - onClick`)
3. 팩토리 함수(인스턴스 객체나 함수를 생성하여 반환하는 함수)를 만들 때
4. 훅, 데코레이터를 만들 때
5. 반복되는 코드를 줄일 때
6. 클래스 메서드는 고차 함수의 파라미터로서 전달했을 때 메서드는 인스턴스에 대한 `this` 바인딩을 잃어버린다. 따라서 `higher order`함수를 호출할 때 인스턴스와 메서드를 함께 인자로 전달해줘야 함

### ❏ Decorator Factory

1. 데코레이터를 사용하려면 `tsconfig.json - experimentalDecorators: true`, `emitDecoratorMetadata: true` `yarn add reflect-metadata` 설정
2. 고차함수: 함수를 반환하는 함수
3. 팩토리: 어떤 인스턴스를 사용하여 반환하는 함수, 메서드
4. 데코레이터 팩토리: 데코레이터 함수를 반환하는 함수
5. 특정 인자만 받는다. 추가적인 인자를 주고 싶다면 고차함수에 매개변수를 추가하여 데코레이터 함수 내부에서 사용할 수 있다.

```typescript
function enumerable(value: boolean) {
    return function (
        target: any,
        propertyKey: string,
        descriptor: PropertyDescriptor
    ) {
        descriptor.enumerable = value;
    };
}

class Greeter {
    @enumerable(false)
    greet(name: string) {
        return "Hello, " + name;
    }
}

// decoratorFacotry 함수를 선언해주세요.
function decoratorFactory(value: string) {
    return function (
        target: any,
        propertyKey: string,
        propertyDescriptor: PropertyDescriptor
    ) {
        console.log(value);
    };
}
// string 타입이고 이름이 value인 매개변수를 받습니다.
// 메서드 데코레이터 함수를 반환합니다.
// 메서드 데코레이터 함수의 매개변수 'target: any, propertyKey: string, propertyDescriptor: PropertyDescriptor'
// 메서드 decorator 함수 내부에서 value를 출력해주세요.

class ExampleClass {
    @decoratorFactory("룰루랄라 퇴근이다")
    static method() {}
}

ExampleClass.method();
```

### ❏ 클래스 데코레이터

1. 생성자 함수를 관찰, 수정, 오버라이딩(재정의) 한다.
2. 기존 클래스의 코드를 변경하지 않고 `property` 를 추가하거나, 생성자 함수에서 기능을 추가하고 싶을 때 사용한다.
3. 클래스 선언 직전에 선언된다.
4. 런타임에 함수로서 호출된다. `class` 에 `property`를 추가해도 `type system` 에서는 알지 못 함
5. 생성자 함수에 적용된다.
6. `target` 매개변수는 생성자 함수이다.
7. `d.ts` 파일(타입 선언 파일), `declare class`에는 데코레이터를 사용하지 못함(`experimentalDecorators: true`)를 해도 안된다.

```typescript
declare type ClassDecorator = <TFunction extends Function>(
    target: TFunction
) => TFunction | void;
```

### ❏ method Decorator

1. 메서드를 관찰, 수정, 오버라이딩 할 수 있다.
2. 메서드의 `property descriptor` 를 수정하거나 기존 메서드 앞 뒤로 기능을 추가하고 싶을 때 사용한다.

```typescript
import { UserGroup, User, Context } from "./types";

function permission(group: UserGroup) {
    return function (
        target: any,
        propertyKey: string,
        descriptor: PropertyDescriptor
    ) {
        const originFn = descriptor.value;

        // decorator function을 작성해주세요.
        descriptor.value = function (this: any, ...args: any[]) {
            // viewer의 group이 매개변수의 group보다 높은 경우(권한이 없는 경우) 함수를 실행하지 않고 에러메시지를 출력해주세요.
            const user = this.context.viewer;
            if (user.group > group) {
                console.log(
                    "permission is denied. viewer group is " + user.group
                );
                return;
            }
            // viewer의 group이 매개변수의 group 이하인 경우 원래 함수를 그대로 실행해주세요.
            return originFn.apply(this, args);
        };

        return descriptor;
    };
}

class UserService {
    constructor(public context: Context) {}

    @permission(UserGroup.NORMAL)
    updateName(user: User, name: string) {
        user.name = name;
    }

    @permission(UserGroup.ADMIN)
    deactivateUser(user: User) {
        user.status = "deactivate";
        return user;
    }
}

const normal: User = {
    id: "1",
    name: "normal",
    status: "activate",
    group: UserGroup.NORMAL,
};

const userService = new UserService({ viewer: normal });
// "permission is denied. viewer group is 2" 출력
userService.deactivateUser(normal);
userService.updateName(normal, "elice");
console.log(normal.name);
```

### ❏ Accessor Decorator

1. 접근자(`getter`, `setter`) 데코레이터는 접근자를 관찰, 수정, 오버라이딩 할 수 있다.
2. 접근자의 프로퍼티 설명자에 적용된다. 전달받는 매개변수가 메서드 데코레이터와 똑같다.(`target`, `propertyKey`, `propertyDescriptor`)
3. `method decorator` 와 같이 `ES5` 보다 낮으면 `undefined` 이 된다. 또한 반환값도 무시된다.
4. 같은 프로퍼티에 대한 접근자 `get`, `set` 중 하나에만 데코레이팅 가능

```typescript
function validate(regexp: string | RegExp) {
    return function (
        target: any,
        property: string,
        descriptor: PropertyDescriptor
    ) {
        const actualFunction = descriptor.set;

        const decoratorFunc = function (this: any, value: string) {
            const regexpTarget =
                typeof regexp === "string" ? new RegExp(regexp) : regexp;
            if (!regexpTarget.test(value)) {
                throw new Error("invalid value");
            }
            return actualFunction?.call(this, value);
        };

        descriptor.set = decoratorFunc;
    };
}
```

```typescript
function max(maximum: number) {
    return function (
        target: any,
        property: string,
        descriptor: PropertyDescriptor
    ) {
        // setter 함수를 교체하려면 descriptor의 어떤 프로퍼티에 적용해야할까요?
        const actualFunction = descriptor.set!; // 느낌표는 타입스크립트에 set함수가 있다고 가정한다. (option )

        const decoratorFunc = function (this: any, value: number) {
            // value가 maximum보다 커지면 `exceed the maximum number: ${maximum}`를 메시지로 메시지로 하는 Error를 throw해주세요
            if (value > maximum) {
                throw new Error(`exceed the maximum number: ${maximum}`);
            }

            // maximum 이하일 때는 함수를 정상적으로 실행해주세요
            return actualFunction.call(this, value);
        };

        descriptor.set = decoratorFunc;
    };
}

class Pagination {
    constructor() {}

    private _page: number = 0;

    get page() {
        return this._page;
    }

    @max(10)
    set page(step: number) {
        console.log();
        this._page = step;
    }
}

const pagination = new Pagination();

// Error: exceed the maximum number: 10
try {
    while (true) {
        pagination.page += 1;
    }
} catch (error) {
    console.log(error);
}
```

### ❏ Property Decorator

1. 프로터피를 관찰, 수정, 오버라이딩 할 수 있다.
2. 프러퍼티의 `property Descriptor` 를 수정할 때 사용할 수 있따.
3. 프로퍼티 선언 직전에 선언된다.
4. 인스턴스가 아닌 클래스 프로토타입의 프로퍼티에 적용된다.
5. `taget`, `propertyKey` 두가지 인자를 받는다.
6. `property Descriptor` 를 사용하지 않는이유: 프로퍼티의 경우, 인스턴스화 되기 전까 지 프로퍼티가 초기화되는 것을 관찰하거나 수정할 수 없음. 때문에 프로퍼티 데코레이터는 프로퍼티가 `클래스` 에 선언되었음을 관찰하는데만 사용할 수 있다.

```typescript
declare type PropertyDecorator = (
    target: Object,
    propertyKey: string | symbol
) => void | PropertyDecorator;

// 프로토타입 공유
function 영혼교환식(target: any, propertyKey: string) {
    let name: string;

    const getter = function () {
        return name;
    };

    const setter = function (value: string) {
        name = value;
    };

    return {
        get: getter,
        set: setter,
        enumerable: true,
        configurable: true,
    } as any;
}

class Human {
    @영혼교환식
    public name: string;

    constructor(name: string) {
        this.name = name;
    }
}

const 햄스터 = new Human("햄스터");
const 그녀 = new Human("그녀");

그녀.name = "민석씨";
console.log(햄스터.name); // 민석씨: 인스턴스가 아닌 클래스 프로토타입의 프로퍼티에 적용되기 때문에 값이 공유된다.

// 프로토타입 Symbol
function 영혼교환식(target: any, propertyKey: string) {
    const uniqueKey = Symbol(); // 매번 unique값을 생성

    const getter = function (this: any) {
        return this[uniqueKey];
    };

    const setter = function (this: any, value: string) {
        this[uniqueKey] = value;
    };

    return {
        get: getter,
        set: setter,
        enumerable: true,
        configurable: true,
    } as any;
}

class Human {
    @영혼교환식
    public name: string;

    constructor(name: string) {
        this.name = name;
    }
}

const 햄스터 = new Human("햄스터");
const 그녀 = new Human("그녀");

그녀.name = "민석씨";
console.log(햄스터.name); // 햄스터
```

1. 프로퍼티가 `null` 또는 `undefined` 일 때 기본값을 반환하는 `Default` 데코레이터만들기

```typescript
function Default(initalValue: any) {
    return function (target: any, propertyKey: string) {
        // 내부 함수에서 쓰일 value를 선언해주세요.
        let value: any;
        // value의 타입을 any로 설정해주세요

        // getter, setter 함수를 작성해주세요
        // getter: value가 null 또는 undefined면 initalValue를 반환해주세요
        function getter() {
            return value ?? initalValue;
        }

        // setter: setter 함수의 매개변수 _value를 그대로 value에 할당해주세요
        function setter(_value: any) {
            value = _value; // this를 붙이지 않아도 됨.
        }

        // propertyDescriptor를 반환해주세요
        // enumerable, configurable을 함께 설정해주세요
        const propertyDescriptor = {
            get: getter,
            set: setter,
            enumerable: true,
            configurable: true,
        };
        return propertyDescriptor as any;
    };
}

class Post {
    @Default(["짱이에요", "멋져요"])
    public comments?: any[];
}

const post = new Post();
console.log(post.comments);
```

### ❏ Parameter Decorator

1. 클래스의 생성자 함수 또는 메서드 선언 함수에 적용된다.
2. 매개변수가 메서드에서 선언되었다는 것을 관찰하는데에만 사용 가능. 그 이상은 `reflect-metadata` 라이브러리를 사용해야 한다.
3. 매개변수 선언 직전에 사용된다.
4. 3가지 인자를 받는다. 반환값은 무시된다.
5. `reflect-metatdata` 를 통해 파라미터에 대한 메타데이터 수집, 저장.
6. 메서드 데코레이터나 클래스 데코레이터와 함께 사용할 수 있음
7. 파라미터 데코레이터 함수에서 반환하는 값은 무시됩니다. (반환값이 void)
8. 파라미터 데코레이터는 메서드에서 매개변수가 선언되었다는 것만 알 수 있습니다.

```typescript
// target은 method(any, object), propertyKey는 메서드의 이름(string, symbol), 매개변수의 인덱스(순서)
declare type ParameterDecorator = (
    target: Object,
    propertyKey: string,
    parameterIndex: number
) => void;

function watch(target: Object, propertyKey: string, parameterIndex: number) {
    console.log(
        `메서드 이름: ${propertyKey}, 데코레이터 인덱스: ${parameterIndex}`
    );
}

class Human {
    constructor(public name: string) {}
    hello(@wath name: string) {}
}

declare type ParameterDecorator = (
    target: Object,
    propertyKey: string | symbol,
    parameterIndex: number
) => void;
```

1. reflect-metadata

```typescript
import { immutableKey } from "./immutable";

export function validateImmutable(
    target: any,
    propertyName: string,
    descriptor: PropertyDescriptor
) {
    const method = descriptor.value!;

    descriptor.value = function () {
        // Reflect.getOwnMetadata를 사용해 메타데이터를 가져와주세요
        const immutableParams: number[] = Reflect.getOwnMetadata(
            immutableKey,
            target,
            propertyName
        );
        // 메타데이터에는 paramIndex가 저장되어있습니다.

        const args = Array.from(arguments as any);
        // 자바스크립트 함수 내부에서 제공되는 arguments에서 메타데이터의 paramIndex만 필터링 해주세요. 그런 뒤 params 변수에 할당해주세요.
        const params = args.filter((val, idx) => immutableParams.includes(idx));

        // params 배열을 순회하며 Object.freeze로 객체를 수정하지 못하게 막아주세요.
        // map: 배열의 item을 변환하여 배열을 반환
        // forEach: 배열을 반환하지 않고 각 item에 함수를 적용할 때
        params.forEach((param) => Object.freeze(param));
        return method.apply(this, arguments);
    };
}
```

### ❏ Decorator의 동작

1. 여러 개의 데코레이터를 한 번에 쓰는 것(합성 함수 `g(fx))` 와 같은 매커니즘
2. `Reflect.decorate` 를 쓸 수 있으면 호출, 없으면 인자의 개수에 따라 매개변수를 다르게 주어 데코레이터를 호출한다.(이때 호출은 아래에서 위로, 합성함수의 매커니즘처럼 작용하기 때문)

```typescript
// 평가(선언): 위에서 아래로, log -> timer
// 적용(호출): 아래에서 위로, timer -> log
class Human {
	constructor(){}
	@log()
	@timer()
	hello(name: string){}

	const elice = new Human();
	elice.hello("elice")
}
```

3. 여러개의 데코레이터의 실행 순서

```typescript
/**
 * code source: https://www.typescriptlang.org/docs/handbook/decorators.html#decorator-composition
 */
function first() {
  console.log("first(): factory evaluated"); // #1
  return function (
    target: any,
    propertyKey: string,
    descriptor: PropertyDescriptor
  ) {
    console.log("first(): called"); // #2
  };
}

function second() {
  console.log("second(): factory evaluated"); // #3
  return function (
    target: any,
    propertyKey: string,
    descriptor: PropertyDescriptor
  ) {
    console.log("second(): called"); // #4
  };
}

class ExampleClass {
  @first()
  @second()
  method() {}
}

// 순서: 1 -> 3 -> 4 -> 2
first(): factory evaluated
second(): factory evaluated
second(): called
first(): called
```

---

## 📍 26일차 11.30.화(실시간 강의)

오늘부터는 `FE`가 아닌 `BE`에 대해서 간략하게 배운다. 여러 프레임워크 중 `Node.js`에 대해서 배우는데 한번 알아보자. 실시간 강의 때는 주로 실습을 하느라 이론을 많이 배우지 못했다. 내일 온라인 강의에서 더 자세하게 알아봐야겠다.

### ❏ Node.js

1. Chrome V8 javscript 엔진으로 빌드된 `javascript` 런타임입니다.
2. `Node.js`의 메인스레드는 하나이다. `JS`가 단일쓰레드인것처럼 `node.js`도 한 번에 한줄씩 실행한다.
3. `Docker`, `Auto scaling` 등을 이용해 `node.js`의 단일 스레드의 단점을 보완 할 수 있다.
4. `offLoading`: 메인스레드와 이벤트 루프는 서로 영향을 받지 않고 계속 실행된다.(저수준의 오래 걸리는 일은 `node.js`에게, 고수준의 로직은 메인스레드에서 실행한다.)
5. `LinkedIn`, `NETFLIX`, `UBER` 등에서 `node.js`를 사용한다.
6. <a href='https://glitch.com/'>Glich</a> 사이트를 통해 온라인에서 무료로 `node.js` 환경을 구축할 수 있다.
7. 예전의 `JS`는 퍼포먼스가 굉장히 떨어졌다. -> 이상한 코드를 집어넣으면 홈페이지가 느려진다. -> `firefox - spidermonkey`로 인해 성능이 매우 좋아졌다. > `microsoft - node.js`는 해당 환경을 브라우저가 아닌 로컬환경에서 작동시키기 위해 만들었다.
8. 런타임 환경: 컴퓨터가 실행되는 동안 프로세스나 프로그램을 위한 소프트웨어 서비스를 제공하는 가상 머신 상태
9. 컴파일 에러: 프로그램 동작 전에 발생하는 에러
10. 런타임 에러: 프로그램이 잘 동작하다가 중간에 발생하는 에러
11. `prettier`: 개발자가 작성한 코드를 통일시키는 방법
12. `eslint`: 자잘한 문법을 잡아준다. 코드를 분석하여 문법적인 오류, 안티 패턴ㅇ르 찾아준다.
13. `npm init`: `package.json` 생성
14. `npm init`: `package.json` 생성
15. `npm i eslint --save-dev`: eslint 설치
16. 라이브러리 ESLint 설치
17. `npm i -g npm`
18. `./node_modules/.bin/eslint --init` : eslint 환경설정
19. `npm i prettier`: 프리티어 설치
20. `./node_modules/.bin/prettier filename`
21. `./node_modules/.bin/prettier filename write`
22. `format`: format on save
23. `formatter`: 어떤 문법규칙으로 정리할지 선택하는 기능
24. `npm i eslint-plugin-airbnb`: airbnb 문법 사용

```javascript
const http = require("http"); // http 모듈 호출
const port = 9999;

http.createServer((req, res) => {
    res.end("Hello, world!"); // end: 담길데이터 다 담겼으니까 요청 글자를 보낸다.
}).listen(port, () => {
    console.log("서버가 켜졌어요!!!");
});

// 이후 F5 -> node.js실행
// res.end("<p style='color:red'>gimotti!!!</p>");처럼 innerHTML와 같은 코드로도 보낼 수 있다.
```

25. `commonJS` 방식은 `Node.js`에서 사용하는 방식으로 ES2015 의 모듈 개념이 나오기 전부터 사용됨. 기본은 `CommonJS` 이나, `package.json`을 수정하면 사용할 수 있음

```javascript
// CommonJS(default)
const http = require("http");

// ES2015, but 실질적인 사용은 2019년부터
import http from "http";
```

26. 동일한 `IP주소` 여도 포트번호를 통해 다르게 연결 할 수 있다.(default: 80)
27. `JS: Express.js` , `TS: Nest.js + Typescript` (해외에서 많이 쓰이고, 국내에서는 스프링을 많이 쓴다. 스프링은 전자정부에서 권장하는 프레임워크라서 많이 사용된다. 러닝커브가 상당히 빡세다.)
28. docker: 서버에 무엇인가를 설치할 때 오류가 발생함. 이런 문제를 줄이기 위해 나왔다. 설치가 이미 완료된 컨테이너를 가지고 잇다. 서비스에 올리기만 하면 바로 사용가능함. 모든 기술은 필요에 의해 나왔기 때문에 왜 기술을 사용하는지에 대해 알아두자.
29. 요즘 개발은 서버와 프론트를 컨테이너 안에 두고 깃허브에서 작성한 코드 커밋 → 테스트 → 빌드 → 자동으로 서버에 올린다. 이러한 과정을 `CI/CD` 라고 부른다.

### ❏ 내장 모듈

1. `node.js` 내부에서 제공하는 모듈
2. 모듈명이 같으면 현재 폴더를 기준으로 가장 가까운 모듈을 먼저 가져온다.
3. `require('fs').readFileSync`: 동기적으로 파일을 불러온다. (아무런 인코딩을 하지 않으면 `byte` 형태로 값을 불러온다. `Buffer`: 16진수 형태)

```javascript
const fs = require("fs");
const result = fs.readFileSync("./test");
const buf = Buffer.from([97, 98, 99, 100, 101]);
console.log(buf.compare(result)); // 0: 서로 같으면 0을 반환, 1이면 `buf` 가 더 크고, -1이면 `result`가 더 크다.

// 에러처리는 try-catch문으로 실행
```

4. `node.js` 데이터 구조: `stream` : 데이터를 작은 청크로 쪼개 처리한다. 큰 데이터를 처리하거나 비동기적으로 얻을 수 있는 데이터를 처리할 때 유용하다.

```javascript
const fs = require("fs");
const stream = fs.createReadStream("src/test");
stream.pipe(process.stdout);
```

5. `__filename`, `__dirname`: 파일 경로, 폴더 경로 표시하는 명령어

```javascript
console.log("__dirname", __dirname);
cosnole.log("__filename", __filename);
```

6. `dns`: `dns` 정보접근

```javascript
// family: verson(IPv4, IPv6...)
const dns = require("dns");
dns.lookup("google.com", (err, address, family) => {
    console.log(address, family);
});
```

7. `path`: 경로설정

```javascript
const path = require("path");
const fs = require("fs");

// 절대 경로 넣기
const filePath = path.resolve(__dirname, "./test.txt");
const fileContent = fs.readFilSync(filepath, "utf-8");
```

---

## 📍 27일차 12.1.수(온라인 강의)

오늘은 2021년 마지막 해의 첫 날이다. 그날 배운 내용들을 복습하는 글도 27번째 쓰고있는데, 22년 2월까지 하루도 빠짐없이 복습하는 글을 작성했으면 좋겠다. 현업에 뛰어들어서 볼 지금의 글들이 밤톨이나마 도움이 된다면 나의 목표는 달성한 것이다. 강의에서는 어제 실시간 강의로 간략하게 배웠던 `node.js`, `express.js`, `module` 등에 대해서 조금 자세하게 배웠다.

### ❏ node.js의 등장 배경

1. 웹의 발전에 의해 등장함. 단방향 통신 위주였던 `WEB1.0` 에서 사용자와 상호작용하는 `WEB2.0` 으로 발전하게 되면서 웹페이지의 동작은 더욱 복잡해졌고, 복잡한 `JS` 를 실행하기위해 고성능의 `JS` 실행기가 필요해졌다. 크롬에서는 웹브라우저를 위한 `V8` 엔진을 만들게 됨 `V8` 엔진으로 인해 `JS` 속도가 상당히 빨라지게 됐고, `V8` 엔진을 이용해서 웹 브라우저에서만 사용하는것이 아닌 어느 환경에서나 동작시킬 수 있도록 만들어진것이 `node.js` 이다. 즉, `js` 를 어느환경에서나 실행할 수 있게 해주는 실행기라고 할 수 있다.
2. 브라우저에서의 `JS`: 브라우저에서 실행, 웹 내부 제한된 동작, 웹 프론트 개발자의 언어
3. `node.js`: 크로스 플랫폼 실행, 제한 없는 동작, 다양한 어플리케이션 개발, 모든 개발자의 언어가 되었다.
4. `FE` : React.js, `BE`: Express.js,(최근 가장 인기 있는 웹서비스 구성), `Mobile`: React-native,(한가지 코드로 IOS와 Android 개발), `Desktop-app`: Electron(discord, slack 등 앱개발), `Machine-Learning`: Brain.js (JS로 구현하는 딥러닝)

![](https://images.velog.io/images/abcd8637/post/ad5ca1e3-ba08-42f4-83a8-47bf8ff67d4b/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-01%2009.20.00.png)

### ❏ node.js의 특징

1. 싱글 스레드 - 비동기 - 이벤트 기반
2. 스레드: 명령을 실행하는 단위, 싱글스레드는 한 번에 한 가지 동작만 실행 가능, 멀티쓰레드는 동시에 여러 동작 수행 가능하다.
3. 장점: 스레드가 늘어나지 않기 때문에 리소스 관리에 효율적
4. 단점: 스레드 기반의 작업들의 효율이 떨어짐(CPU 연산 작업)
5. 그래서 `node.js` 는 비동기 동작으로 스레드 기반의 작업을 최소화한다.
6. 비동기: 동작을 실행한 후 완료가 되길 기다리지 않는 방식, 동작의 완료를 기다리지 않기 때문에 다른 동작을 바로 실행 가능, `node.js` 는 싱글 스레드이기 때문에 비동기 방식을 사용함.
7. 멀티스레드는 한번에 여러가지 동작을 수행하기 때문에 동작을 수행하고 완료를 기다리는 동안 `CPU` 리소스가 낭비되는 반면, 싱글스레드는 한번에 여러가지 동작을 수행할 수 없지만 동작의 완료를 기다리지 않기 때문에 `CPU` 리소스를 효율적으로 사용할 수 있다.
8. 이벤트 기반: 비동기 동작의 완료를 처리하는 방법. 비동기 방식은 특정 동작을 실행한 후, 해당 동작을 전혀 신경쓰지 않음. 대신 해당 동작이 완료될 경우 실행 할 함수를 미리 등록함. 비동기 동작이 완료되면 미리 등록된 함수를 실행한다.
9. `node.js` 는 싱글 스레드기 때문에 비동기 동작이 필요하고 비동기 동작을 구현하기 위해 이벤트 기반의 동작 방식을 사용한다.

![](https://images.velog.io/images/abcd8637/post/099e18f8-03f5-482c-a601-06272f907e33/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-01%2009.27.01.png)

### ❏ node.js 시작하기

1. `node.js` 는 빠르게 개발 중이므로 보안 이슈 및 버그 수정, 최신기술을 빠르게 적용한다. 급변하는 기술은 가장 안정적인 최신 버전을 선택하는 것이 최선이다.
2. `LTS(Long-term support)`: `node.js` 의 안정적이고, 오래 지원하는 버전 명
3. 가장 최신의 기술보다 안정적이고 최신의 버전을 선택하자.

### ❏ ES6

1. `ECMA6` 버전 이후를 통틀어 일반적으로 `ES6` 라고 부름
2. `ECMAScript`: 계속해서 발전해가는 `JS` 의 표준문법, 2015년 `ES6` 이후 많은 현대적인 문법이 추가됨
3. `let`, `const`: 상수와 변수 구분 가능
4. `Template String`: 기존에는 줄 바꿈은 `\n` 를 사용했으나 `backtick` 사용시 `\n`을 사용하지 않아도 된다. 변수는 `${}` 와 같이 사용할 수 있다.
5. `arrow-function`: 기존 함수는 `function` 으로 선언했으나, `()=>{}` 와 같이 간결하게 표현 가능하다.
6. `class`: 기존에는 객체 지향을 구현하기 위해 `function` 과 `prototype` 을 사용했다. `class` 는 `function` 으로 선언하고 클래스의 멤버나 메소드를 구현할 때는 `prototype` 을 사용했다. 이는 직관적이지 않고 가독성이 떨어졌다. `ES6` 에서 `class` 형태로 객체 지향적인 코드를 작성할 수 있다.
7. `destructing`: `Object` 에서 값을 꺼낼 때 일일이 작성하지 않고 `{} = obj` 처럼 변수를 꺼낼 수 있다.

### ❏ 비동기 코딩

1. 비동기: 이벤트 기반 동작을 코드로 구현하는 방법
2. `callback`: 전통적인 `JS` 의 이벤트 기반 코딩 방식

```javascript
// callback
// getUsers로 넘기는 함수가 이벤트 함수이고, 이러한 형태를 콜백이라 부른다.
// 쿼리가 완료되면 오류가 있는지, 혹은 성공했는지 여부를 인자형태로 받는다.
// 에러와 결과를 같이 전달하는 것이 표준으로 자리잡혀 있음

db.getUsers((err, users) => {
	console.log(users)
});

// callback-hell
// async1, async2, async3...을 동기적으로 실행해야 하는 경우, node.js는 기본적으로 비동기 동작을 callback으로 처리하기 때문에 콜백지옥 현상이 일어난다.
db.getUsers((err, users) => {
	if (err) {
		return;
	}
	async1(users, (r1) => {
		async2(r1, (r2) => {
			async3(r2, (r3) => {
				...
			});
		});
	});
});
```

3. `Promise`: callback 의 단점을 보완한 비동기 코딩 방식

```javascript
// promise: 함수의 동작이 완료되면 then에 등록된 callback을 실행한다. 오류가 발생한 경우 catch문의 callback 실행
// promise.chaning으로 코드를 간결하게, short-hand 표현으로 더욱 간결하게 표현 가능
db.getUsersPromise()
	.then((users) => {
		return promise1(users);
})
	.then(r1 => promise2(r1))
	.catch(... );

// callback을 promise 함수로 변경하기
// async1 함수의 실행 결과에 따라 resolve, reject로 분리
// reject는 catch에 등록된 callback 실행, resolve는 then에 등록된 callback 실행
function getUsersPromise(params){
	return new Promise((resolve, reject) => {
		getUsers(params, (err, users) => {
			if(err){
				reject(arr);
				return;
			}
			resolve(users);
		});
	});
}
```

4. `Async-await`: `promise` 의 단점을 보완한 비동기 코딩 방식, `promise` 의 다른 문법

```javascript
// async-await: 리턴 값은 promise
// await 한 promise 함수가 완료될 때까지 다음 라인으로 넘어가지 않음
// 순차적 프로그래밍처럼 작성 가능하다.
async function doSomething() => {
	const r1 = await promise1();
	const r2 = await promise2(r1);
	const r3 = await promise3(r1, r2);
	...
	return r3;
}

doSomething().then(r3 => {
	console.log(r3);
});

// err처리
async function doSomething(msg) => {
	try {
		const r1 = await promise1();
		console.log(r);
	}catch(e){
		console.log(e)
	}
}

// parallel run: promise 함수를 동시에 실행시키고 등록된 모든 함수가 마무리되면 결과값을 한꺼번에 반환
// 총 2초의 시간 소요
async function parallel(){
	const [r1, r2] = await Promise.all([
		promise1(),
		promise2(),
	]);
	console.log(r1, r2);
}

// 총 3초의 시간 소요
async function doSomething() => {
	const r1 = await promise1();
	const r2 = await promise2();
	console.log(r1, r2)
}
```

5. `callback-hell` : `promise chaining` 으로 해결
6. `promise-hell`: `async-await` 으로 해결
7. 대부분 가독성이 좋은 `async-await` 을 사용하지만, 상황에 따라 `callback`, `promise` 를 구사할 줄 알아야 한다.

### ❏ 이벤트 루프

1. 이벤트를 처리하는 반복되는 동작(loop)
2. `node.js` 가 비동기 - 이벤트 동작을 처리하는 일련의 반복 동작이며, 비동기 코딩이 어떤 순서로 수행되는지에 대해 이해할 수 있다.
3. 브라우저와 `node.js` 의 이벤트 루프는 기본적인 동작방식에 큰 차이가 없음. 이벤트루프의 기본적인 동작 원리를 이해하는 것이 중요하다.
4. `call stack`: `LIFO` 스택, 이벤트 루프는 콜스택이 비어있을 때까지 스택의 함수를 실행한다.
5. `message queue`: `setTimeout` 같은 지연실행 함수를 등록하는 `FIFO` 큐, 콜스택이 비어있을 경우 이벤트 루프에 의해 등록된 함수를 콜 스택에 추가한다.(setTimeout은 콜스택이 비어있을 때 실행)
6. `job queue`: `Promise` 에 등록된 콜백을 등록하는 `FIFO` 큐, 상위 함수가 종료되기 전에 콜스택이 비어있지 않더라도 잡큐에 등록된 콜백을 콜스택에 추가한다.(promise는 상위함수가 종료되기 전 실행)

### ❏ npm

1. `npm(node package manager)`: `node.js` 프로젝트를 관리하는 필수적인 도구(온라인 저장소 + 커맨드라인 도구)
2. `npm 저장소`: 필요한 라이브러리나 도구를 손쉽게 검색 가능. `node.js` 의 인기로, 거대한 생태계를 보유
3. 커맨드라인 도구: 프로젝트 관리를 위한 다양한 명령어 제공(프로젝트 설정 / 관리, 프로젝트 의존성 관리)
4. `npm init`: 해당 디렉토리 안에서 `package.json` 이라는 파일을 만들고, 이 디렉터리는 `node.js` 프로젝트가 된다.
5. `package.json`: 프로젝트 관련 정보들이 저장되는 파일. 이 파일을 직접 수정하거나 `npm` 명령어를 사용하여 프로젝트의 정보를 수정할 수 있음
6. 의존성: 프로젝트 내에서 라이브러리를 관리하는 방법, 프로젝트가 실행되기 위해 라이브러리에 의존하기 때문에 이러한 라이브러리들을 `dependency(의존성)` 이라고 부른다.
7. 라이브러리: 특정 기능을 수행하는 코드의 묶음, 복잡한 기능을 직접 작성하지 않고, 다른 사람이 구현한 것을 사용하는 방법(`node.js` 에서는 패키지라고도 부른다.)
8. `npm install`(약어 `npm i`): 프로젝트 의존성 관리 가능(의존성 추가, 의존성 내려받기, 개발용 의존성 추가, 전역 패키지 추가)
9. `npm install [package-name]`: 필요한 패키지를 프로젝트에 추가한다. 추가된 패키지는 `package.json` 의 `dependencies` 안에 추가되며, `node_modules` 디렉터리에 저장된다.
10. `npm install [package-name] --save-dev`: 개발용 의존성은 배포 전까지만 사용하느 의존성(유닛 테스트 라이브러리 등)인데, `--save-dev` 옵션을 이용하면 개발용 의존성을 추가할 수 있다. 개발용 의존성은 `package.json-devDependencies` 에 추가된다. 기본적으로 `node_modules` 디렉터리는 코드 관리나 배포시에 업로드 하지 않는데, 의존성이 많아지면 용량이 너무 커지고 운영체제별로 실행되는 코드가 다른 경우가 존재하기 때문이다.
11. `npm install --production`: 프로젝트 배포시 개발용 의존성을 포함하지 않고 내려받는다. `package.json-dependencies` 만 `node_modules` 에 내려받는다.
12. `npm install [package-name]@[version]`: `~1.13.0`: 1.13.x버전 설치, `~^1.13.0`: 1.x.x 버전 설치, 가장 왼쪽의 0이 아닌 버전을 고정, `0.13.0`: 0.13.0 버전만 설치(버전이 달라 오류가 날 때 주로 사용)
13. 프로젝트에 의존성을 추가하면 `package-lock.json` 이라는 파일이 생성됨. 프로젝트에 의존성을 추가하면 자동으로 `^`최신버전으로 추가가 되는데, 의존성 버전이 갑자기 변경되지 않도록, 설치된 버전을 고정하는 역할을 한다.
14. `npm install [package-name] —global`: 패키지를 전역 패키지 디렉토리에 내려받는다. 커맨드라인 도구들을 주로 전역 패키지로 추가해서 받음(`express-generator,pm2`)
15. 로컬 패키지: `package.json` 에 선언되어 있고, `node_modules` 에 저장된 패키지
16. 전역 패키지: `npm install -g` 를 통해 내려받아, 전역 패키지 저장소에 저장된 패키지
17. 전역 패키지도 프로젝트에서 사용할 수 있으나, 프로젝트의 의존성이 `package.json` 내에 명시적으로 선언되어 있는 것이 프로젝트 관리의 좋은 방향이다.
18. `npm remove [package-name]`: 의존성 패키지를 삭제한다. `dependencies`, `devDependencies` 에서 삭제하고 `node_modules` 에서도 삭제한다.
19. `npm run [script-name]` : 스크립트(간단한 동작을 수행하는 코드)를 실행한다.
20. `npm script` : 의존성 패키지를 사용할 수 있음
21. `npm test`: 코드 유닛테스트 등에 사용
22. `npm start`: 프로젝트 실행
23. `npm stop`: 프로젝트 종료
24. `run` 을 제외하고 사용할 수 있을뿐, `npm` 내부적으로 코드를 제공해 주는것은 아니다.

### ❏ npx

1. `npm` 패키지를 설치하지 않고 사용할 수 있게 해주는 도구, 프로젝트에 추가하거나 전역 패키지로 추가하지 않고 `npx` 를 이용하여 바로 실행할 수 있음
2. `gist` 코드를 다운받지 않고 바로 실행 가능(코드를 잘 확인하고 실행해야 함)

```javascript
// npm
npm i cowsay -g
cowsay hi

// npx
npx cowsay hi
npx node@12 index.js
```

### ❏ module

1. 간단한 프로그램이라면 파일 하나로도 가능, 프로젝트가 커지면 기능에 맞게 코드를 분리하는 것이 중요하다. 모듈은 코드를 분리하기 위한 방법
2. 반복되는 코드는 모듈로 분리하여 사용(재사용성 증가)
3. 패키지는 모듈의 모음, `npm` 패키지들은 많은 모듈을 포함하고 있는 코드 모음
4. `process`: 현재 실행프로세스 관련 기능 제공(`arch`, `argv`, `env`, `abort`, `kill`, `exit`)
5. `fs`: 파일 입출력을 하기 위해 사용(`readFile`, `writeFile`, `watch` 로 파일 / 디렉터리 변경 이벤트 감지)
6. `http`: `http` 서버, 클라이언트를 위해 사용, `createServer` 함수로 서버 생성, `request` 함수로 `http` 요청 생성
7. 기타 기본제공 모듈 확인하기: <a href='https://nodejs.org/dist/latest-v14.x/docs/api/'>node.js/doc</a>

### ❏ 모듈의 작성과 사용

1. `require` 함수를 통해 모듈을 `load` 할 수 있음
2. 의존성 패키지, 직접 작성한 모듈 사용 가능
3. `node.js` 의 모듈은 첫 `require` 시 `cache` , 두 번 실행하지 않음
4. 모듈 코드를 여러 번 실행하기 위해선 함수 모듈로 작성
5. 의존성 패키지들은 `require('package-name')` 로 `load` 가능하다. 패키지를 사용하려면 `node_modules` 에 내려받아져 있어야 함

```javascript
const name = "elice";
const age = 5;
const nationality = "korea";

// 모듈의 기본적인 사용법
// 모듈이 load 될 때 사용될 값을 module.exports로 내보냄
module.exports = {
    name,
    age,
    nationality,
};

// 변수명으로 export 하는 모듈 작성하기
// 모듈을 object로 만들고, 각 key - value를 지정해서 내보냄
exports.name = name;
exports.age = age;
exports.nationality = nationality;

const student = require("./elice"); // { name: "alice", age: 5, nationality: "korea" }

// 함수를 export하는 모듈
module.exports = (name, age, nationality) => {
    return {
        name,
        age,
        nationality,
    };
};

// npm 패키지 모듈
const dayjs = require("dayjs");
console.log(dayjs());

// 직접 작성한 모듈
const myModule = require("./my-module");
console.log(myModule);

// 함수형 모듈: 함수형은 load한 즉시 실행되지 않음
const myFunctionModule = require("./my-function-module");
console.log(myFunctionModule(name, age, nationality));

// json 모듈: json파일도 load가능, object로 자동파싱
const myData = require("./my-data");
console.log(myData);
```

### ❏ ES Module

1. ES6에서 등장한 JS의 공식적인 표준 모듈
2. JS는 기본적으로 모듈을 제공하지 않았다.
3. `node.js` 는 독자적인 방식을 통해 모듈을 지원하고 있었다(common js)
4. ES module의 등장으로 `node.js` 에서는 2가지 모듈을 지원해야한다.
5. `commonjs` 는 `module.exports`, `require` 로 모듈을 사용, `ES module` 은 `export` 와 `import` 로 모듈을 만들고 사용
6. 현재 `ES Module` 은 `node.js` 에서 기본적으로 사용하기에 제약이 많다.(프로젝트 타입을 `module` 로 변경, `commonjs` 모듈 `import` 시 문제 발생 등)

### ❏ 웹의 이해

1. 웹 서비스는 기본적으로 `HTTP` 요청과 응답의 반복으로 이루어짐. `HTTP` 요청은 사용자가 어떤 데이터가 필요한지를 서버에게 알리는 역할, `HTTP` 응답은 `HTTP` 요청에 해당하는 적절한 데이터를 전달하는 역할

![](https://images.velog.io/images/abcd8637/post/8709385a-0f67-4f2c-9cb0-b856268bea83/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-01%2013.54.35.png)

2. 정적 웹(Web 1.0): 사용자와 상호작용하지 않는 페이지 - 단방향 통신, `Link` 를 통한 페이지 이동 정도만 가능, 일반적으로 변하지 않는 `html` 파일로 제공
3. 동적 웹(Web 2.0): 사용자와 상호작용을 함 - 양방향 통신, 구글 맵, 웹, 채팅 등 사용자가 다양한 기능을 수행할 수 있음, `FE` 와 `BE` 가 유기적으로 통신하며 동작한다. 현대적인 웹은 대부분 동적 웹이다.
4. `CSR` : 프론트엔드에서 사용자가 페이지에서 보는 동적인 부분을 대부분 처리하는 방식(사이트가 변하는 부분을 프론트엔드에서 처리, 페이지 리소스들이 미리 정의, `API` 통신이용, `API` 호출이 완료된 후에 보여준다. 복잡한 프로젝트 구성, 개발 사이즈가 커진다.)
5. `SSR`: 백엔드에서 페이지 대부분의 영역을 처리해서 프론트엔드로 전달하는 방식(프론트엔드는 `HTTP` 응답을 받아 화면에 표시, 백엔드에서 필요한 데이터가 포함된 페이지를 만들어서 `HTTP` 응답에 전달, 백엔드에서 `HTML` 파일을 작성해서 프론트로 전달, 쉬운 구성, 작은 개발사이즈, 로딩이 느려보이고, 페이지가 이동하면 페이지가 깜빡인다.)
6. 웹서버는 `HTTP` 요청과 `HTTP` 응답으로 이루어지는데 클라이언트는 서버로 `HTTP` 요청을 보내고, 서버는 `HTTP` 응답을 보낸다.

### ❏ 웹 프레임워크

1. 웹 서비스에 필요한 기능들을 제공해주는 다양한 도구들의 모음, 필요한 부분만 집중해서 개발 할 수 있음
2. `HTTP 요청`, `HTTP 응답`, `라우팅`, `HTML Templating`
3. 라우팅: `HTTP` 요청에 따라 알맞은 응답을 보내주는 경로를 설정하는 일
4. `HTML Templating`: `SSR` 을 구현하기 위한 방법, `SSR` 에서 응답으로 보낼 `HTML` 을 서버에서 작성하기 위해 `HTML Template` 를 통해 미리 페이지의 뼈대를 작성 가능
5. `node.js` 의 다양한 웹 프레임워크: `Express.js`, `Koa.js`, `Nest.js`, `Hapi`, `Sails.js`, `Meteor.js` 등등

### ❏ Express.js 시작하기

1. `node.js` 웹 프레임워크 중 가장 유명한 웹 프레임워크
2. 필요에 따라 유연하게 구조 설정 가능
3. 다양한 미들웨어를 통해 필요한 기능을 간단하게 추가 기능
4. 모든 동작이 명시적으로 구성되기 때문에, 웹 프레임워크의 동작 방식을 이해하기 가장 좋은 프레임워크
5. `npm init express`
6. `express-generator`: 프로젝트 생성기, 리액트의 `CRA` 와 비슷함

```javascript
// npm 시작
npm i -g express-generator
express my-web
cd my-web
npm i
npm start

// npx 시작
npx express-generator
cd my-web
npm i
npm start
```

### ❏ Express.js 구조

![](https://images.velog.io/images/abcd8637/post/0d5266c7-d607-4288-8b5a-0b8863ae3cfe/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-01%2014.21.14.png)

### ❏ Express.js 동작방식

1. `express-generator` 로 만들어진 프로젝트 디렉토리에 접근하여, `npm start` 로 `Express.js` 프로젝트를 실행할수 있고 `[localhost:3000](http://localhost:3000)` 에 접속하여 페이지를 확인할 수 있다.

```javascript
1. localhost:3000 접속
2. app.js -> app.use('/', indexRouter);
3. routes/index.js -> router.get('/', ...)
4. routes/index.js -> res.render('index', ...)
5. views/index.jade
```

2. app.js: `express()` 로 생성되는 `app` 객체를 확인할 수 있다. `Express.js` 의 기능을 담은 객체
3. 라우팅: `app라우팅`, `express 라우팅`
4. `path parameter`: 주소의 일부를 변수처럼 사용할 수 있다.

```js
1. /users/:id - /users/123, /users/456 등으로 접속했을 때 라우팅 적용
2. /messges/:from-:to /message/123-456/ 등으로 접속했을 때 라우팅 적용
```

5. `request handler - request`: 라우팅에 적용되는 함수, `HTTP` 요청과 응답을 다룰 수 있는 함수로, 설정된 라우팅 경로에 해당하는 요청이 들어오면 `Request handler` 함수가 실행됨

![](https://images.velog.io/images/abcd8637/post/c0917c7f-e341-426f-9d3d-47833c4ec7e5/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-01%2015.02.32.png)

```javascript
// 설정된 라우팅 경로에 해당하는 요청이 들어오면 `request handler` 함수를 실행한다.
router.get("/:id", (req, res) => {
    const id = req.params.id;
    res.send(`hello ${id}`);
});
```

6. `resquest-handler - response`: HTTP 응답을 처리하는 객체, HTTP 응답의 데이터를 전송하거나, 응답 상태 및 헤더를 설정할 수 있음

![](https://images.velog.io/images/abcd8637/post/491ccb9e-2905-4a01-97df-f766b09f0b0f/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-01%2015.03.04.png)

```javascript
// path parameter
const express = require("express");

const app = express();

app.get("/", (req, res) => {
    res.send("hi");
});

// path parameter 사용하기
app.get("/say/:greeting", (req, res) => {
    const { greeting } = req.params;
    res.send(greeting);
});

app.listen(8080);

// router 연결
const express = require("express");
const userRouter = require("./routes/users");

const app = express();

app.get("/", (req, res) => {
    res.send("OK");
});

/* 라우터를 '/users' 경로에 연결 */
app.use("/users", userRouter);

app.listen(8080);
```

---

## 📍 28일차 12.2.목(실시간 강의)

바쁘게 살면 시간이 빨리 가는것처럼 느껴지는 특징이 있는데, 지금의 내가 그렇다. 엄청 많이 한것같지도 않은데 벌써 목요일이다. 얼른 수료하고 취업전선에 뛰어들고 싶다. 오늘은 `npm`, `API`, `RESTAPI`, `express.js`, `middleware`에 관한 내용을 배웠다.

### ❏ npm

1. `npm init`: `package.json` 파일 생성
2. `package.json`: 모듈을 관리하는 파일
3. `package.json - dependencies`: 내가 설치한 라이브러리를 보여준다. 버전 앞에 `^`는 버전을 대략적으로 보여준다. 업데이트 부분에서 자세하게 다룬다.
4. `npm cache clean -f`: 캐쉬 강제로 비우기
5. `node_modules`: 내가 설치한 모듈의 자세한 정보(내 컴퓨터 - programfiles라고 생각하면 편하다.)
6. 다른 개발자들과 협업할때는 `package.json`에 있는 모듈의 버전말고 `package-lock.json` 파일에 있는 모듈의 버전을 알려줘야 에러를 방지할 수 있다. `package.json`은 버전이 대략적으로만 나와있다.
7. `npm install [package-name] --save-dev`: 개발용으로 모듈을 설치한다.
8. `npm install \ yarn install`: `node_modules`가 없을 때 `package.json` 파일을 참고하여 `node_modules`를 설치해준다. (git clone 하고나서 사용하면 된다.)
9. `npm install --production`: 개발용 의존성(`devDependencies`) 모듈은 제외하고, `dependencies`에만 설치한다.
10. `sementic versioning`: 0.0.0(앞에서부터 `major`, `minor`, `patch` 순서로 부른다.)
11. `npm update [package-name]`: 버전 앞에 `^`가 붙어있으면 두번째 자리인 `minor`한 최신 버전을 업데이트한다. 버전 앞에 `~`가 붙어있으면 세번째 자리인 `patch` 를 최신 버전으로 업데이트 한다.
12. `npm install -g [package-name]`: 글로벌로 모듈을 설치한다.
13. `yarn add [package-name]`: 모듈 설치
14. `yarn add -D [package-name]`: 개발용 모듈 설치
15. `yarn remove [package-name]`: 모듈 제거
16. `scripts`: `CLI` 명령어 설정

### ❏ API

1. 내장 라이브러리로 사용하다 외부에 데이터를 저장해서 서버와 통신기기간에 정보를 주고받는 값을 말한다.
2. `soap`, `rest`: 정보 교환의 표준성 개발을 의미하는데, `soap`는 `xml` 기반으로 `html`처럼 코드가 복잡해서 이를 보완하기 위해 나온 것이 `rest`다. `rest`는 `json` 기반으로 코드가 간결하다.
3. `--print=hHbB`: 헤더를 통해 보낸값과 받은 값을 보여주는 명령어
4. `npm install --save-dev nodemon`: `node.js`의 코드가 바뀔 때마다 자동으로 새로고침해주는 라이브러리, 개발용으로만 사용하고 배포할때는 사용하지 않는 것을 권장한다.
5. `?`: 매개변수(쿼리끼리는 `&`로 구분한다.)

```json
http://localhost:9999/routes/is_odd_2?number=13&number3=1
```

6. `RESTAPI`: `API`지만, 웹을 통해 원하는 요청을 보내고, 그 요청을 받는 것. `URL`로 요청을 보내면 `HTTP` 상태 코드와 함께 결과값을 보낸다. 요청을 명세에 맞추어 보내야 `FE`, `BE`간에 원활한 통신이 가능하다. (`swagger`: RESTAPI 명세 작성 사이트)

```javascript
// GET
1. 데이터를 읽거나 검색할때 사용하는 메서드 (성공시 200 return)
2. GET 요청은 읽을 때만 사용, 수정될 때는 사용지 않아야 한다.

// POST
1. 주로 새로운 리소스를 생성할 때 사용 됨(일반적으로 성공 시 201return)
2. POST는 HTMl body나 JSON으로 전달 함
```

7. `.dotenv`: 함부로 노출할 수 없는 값(APIKEY, password 등)을 `env` 폴더에 저장해서 사용한다. (`gitignore`를 꼭 적용하자.)

### ❏ MiddleWare

1. `서버`와 `클라이언트`사이에 존재, 각기 분리된 2개 이상의 프로그램 사이에서, 매개역할을 하거나 연합시켜주는 프로그램. `next()`를 작성하지 않으면 해당 미들웨어에서만 실행하고 다음 미들웨어로 넘어가지 않는다.
2. `Express.js`에서 미들웨어는 순차적으로 코드를 실행한다.
3. 인증파트에서 `middleware`를 사용하고 인증이 되었으면, 내 주문, 선물함, 결제내역 등을 보는데 사용 될 수 있다.
4. `html form methods="POST"`로 설정하면 `URI` 뒤에 `?`형태로 쿼리값이 넘어온다

```javascript
// middle ware의 절차적인 프로세스1
app.use('/', (req, res, next) => {
	console.log('middelware 1');
	next();  // next가 없으면 넘어가지 않는다.
}

app.use('/', (req, res, next) => {
	console.log('middelware 2');
}

// middle ware의 절차적인 프로세스2: middleware2, hello, express
app.use('/', (req, res, next) => {
	console.log('middelware 2');
	res.send("hello, express!');
}

app.use('/', (req, res, next) => {
	console.log('middelware 1');  // 위 app에서 next가 없기때문에 실행되지 않는다.
}

// middleware에서 값을 넘겨주기
app.use('/', (req, res, next) => {
	console.log('middelware 1');
	const requestdAt = new Date();
	req.requestdAt = requestdAt;
	next();
}

app.use('/', (req, res, next) => {
	console.log(req.resquestedAt);  // Date
}

// promise 사용하기
app.use('/', (req, res, next) => {
	console.log('middelware 1');
	const fileContent = await fs.promises.readFile(".gitignore");
	req.fileContent = fileContent;
	next();
}

// 경로 설정
const express = require('express');
const app = express();
const PORT = 5000;

const fs = require('fs');

app.get('/',(req, res) => {
	res.send("Root - GET")
})

app.post('/',(req, res) => {
	res.send("Root - POST")
})

// ?: 앞의 값이 있어도 되고 없어도 된다.(option)
app.get('/ab?cd',(req, res) => {
	res.send("Root - GET")
})

// +: 앞의 값이 여러개가 와도 된다.
app.get('/ab+cd',(req, res) => {
	res.send("Root - GET")
})

// *: *자리에 아무문자나 와도 된다.
app.get('/ab*cd',(req, res) => {
	res.send("Root - GET")
})

// ()?: ()안의 값은 묶어서 사용한다.
app.get('/a(bc)?cd',(req, res) => {
	res.send("Root - GET")
})

// $: $앞의 값을 포함해야 한다
app.get('/abcd$/',(req, res) => {
	res.send("Root - GET")
})

// []: 배열 안의 값이 매칭될때
app.get(['/abc', '/xyz'],(req, res) => {
	res.send("Root - GET")
})

// 분기처리 전
app.get('/users',(req, res) => {
	res.send("Root - GET")
})

app.get('/users/:id',(req, res) => {
	res.send("Root - GET")
})

// 분기 처리 후
const userRouter = express.Router();
app.get('/',(req, res) => {
	res.send("Root - GET")
})
app.get('/:id',(req, res) => {
	res.send("Root - GET")
})
app.use('/users', userRouter);

// path parameter
userRouter.param('id', (req, res, next, value) => {
	req.user = USERS[value];
	next()
})

userRouter.get('/:id', (req, res) => {
	res.send(req.user);
})

// path parameter2
userRouter.post('/:id/nickname', (req, res) => {
	const { user } = req;
	const { nickname } = req.body;
	user.nickname = nickname;
})
```

5. 에러핸들링

```javascript
const user = USERS[value];

if (!user) {
    const err = new Error("User not found");
    err.statusCode = 404;
    throw err;
}

req.user = user;
next();

// express에서 4개의 인자를 준다. error 핸들링 미들웨어로 인식
app.use((err, req, res, next) => {
    res.statusCode = err.statusCode || 500;
    res.send(err.message);
});
```

---

## 📍 29일차 12.3.금(온라인 강의)

어제에 이어서 `express.js` 사용법 그리고 `middleware`, `postman`을 이용한 `RESTAPI`실습을 배웠다. 실습을 하면서 느낀건 <a href='https://velog.io/@abcd8637/%EC%B5%9C%EC%A2%85%EB%A9%B4%EC%A0%91-SW-%EC%A0%95%EA%B8%80%EC%82%AC%EA%B4%80%ED%95%99%EA%B5%90-%ED%9B%84%EA%B8%B0'>예전</a>에 정글사관학교 면접보기 전 과제 시험에서 게시판 `CRUD` 구현하는 과제가 있었는데, `R, U` 기능을 해결하지 못했었다. 이전의 기억을 트라우마로 갖고있어 `CRUD`를 조금 회피(?)하게 되었지만, 이번에 완전히 정복하겠다는 의지로 공부했다. 나중에 백엔드 엔지니어와 협업할 때 서버에 관해 대화를 할 때 말이 잘 통할정도로 성장하고 싶다.

### ❏ middleWare

1. 미들웨어는 `Express.js`동작의 핵심이다. `HTTP` 요청과 응답 사이에서 단계별 동작을 수행해주는 함수를 뜻한다.
2. `HTTP` 요청이 들어온 순간부터 `express.js` 가 실행된다. 미들웨어는 `HTTP` 요청과 응답 객체를 처리하거나, 다음 미들웨어를 실행 할 수 있다.(순차적으로 처리한다.) `HTTP` 응답이 마무리 될때까지 미들웨어 동작 사이클이 실행된다.
3. `req`, `res`, `next` 를 가진 함수를 작성하면 해당 함수는 미들웨어를 동작할 수 있다.

```javascript
1. req: HTTP 요청을 처리하는 객체
2. res: HTTP 응답을 처리하는 객체
3. next: 다음 미들웨어를 실행하는 함수
```

4. `RouteHandler`: 미들웨어의 한 종류, 라우팅 함수(get, post, put, delete 등)에 적용된 미들웨어, 일반적인 미들웨어와는 다르게 path parameter를 사용할 수 있다. next 함수가 호출되지 않으면 미들웨어 사이클이 멈추기 때문에 주의할것

```javascript
const logger = (req, res, next) => {
    console.log(`Request ${req.path}`);
    next();
};

const auth = (req, res, next) => {
    if (!isAdmin(req)) {
        res.send("Not Authorized");
        return;
    }
    next();
};
```

5. `middleware`는 적용되는 위치에 따라 어플리케이션 미들웨어, 라우터 미들웨어, 오류처리 미들웨어로 분류가능하다. 필요한 동작 방식에 따라 미들웨어를 적용할 위치를 결정한다.

```javascript
// 애플리케이션 미들웨어
// use나 http method 함수를 사용하여 미들웨어를 연결 할 수 있다.
app.use((req, res, next) => {
	console.log(`Request ${req.path}`);
	next();
)

app.use(auth);

app.get('/', (req, res, next) => {
	res.send('Hello express!')
})

// 라우터 미들웨어
// 특정경로의 라우팅에만 미들웨어를 적용하기 위한 방법
router.use(auth);

router.get('/', (req, res, next) => {
	res.send('Hello Router!')
})

app.use((req, res, next) => {
	console.log(`Request ${req.path}`);
	next();
)

app.use('/admin', router)

// 미들웨어 서브스택
// 여러개의 미들웨어를 동시에 적용할 수 있음. 주로 한개의 경로에 특정해서 미들웨어를 적용하기 위해 사용
app.use(middleware1, middleware2...);

app.use('/admin', auth, adminRouter);

app.get('/', logger, (req, res, next) => {
	res.send('Hello Router!')
})
```

6. 오류처리 미들웨어: 일반적으로 가장 마지막에 위치하는 미들웨어, 다른 미들웨어와 달리 err, req, res, next 네가지 인자를 가지며, 앞선 미들웨어에서 next 함수에 인자가 전달되면 실행됨

```javascript
// next에 인자로 넘기면 중간을 건너뛰고 마지막 오류처리 미들웨어가 실행된다.
app.use((req, res, next) => {
    if (!isAdmin(req)) {
        next(new Error("Not Authorized"));
        return;
    }
    next();
});

app.get("/", logger, (req, res, next) => {
    res.send("Hello Router!");
});

app.use((err, req, res, next) => {
    res.send("Error Occurred!");
});
```

7. 함수형 미들웨어: 하나의 미들웨어를 작성하고, 작동모드를 선택해서 사용하고 싶을 경우, 미들웨어를 함수형으로 작성하여 사용한다. (예, API 별로 사용자의 권한을 다르게 제한하고 싶은 경우)

```javascript
const auth = (memberType) => {
	return (req, res, next) => {
		if(!checkMember(req, memberType)){
			next(new Error(member not ${memberType}));
			return;
		}
		next();
	}
}

app.use('/admin', auth('admin'), adminRouter);
app.use('/users', auth('member'), userRouter);
```

8. 요약: 미들웨어는 HTTP 요청과 응답 사이에서 작동하는 함수, req, res, next 를 인자로 가질 수 있다. app 혹은 router 객체에 연결해서 사용가능하다. next 에 인자로 넘기면 오류처리 미들웨어가 실행된다. 미들웨어에 값을 설정하고 싶다면 함수형 미들웨어로 설정하라.

### ❏ REST API

1. `REST` 아키텍쳐를 준수하는 웹 `API`, `RESTFul` 이라고도 부른다.
2. `API` : 서비스나 프로그램간에 미리 정해진 기능을 실행할 수 있도록 하는 규약
3. `REST`: 웹에서 자료를 전송하기 위한 표현 방법의 아키텍쳐, 기본적인 REST 가이드를 따르면 조금 더 좋은 구조의 API를 구성할 수 있음
4. API의 동작을 `HTTP method + 명사형 URL` 으로 표현함. `/posts` `url` 은 게시글 자원을 가리킨다고 할 때 http method(get, post, put, delete)와 결합하여 api 동작을 정의한다.
5. `url` 표현법: 자원을 복수형으로 표현하고 하나의 자원에 접근은 복수형 + 아이디를 통해 특정 자원에 접근한다. 예를 들어 `/posts` 가 게시글 전체라고 한다면, `/posts`은 1번 게시글이라는 자원을 표현함
6. `rest api` 는 `url` 을 통해 자원을 계층적으로 표현한다. `/users/1/posts` 라는 `URL` 은 1번 유저의 게시글 전체라는 자원을 나타낸다
7. restapi는 rest 아키텍쳐를 준수하는 웹 api를 의미하며, rest 아키텍쳐를 준수하는 간단한 방법으로 url을 통한 자원의 표현 방법과 http method를 통한 api 동작의 정의 정도만 사용해도 훌륭한 rest api를 구현할 수 있다.

### ❏ JSON

1. JS에서 객체를 표현하는 표현식으로 시작했다. 데이터를 표현하는 방법이 단순하고 이해하기 쉬워서 데이터를 전송할 때 많이 사용한다.
2. 웹 api는 데이터를 문자열로 전송한다. 어떤 객체를 웹 api를 통해 문자열로 전달하기 위해 json을 사용한다.
3. `value` 에는 어떤 값이라도 사용 될 수 있다.

### ❏ Express.js로 REST API 구현하기

1. 간단한 메모의 작성, 삭제, 확인기능 api 구현
2. express-generator를 사용하지않고 MVC패턴 구현

### ❏ MVC 패턴

1. 프로젝트의 기능들을 어떻게 분리할지에 대한 하나의 구성 방법
2. model: 데이터에 접근하는 기능, 데이터 그 자체, 데이터의 읽기 쓰기는 `model` 을 통해서만 표현
3. view: 데이터를 표현하는기능, controller에 의해 데이터를 전달받고 화면에 표시하는 기능
4. controller: model을 통해 데이터에 접근하여 처리 결과를 view에 전달하는 기능, 라우팅 함수가 controller기능을 수행한다.
5. `express.js` 는 기본적으로 `HTTP body` 에 전달되는 `JSON` 데이터를 처리하지 못함. `express` 에서 기본적으로 제공해주는 `express.json()` 미들웨어를 사용해야 `JSON` 데이터를 사용할 수 있 `a pp.use(express.json())`
6. 가장 마지막 미들웨어로 오류 처리 미들웨어를 적용하면 모든 라우팅에 공통적인 오류처리 로직을 적용할 수 있음

```javascript
// 이전에 next()에 인자로 넘겨줌
app.use((err, req, res, next) => {
    res.status(500);

    res.json({
        result: "fail",
        error: err.message,
    });
});
```

7. 모든 라우팅이 적용 된 이후 사용되는 미들웨어는 설정된 경로가 없는 요청을 처리하는 Route Handler 로 동작한다. Express.js 는 기본적으로 404 페이지를 가지고 있지만, 직접 처리가 필요할 때 Route Handler 를 추가한다.

```javascript
app.use((req, use, next) => {
    res.status(404);
    res.send({
        result: "fail",
        error: `Page not found ${req.path}`,
    });
});
```

### ❏ postman

1. API 테스트 도구로 HTTP 요청을 손쉽게 작성하여 테스트해볼 수 있게 도움을 준다.

### ❏ 미들웨어 작성과 사용

이하 실습 코드 생략

---

## 📍 30일차 12.4.토(온라인 강의)

오늘은 `mongoDB`와 `express.js`를 연동하여 `CRUD`하는 법을 배웠다. 예전에 `mongoDB`를 이용하여 최신 기사를 한눈에 보여주는 <a href='https://blog.naver.com/abcd8637/222152180429'>지금 뉴스!</a> 프로젝트를 진행했으나, `AWS` 무료 티어기간이 끝나서 취소하는 바람에 서버를 닫았다. 그때는 `Robo 3T` 프로그램으로 `mongoDB`를 조작했는데 이번에는 <a href='https://www.mongodb.com/ko-kr'>mongoDB</a> 홈페이지에 `cloud` 기능과 연동하는 법을 배웠다. mongoDB 홈페이지에서 다루니까 훨씬 `UX`가 좋았다.

### ❏ MongoDB

1. 대표적인 `NoSQL`, `Document DB` mongo는 Humongous에서 따온 말로, 엄청나게 큰 DB, 대용량 데이터를 처리하기 좋게 만들어짐
2. `NoSQL` (Not Only SQL): 구조화된 질의어를 사용하지 않는 데이터베이스, 자료간의 관계에 초점을 두지 않음. 데이터를 구조화하지 않고 유연하게 저장함
3. `RDB` (Relational Database): 관계형 데이터 베이스, 자료들의 관계를 주요하게 다룸, SQL 질의어를 사용하기 위해 데이터를 구조화 해야함
4. 왜 `NoSQL`을 사용하는가? `SQL`을 사용하기 위해서는 데이터를 구조화하는 것이 필수이다.(`DDL`) 스키마에 정의된 데이터가 아니면 저장할 수 없는 제약이 따르는데, `NoSQL` 을 사용하면 사전작업 없이 DB 를 사용할 수 있다.(DB크기에 관여하지 않고 프로젝트를 빠르게 진행할 수 있음)

```SQL
// MySQL
CREATE DATABASE simple_board

CREATE TABLE posts (
	id NOT NULL AUTO INCREAMENT
	title VARCHAR(30),
	content TEXT,
	PRIMARY KEY(id)
)

INSERT INTO posts (title, content)
VALUES
('first title', 'first content'),
('second title', 'second content')

// MongoDB
use simple_board
db.posts.insert([
	{
		title: 'first title',
		content: 'first content'
	},
	{
		title: 'first title',
		content: 'first content'
	}
])
```

5. NoSQL은 다양한 종류가 있지만, 대표적으로 자료를 문서로 저장하는 `DocumentDB` 가 일반적, 이 외에, `key-value`, `Graph`, `large collection` 등의 `NoSQL DB` 가 존재한다.
6. `mongoDB` 를 직접 설치하거나 `Cloud` 서비스를 사용할 수 있음. 직접 설치하면 귀찮고 어렵지만, 원하는 만큼 얼마든지 데이터를 사용할 수 있음. `Cloud` 를 사용하면 쉽고 빠르게 시작 가능하지만, 사용량에 따라 요금이 부과된다.
7. 직접 설치하기: 직접 모든 DB 관련 설정을 해야한다. sharding 이나 replication 등의 작업이 필요할 때 운영지식과 노하우가 요구된다. 무료로 제공하는 community version 을 제공함
8. `mongoDB cloud`: 모든 DB 기능을 웹에서 관리 가능하다. 특별한 노하우없이 DB 운용 가능하고 `512MB`까지는 평생 무료로 사용가능
9. `mongoDB compass`: mongoDB에 접속하여 Database, collection, document 등을 시각화하여 관리할 수 있게 도와주는 도구, MySQL workbench 와 유사

### ❏ MongoDB의 기본 개념

1. `Database`: 하나 이상의 `collection` 을 가질 수 있는 저장소, `SQL`에서의 `database` 와 유사
2. `Collection`: 하나 이상의 `Document`가 저장되는 공간. SQL 에서의 table 과 유사하다. 하지만, collection 이 document 의 구조를 정의하지 않음
3. `Document`: `mongoDB` 에 저장되는 자료, SQL 에서 row 와 유사하지만, 구조제약 없이 유연하게 저장 가능, JSON 과 유사한 BSON 을 사용하여 다양한 자료형을 지원한다.
4. `document - objectID` : 각 document 의 유일한 키 값, SQL 의 primary key 와 유사하다. 하나씩 증가하는 값이 아닌 document 를 생성할 때 자동으로 생성되는 값(timestamp + random value + auto increament)

### ❏ Mongoose ODM

1. `ODM(Object Data Modeling)`: MongoDB의 collection에 집중하여 관리하도록 도와주는 패키지 Collection 을 모델화하여, 관련 기능들을 쉽게 사용할 수 있도록 도와줌
2. `MongoDB` 는 기본 `Node.js` 드라이버는 연결상태를 관리하기 어려움 이때, `Mongoose` 를 사용하면 간단하게 데이터베이스와의 연결상태를 관리해줌.
3. 스키마 관리: 스키마를 정의하지 않고 데이터를 사용하는 것은 NoSQL 의 장점이지만, 데이터 형식을 미리 정의 해야 코드 작성과 프로젝트 관리에 유용함. `Mongoose` 는 `Code-level` 에서 스키마를 정의하고 관리할 수 있게 해줌, 중간단계에서 체크해주고 관리함
4. `populate`: `mongoDB`는 `join` 을 제공하지 않음. `join` 과 유사한 기능을 사용하기 위해서 `aggregate` 라는 복잡한 쿼리를 사용하지만 `Mongoose` 에서 `populate` 를 사용하여 간단하게 구현할 수 있음

### ❏ Mongoose ODM 사용순서

1. 스키마 정의 → 모델 만들기 → 데이터베이스 연결 → 모델 사용
2. 스키마 정의: `Collection` 에 저장될 `Document` 의 스키마를 `Code-level` 에서 관리할 수 있도록 `schema` 를 작성할 수 있음. 다양한 형식을 미리 지정하여 생성, 수정 작업 시 데이터 형식을 체크해주는 기능을 제공함. `timestamps` 옵션을 사용하면 생성, 수정 시간을 자동으로 기록해 줌

```javascript
const { Schema } = require("mongoose");

const PostSchema = new Schema(
    {
        title: String,
        content: String,
    },
    {
        timestamps: true,
    }
);

module.exports = PostSchema;
```

3. 모델 만들기: 작성된 스키마를 `mongoose` 에서 사용할 수 있는 모델로 만들어야 함. 모델의 이름을 지정하여 `populate` 등에서 해당 이름으로 모델을 호출 할 수 있음

```javascript
const mongoose = require("mongoose");
const PostSchema = require("./schemas/board");
exports.Post = mongoose.model("Post", PostSchema);
```

4. 데이터베이스 연결하기: `connect` 함수를 이용하여 간단하게 DB 에 연결할 수 있음. `mongoose` 는 자동으로 연결을 관리해주기 때문에 직접 연결 상태를 체크하지 않아도 모델 사용 시 연결 상태를 확인하여 사용이 가능할 때 작업을 실행 함

```javascript
const mongoose = require("mongoose");
const { Post } = require("./models");
mongoose.connect("mongodb://localhose:27017/myapp");
```

### ❏ 모델 사용하기 - 간단한 CRUD

![](https://images.velog.io/images/abcd8637/post/5f2948d4-a672-49e9-bcd5-92c2d5ba714d/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-04%2012.09.12.png)

1. `CREATE`: create 함수를 사용하여 Document생성, create 함수에는 Document Object 나 (단일 Document) Document Object 의 Array 전달 가능(복수Document), create 는 생성된 Document 를 반환해줌

```javascript
const { Post } = require("./models");

async function main() {
    const created = await Post.create({
        title: "first title",
        content: "second title",
    });

    const multipleCreated = await Post.create([item1, item2]);
}
```

2. `FIND(READ)`: find 관련 함수를 사용하여 document 를 검색, query 를 사용하여 검색하거나 findById 를 사용하면 objectID 로 document 를 검색할 수 있음

```javascript
const { Post } = require("./models");
async function main() {
    const listPost = await Post.find(query);
    const onePost = await Post.findOne(query);
    const postById = await Post.findById(id);
}
```

3. `query` : MongoDB 에도 SQL where 와 유사한 조건절 사용 가능. MongoDB 의 query 는 BSON 형식으로 기본 문법 그대로 mongoose 에서도 사용 가능, {key: value}로 `exact match`

```javascript
Person.find({
    name: "AYW",
    age: {
        $lt: 20, // less then: 미만(and)
        $gte: 10, // grater then equal: 이상(and)
    },
    languages: {
        $in: ["ko", "en"], // in: 존재하면(and)
    },
    $or: [
        // or: acive이거나 true인 값 중 하나
        { status: "ACTIVE" },
        { isFresh: true },
    ],
});
```

4. `mongoose` 는 쿼리 값으로 배열로 전달하면 자동으로 `$in` 쿼리를 생성해준다.

```javascript
Person.find({ name: ["elice", "ted"] }); // { name: { $in: ['elice', 'ted' ]}}
```

5. `UPDATE`: update 관련 함수를 사용하여 document 를 수정, find~ 함수들은 검색된 document를 업데이트를 반영하여 반환해준다. 반면, update 는 기본적으로 $set operator 를 사용하여 document 를 통째로 변경하지 않는다.

```javascript
async function main() {
    const updateResult = await Post.updateOne(query, {});
    const updateResults = await Post.updateMany(query, {});
    const postById = await Post.updateOne(query, {});
    const onePost = await Post.findOneAndUpdate(query, {});
}
```

6. `DELETE` : delete 관련 함수들을 사용하여 document 삭제결과를 리턴한다. find~ 함수들은 검색된 document 를 반환해준다.

```javascript
async function main() {
    const deleteResult = await Post.deleteOne(query, {});
    const deleteResults = await Post.deleteMany(query, {});
    const onePost = await Post.findOneAndDelete(query, {});
    const postById = await Post.findByIdAndDelete(query, {});
}
```

7. `populate`: document 안에 document 를 담지 않고 objectID 를 가지고 reference 하여 사용할 수 있는 방법, document 에는 reference 되는 ObjectID 를 담고, 사용할 때 populate 하여 하위 Document 처럼 사용할 수 있게 해줌

```javascript
const Post = new Schema({
    user: {
        type: Schema.Types.ObjectId,
        ref: "User",
    },
    comments: {
        type: Schema.Types.ObjectId,
        ref: "Comment",
    },
});

const post = await Post.find().populate(["user", "comments"]);
```

### ❏ Express.js + Mongoose ODM

1. `Express.js` 는 프로젝트 구조를 자유롭게 구성할 수 있기 때문에 어느 부분에 `Mongoose ODM` 을 위치시키면 좋을지 적절한 위치를 결정하는 것이 중요
2. 일반적으로 `models` 디렉터리에 `Schema` 와 `Model` 을 같이 위치시킨다. `app` 객체는 어플리케이션 시작을 의미하는 부분으로 해당 부분에 데이터베이스 연결을 명시하는 `mongoose.connect` 를 위치한다. 특별한 제약이 있는것은 아니다.

![](https://images.velog.io/images/abcd8637/post/015977e8-b060-4a36-876b-28414b573f3c/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-04%2016.34.38.png)

3. `Express.js` 어플리케이션은 종료되지 않고 동작하기 때문에, 계속해서 DB 가 정상적으로 동작하는지 파악하기 위해 동작 중에 발생하는 DB 연결 관련 이벤트에 대한 처리를 하는 것이 좋음

```javascript
// connection events
mongoose.connect("----");
mongoose.connection.on("connected", () => {}); // 연결완료
mongoose.connection.on("disconnected", () => {}); // 연결끊김
mongoose.connection.on("reconnected", () => {}); // 재연결 완료
mongoose.connection.on("reconnectFailed", () => {}); // 재연결 시도 횟수 초과
```

### ❏ Sequelize ORM

1. `ORM`(Object-Relational Mapping): `MySQL`, `PostgreSQL` 등의 `RDBMS` 를 이용하는 간단한 방법 `ODM` 이 단순히 모델에 집중하여 관리하는 것에 반해, `ORM` 은 테이블 관계와 쿼리 등의 기능을 더욱 단순화하는 용도로 주로 사용
2. `sequelize` 도 연결을 관리하는 간단한 방법을 제공, `mongoose` 가 `mongoDB` 만 연결이 가능한데에 반해, `sequelize` 는 `MySQL`, `PostgreSQL` , `SQLite` 등 다양한 `RDBMS` 에 연결가능하다.
3. 나중에 `node.js`로 관계형 데이터베이스를 구현하고 싶으면 `Sequelize`를 공부하자.

```javascript
// connect db
const sequelize = new Sequelize("database", "usename", "password", {
    host: "localhost",
    dialect: "mysql",
});
```

4. 스키마 작성: `define` 을 통해 `Schema` 생성, `sequelize` 는 `Schema`가 `DDL도` 생성해준다.

```javascript
const User = sequelize.define(
    "User",
    {
        name: {
            type: DataTypes.STRING(10),
            allowNull: false,
        },
        age: {
            type: DataTypes.Integer,
        },
    },
    {}
);
```

5. 관계 정의: 테이블 간의 관계를 `Code-level` 로 관리 할 수 있다. 이를 이용하면 외래키 설정과 제약조건까지 `DDL` 로 생성한다. 또한 다대다 관계 설정을 통해 `relation table` 도 자동으로 생성한다.

```SQL
User.hasMany(Post);
Post.belongsTo(User);
Foo.belongsToMany(Bar);
Bar.belongsToMany(Foo);
```

6. 쿼리: Operator 를 이용해 SQL 쿼리를 코드로 작성 가능, 스키마의 관계 설정을 한 경우 include 를 사용하여 자동으로 join 쿼리 생성 가능

```SQL
User.findAll({
	where: {
		name: 'elice',
		age: {
			[Op.lt]: 20,
			[Op.gte]: 10.
		},
	},
	include: User,
})
```

7. `Synchronization`: `define`된 model 데이터를 바탕으로 DDL 을 자동으로 실행해줌. 직접 데이터베이스에 접속하여 테이블 생성 및 관리를 할 필요가 없음. 자동으로 생성된 DDL 을 따르지 않으면 테이블 관리가 어려워 짐

```javascript
sequelize.sync();
```

8. `Sequelize ORM` 를 사용하면 데이터베이스에 직접 DDL 을 사용하지 않고, JS 코드로 테이블 및 관계를 관리할 수 있다. 또한 RDB 의 어려운 점 중 하나인 join 을 includes 옵션을 통해 간단하게 사용할 수 있다.

---

## 📍 31일차 12.7.화 데이터 베이스 연동(실시간 강의)

이번주는 `node.js`를 바탕으로 `mongoDB`를 이용하여 데이터베이스를 연동하여 회원가입과 로그인 기능을 구현한다. 프론트엔드를 준비하고 있어 `DB`를 많이 공부하진 않았지만 이번 기회를 계기로 `DB`와 친해져보고 게시판 `CRUD`와 페이지네이션을 구현해보고 싶다.

### ❏ DataBase

1. 여러 사람이 공유하여 사용 할 목적으로 체계화하여 관리되는 데이터의 집합(`DBMS`에 의해 제어 됨)
2. 데이터 공유: 여러명이 동시에 공유하더라도 안정성, 정확성을 갖춤
3. 데이터 중복 최소화: 하나의 데이터베이스에 여러 테이블을 나누어 데이터 중복 최소화
4. 지속성: 데이터가 여러 군데에 산재해 있으면 동시에 관리하기 어렵고, 무결성 유지도 어려움, 데이터베이스는 `DBMS`에 의해 중앙집중적으로 관리되어 무결성 유지가 용이
5. 보안성: 중앙집중적으로 관리되기에 한 군데만 보안을 유지하면 됨
6. `ACID`: 원자성(Atomicity) - 트랜잭션 관련 작업이 모두 수행됐는지 확인, 일관성(Consistency) - 데이터가 언제나 일관성 있는 상태인지 확인, 고립성(Isolation) - 한 작업 수행시 다른 작업이 끼어들지 못하게 보장, 지속성(Durability) - 성공적으로 수행된 작업은 영원히 반영 즉 `ACID`는 데이터베이스 트랜젝션이 안전하게 수행된다는 것을 보장하기 위한 성질이다.
7. `SQL`은 `ACID`가 있는 대신 프로그램이 무겁지만 안전하다. 반대로 `NoSQL`은 `ACID`가 없는 대신에 프로그램이 `SQL`보다 가볍고 빠르다. 대신 어플리케이션단에서 보안을 강화시켜야 한다.
8. 수직확장: `SQL`에서 한 인스턴스를 키워 더 큰 로드를 감당한다. 이는 한계가 있다.
9. 수평확장: `NoSQL`에서 더 많은 인스턴스를 만들어 더 큰 로드를 감당한다. `NoSQL`은 데이터 구조가 정해져 있지 않아 인스턴스를 무제한 늘릴 수 있다.(운영비용이 받쳐준다면..)

### ❏ DBMS

1. Oracle: 가장 먼저 상업용으로 발표된 관계형 데이터베이스, DB시장 점유율 1위지만, 비용이 많이들고, 대기업에서 주로 사용한다.
2. MySQL: `MySQL`사에서 만든 오픈소스 데이터베이스, `Oracle`에 비해 대용량 데이터 처리는 어려움
3. PostgreSQL: 객체 관계형 데이터베이스 시스템, 오픈소스, 다양한 데이터베이스 객체를 사용자가 임의 생성가능
4. MariaDB 등등..
5. 열 = 필드 = 속성
6. 행 = 튜플 = 레코드

### ❏ NoSQL

1. `key-value`: `Redis`, `AWS DynamoDB`, `value`는 어떤 값이든 가능, 가장 단순한 형태
2. `doucment`: `DynamoDB`, `CouchDB`, 각 레코드가 하나의 문서가 됨, 문서는 데이터베이스에 따라 `XML`, `YAML`, `JSON`, `BSON` 등을 사용한다.
3. `graph-based`: `Neo4j`, `AWS Neptune`, 그래프 이론을 바탕으로 데이터베이스를 그래프로 표현한다. 관계기반문제에 유리함

### ❏ mongoDB CRUD

```javascript
// create
const users = client.db('fc21').collection('users')
    // delete, users collection은 항상 비워짐
await users.deleteMany({})

    // insert
await users.insertMany([
    {
        name: 'Foo'
    },
    {
        name: 'Bar'
    },
    {
        name: 'Baz'
    }
    ])
const cursor = users.find({})
await cursor.forEach(console.log)

// update
await users.updateOne(
    {
        name: 'Baz'
    },
    {
        $set: {
            name: 'Boo'
    }
}

// read
await users.insertMany([
    {
        name: 'Foo',
        birthYear: 2000,
    },
    {
        name: 'Bar',
        birthYear: 1995,
    },
    {
        name: 'Baz',
        birthYear: 2000,
    },
])

const cursor = users.find({ birthYear: 1995 });

// delete
await users.deleteOne({
    name: 'Baz',
})
```

### ❏ 관계형 데이터베이스(RDB)

1. 가장 고전적이고 널리 알려진 데이터베이스 모델
2. 데이터의 규격인 스키마(테이블)와 각종 제약 조건을 정하고, 그에 맞게 데이터 저장
3. 대부분의 경우 `SQL`로 상호작용한다.

```SQL
SELECT id, name FROM cities
INSERT INTO users (name, 'cityId') VALUES ('Bobo', 1)
UPDATE users SET name = 'Coco' WHERE name = 'bobo'
DELETE FROM users WHERE name = 'Coco'
```

4. `ORM(Object-relation-mapping)`: 객체와 관계형 데이터베이스의 데이터를 자동으로 매핑해주는 것(JPA, Hibernate 등)
5. `SQL injection`: 악의적인 사용자가 보안상의 취약점을 이용하여, 임의로 `SQL`문을 주입하고 실행하여 `DB`가 비정상적인 동작을 하도록 조작하는 행위

```javascript
// postgres - SQL injection
program.command('remove').action(async () =>
    {
        const client = await connect()
        const userName = await prompts({
            type: 'text',
            name: 'userName',
            message: 'Provide a user name to delete.'
 })
 // SQL injection이 가능한 지점
 const inserted = `' OR '' = '`

 // 모든 row 삭제
 const query = `DELETE FROM users WHERE name = '${inserted}'`
 console.log(query)

 // await client.query(query)
 await client.end()

 // prevent SQL injection
 await client.query(`DELETE FROM users WHERE name = $1::text`, [
 userName.userName])
```

6. `Sequelize`: 객체의 메서드를 활용하는 것처럼 쿼리 로직을 작성가능, Node.js 의 대표적인 ORM, Promise 기반으로 구현되었기 때문에 비동기 로직을 편리하게 작성할 수 있다.

### ❏ CRUD 사용자 추가하기

1. 웹의 성능을 포기해도 사용자가 편리하게 끔 만들자.
2. 데이터를 넣고 지우는것보다 전체를 새로 그려내는경우가 빠를 때가 있다.
3. `app.use(express.json())`: req.body에 값을 넣어준다. ()
4. `app.use(express.urlencoded({extended: false}))`: js 내부 모듈 중 `query-string` 모듈이 있는데 우리가 사용하기 편하게 분석해서 `req.body` 에 넣어주고. `extended: true` 를 사용하면 `qs` 모듈을 이용해서 `req.body` 에 넣어준다. (`query-string` 에 비해 보안성에서 뛰어나다?정도의 차이, 단점은 버전관리)
5. POST로 한글(유니코드)을 넘길때 몇몇 프록시에서 한글이 깨지는 경우가 있다. (대부분은 지원함)
6. 개발시 귀찮더라도 범용성있게 작성해야한다. (안되는 브라우저를 위해서)

---

## 📍 32일차 12.8.수. 온라인 강의

오늘은 `CRUD를 이용하여 게시판 만들기`,` Template Engine`, `Pug`, `PM2`을 배웠다. `node.js`의 기본언어는 `JS`인데, 한가지의 언어로 프론트와 백을 다룬다고 생각하니까 가슴이 웅장해졌다. (아직은 어색하지만..) 자주 살펴보며 눈에 익히는 것이 아무래도 좋겠지??

### ❏ 게시판 만들기

1. 웹 서비스 개발의 기본을 학습하기 좋다. 게시판을 통해 기본기를 잘 다지면 무엇이든 응용 가능
2. 게시판 목록, 보기, 수정, 작성, 삭제
3. 회원가입, 로그인, 비밀번호 찾기, pagination, 구글 로그인, 유저 작성글 모아보기

### ❏ Template Engine

1. 서버에서 클라이언트로 보낼 `HTML` 형태를 미리 템플릿으로 작성하고 동작시에 미리 작성된 템플릿에 데이터를 넣어 완성된 `HTML`을 생성한다.
2. 템플릿 엔진은 템플릿 작성 문법과 템플릿을 `HTML` 형태로 변환하는 기능을 제공한다.

![](https://images.velog.io/images/abcd8637/post/87224629-659a-4550-ac3d-4e76a6144652/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-08%2009.10.41.png)

3. `Express.js`의 템플릿엔진: `EJS`(html과 유사한 문법), `Mustache`(간단한 데이터 치환정도만 제공하는 경량화 된 템플릿 엔진), `Pug`(들여쓰기 표현식을 사용한 간략한 표기와 레이아웃 등 강력한 기능을 제공)

### ❏ Pug

1. 들여쓰기 표현식을 이용해 가독성이 좋고 개발 생산성을 높인다.
2. `HTML`을 잘 몰라도 문법적인 실수를 줄일 수 있다.
3. `layout`, `include`, `mixin` 등 강력한 기능을 제공한다.
4. `HTML` 닫기 태그 없이 들여쓰기로 블럭을 구분한다.
5. `=` 을 이용해 전달받은 변수를 사용할 수 있다.
6. `id` 나 `class` 는 태그 뒤에 이어서 바로 사용하고, `()` 를 이용해서 `attribute` 를 사용한다.
7. `each-in`: `for` 과 비슷한 태그
8. `if, else if, else` : 조건문

```pug
// index.pug
html
	head
		title= title   // title 변수 사용
	body
		h1#greeting 안녕하세요
		a.link(href="/") 홈으로

// each, if
each item in arr
	if item.name == 'new'
		h1 New Document
	else
		h1= `${item.name}`

// layout.pug
html
	head
		title= title
	body
		block content

// main.pug, 반복되는 웹사이트의 틀을 작성하고 extends하며 개발하면 매우 편리하다.
extends layout  // layout을 extends하면 block 부분에 작성한 HTML 태그가 포함됨
block content  // block을 포함한 템플릿은 layout으로 사용가능
	h1 Main Page

// include, layout은 바깥에 선언하고 가져다 쓰고, include는 조각을 만들어서 가져다 쓴다.
// 자주 반복되는 구문을 미리 작성하고 include하여 사용한다.
// 일반적인 텍스트파일도 include하여 템플릿에 포함 가능하다.

// title.pug
h1= title

// main.pug
extend layout
block content
	include titie
	div.content
		안녕하세요
	pre
		include article.txt

// mixin, 템플릿을 함수처럼 사용할 수 있다.
// include는 값을 지정할 수 없지만, mixin은 파라미터를 지정하여 값을 넘겨받아 템플릿에 사용할 수 있다.

// listItem.pug
mixin listItem(title, name)
	tr
		td title
		td name

// main.pug
include listItem
table
	body
		listItem('제목', '이름')
```

### ❏ Express.js와 pug의 연동

1. `app.set` 을 이용해 템플릿이 저장되는 디렉토리를 지정하고, 어떤 템플릿 엔진을 사용할지 지정할 수 있다.
2. `res.render` 함수는 `app.set` 에 지정된 값을 이용해 화면에 그리는 기능을 수행한다. `render` 함수의 첫 번재 인자는 템플릿의 이름, 두번째인자는 템플릿에 전달되는 값

```javascript
// app.js
app.set("views", path.join(__dirname, "views"));
app.set("view engine", "pug");

// request handler
res.render("main", {
    title: "Hello Express",
});
```

3. `app.locals` : `render` 함수에 전달되지 않은 값이나 함수를 사용할 수 있다. 템플릿에 전역으로 사용될 값을 지정하는 역할

```javascript
// app.js
app.locals.appName = "Express"

// main.pug
h1= appName
<h1>Express</h1>
```

### ❏ Express-generator 사용 시 템플릿 엔진 지정하기

1. `express-generator` 는 기본적으로 `jade` 라는 템플릿 엔진을 사용한다.
2. `jade` 는 `pug` 의 이전 이름으로, 최신 지원을 받으려면 템플릿 엔진을 `pug` 로 지정해야 한다.
3. `--view`: 템플릿 엔진을 지정할 수 있다.

```javascript
$ express --view=pug myapp
```

### ❏ 게시판 CRUD 만들기

1. 데이터를 다루는 네 가지 기본적인 기능
2. Create: 게시글 작성기능, 제목, 내용, 작성자, 작성 시간 등의 정보를 기록함, 게시글의 제목과 내용은 최소 n글자 이상이어야 함
3. Read: 게시글의 목록과 게시글의 상세를 볼 수 있어야 함. 목록은 간략화된 정보를 보여줌, 게시글 상세는 제목, 작성자, 내용, 작성 시간, 수정 시간 등의 상세한 정보를 보여줘야 한다.
4. Update: 게시글은 수정이 가능해야한다. 제목, 내용을 수정하고, 수정 시간을 기록한다. (게시글 수정은 작성자만 가능하다. + 회원기능)
5. Delete: 게시글 삭제하기, (게시글 삭제는 작성자만 가능하다. + 회원기능)
6. 모델선언하기: `ID` 는 url에 사용하기 좋은 값이 아니기 때문에 `shortId` 로 생성한다. 제목, 내용, 작성자를 `string` 타입으로 스키마에 선언한다.(작성자는 회원가입 후 실시) `timestamps`옵션으로 작성 시간, 수정 시간을 자동으로 기록해준다.

```javascript
// shortId 타입을 mongoose custom type으로 선언
// nanoid: 중복 없는 문자열 생성
// default를 이용해 모델 생성시 자동으로 아이디 생성
const { nanoid } = require("nanoid");

const shortId = {
    type: String,
    default: () => {
        return nanoid();
    },
    require: true,
    index: true,
};

module.exports = shortId;
```

### ❏ 게시글 작성 흐름

1. `/posts?write=true` 로 작성페이지 접근
2. `<form action="/posts" method="post">` 를 이용해 `post` 요청 전송
3. `[router.post](http://router.post)` 를 이용하여 `post` 요청 처리
4. `res.redirect` 를 이용하여 `post` 완료 처리

```javascript
// ./routes/posts.js
const { Router } = require('express');

const router = Router();

router.get('/', (req, res, next) => {
	if (req.query.write){
		res.render('posts/edit');  // write 값이 있으면 edit파일로 연결한다.
		return;
	}
	...
});

module.exports = router;

// ./views/posts/edit.pug
...
form(action='/posts', method="post")
	table
		tbody
			tr
				th 제목
				td: input(type='text' name='title')
			tr
				th 내용
				td: textarea(name='content')
			td
				td(colspan="2")
					input(type="submit" value="등록")

// ./routes/posts.js
const { Post } = require('./models);

router.post('/', async (req, res, next) => {
	const { title, content } = req.body;
	try{
		await Post.create({
			title,
			content,
	});
	res.redirect('/');  // 게시글 작성 후 홈 화면으로 이동하기
	} catch(err){
		next(err);
	}
}
```

### ❏ 게시글 목록 및 상세 흐름

1. `/posts` 로 목록 페이지 접근
2. `<a href='/posts/:shortId'>` 를 이용하여 상세 URL link
3. `router.get('/:shortId')` path parameter를 이용하여 요청을 처리함

```javascript
// ./routes/posts.js
// 처음 접속시 모든 리스트를 불러온다.
router.get('/', async(req, res, next) => {
	const posts = await Post.find({});
	res.render('/posts/list', { posts });  // posts/list에 { posts } 값이 넘어간다.
});

router.get('/:shortId', async(req, rse, next) => {
	const { shortId } = req.params;
	const post = await Post.findOne({ shortId });
	if(!post){
		next(new Error('Post notfound!');
		return;
	}
	res.render('posts/view', { post });  // posts/view로 값 보내기
});

// ./views/posts/list.pug
...
	table
		tbody
			each post in posts  // each로 반복문 돌기
				tr
					td
						a(href='/posts/${post.shortId}') = post.title
					td= post.author
					td= formatDate(post.createdAt)  // formatDate: custom function
		tfoot
			tr
				td(colsapn='3')
					a(href="/posts?write=true") 등록하기

// app.js
// dayjs 패키지 사용
const dayjs = require('dayjs');
app.locals.formatDate = (date) => {
	return dayjs(date).format('YYYY-MM-DD HH:mm:ss');
}

// ./views/posts/view.pug
...
	table
		tbody
			tr
				td(colspan="2")= post.title
			tr
				td= post.author
				td= formatDate(post.createdAt)
			tr
				td(colspan="2"): pre= post.content
			tr
				td: a(href='/posts/${post.shortId}?edit=true') 수정
				td button(onclick=`deletePost("${post.shortId}")`) 삭제
```

### ❏ 게시글 수정 흐름

1. `/posts/{shortId}?edit=true` 로 수정페이지 접근
2. 작성페이지를 수정페이지로도 동작하도록 작성
3. `<form action="/posts/:shortId" method="post">` 를 이용해 `post` 요청 전송
4. html form 은 `PUT method`를 지원하지 않기 때문에 `post` 사용
5. `res.redirect` 는 항상 GET요청으로 넘어간다.

```javascript
// ./routes/posts.js
router.get('/:shortId', async (req, res, next) => {
	if (req.query.edit){
		res.render('posts/edit', { post });
	}
	...
});

// 수정 요청 처리하기
router.get('/:shortId', async (req, res, next) => {
	const { shortId } = req.params;
	const { title, content } = req.body;
	const post = await Post.findOneAndUpdate({ shortId }, { title, content })  // shortId를 찾아 새로운 title, content로 바꾸겠다.
	if(!post){  // 상세 post가 없으면
		next(new Error('Post notfound');
		return;
	}
	res.redirect(`/posts/${shortId}`);  // redirect는 항상 GET요청으로 넘어간다.
});

// ./views/posts/edit.pug
...
	- var action = post ? `/posts/${post.shortId}` : "/posts"  // post가 있는 경우에는 상세 페이지로 이동, 그렇지 않은 경우는 작성하기 위한 URL로 보낸다.
	form(action=action, method="post")
		table
			tr
				th 제목
				td: input(type="text" name="title" value=post&post.title) // post가 있으면 제목을 post.title로 채우기
			tr
				th 내용
				td: textarea(name="content")= post&&post.content  // post가 있으면 내용을 post.content로 채우기
			td
				td(colspan="2")
					- var value = post ? "수정" : "등록"
					input(type="submit" value=value)
```

### ❏ 게시글 삭제 흐름

1. 게시글 상세 페이지에 삭제 버튼 추가
2. `html form` 은 DELETE 메서드를 지원하지 않음
3. `JS` 를 이용해 `fetch` 함수로 `HTTP Delete` 요청 전송
4. `router.delete` 의 응답을 `fetch` 에서 처리

```javascript
// posts/view.pug
td
	button.delete(onclick='deletePost("${post.shortId}")') 삭제

// delete.pug, promise로 실행된다.
script(type="text/javascript").
	function deletePost(shortId){
		fetch('/posts/' + shortId, { method: 'delete' })
			.then((res) => {
				if (res.ok) {
					alert('삭제가 완료되었습니다.');
					window.location.href='/posts';  // 삭제 완료 후 게시글 목록으로 이동
				}else{
					alert('오류가 발생했습니다.');
					console.log(res.statusText);
				}
			})
		.catch((err) => {
			console.log(err);
			alert('오류가 발생했습니다.');
		});
}

// 삭제 요청 처리하기
// ./routes/posts.js
router.delete('/:shortId', async (req, res, next) => {
	const { shortId } = req.params;
	try{
		await Post.delete({ shortId });  // mongoDB 내 해당 데이터 삭제
		res.send('OK');
	}catch(e){
		next(e);
	}
});
```

### ❏ Async Request Handler

1. 공식적으로 사용되는 `express` 기술은 아니고 패턴 중 하나임.
2. `async` 함수를 조금 더 쉽게 사용할 수 있고, 비동기 실행 중 오류 처리를 더 간단하게 할 수 있는 장점이 있다.
3. `request handler` 에서 오류를 처리하기 위한 방법 (`promise().catch(next)`, `async function, try - catch, next`)
4. `async` 의 비동기 처리는 매우 편리하지만, 매번 `try-catch` 구문을 작성하는 것은 귀찮고 실수하기 쉬움 따라서 `request handler` 를 `async function` 으로 작성하면서 `try-catch next` 를 자동으로 할 수 있도록 구성한 아이디어
5. `asyncHandler` 는 `requestHandler` 를 매개변수로 갖는 함수형 미들웨어, 전달된 `requestHandler` 는 `try-catch` 로 감싸져 `asyncHandler` 내에서 실행되고, `throw` 되는 에러는 자동으로 오류처리 미들웨어로 전달되도록 구성됨.
6. 오류처리를 올바르게 사용하지 않으면 `express` 앱이 종료될 수 있다.
7. `next` 인자는 제거하고 `try-catch` 구문을 제거해도 동일하게 오류 처리가 가능하다.

```javascript
const asyncHandler = (requestHandler) => {
	return async (req, res, next) => {
		try{
			await requestHandler(req, res);
		}catch(err){
			next(err);
		}
	}
}

router.get('/', asyncHandler(async (req, res) => {
	const posts = await Post.find({});
	if (posts.length < 1){
		throw new Error('Not found');
	}
	res.render('posts/lists', { posts });
});

// 실제 적용 코드(next 인자는 빼줘야한다.)
// posts.js
const { Router } = require('express');
const { Post } = require('../models');
const asyncHandler = require('../utils/async-handler');

const router = Router();

router.get('/', asyncHandler(async (req, res) => {
  if (req.query.write) {
    res.render('post/edit');
    return;
  }

  const posts = await Post.find({});

  res.render('post/list', { posts });
}));

router.get('/:shortId', asyncHandler(async (req, res) => {
  const { shortId } = req.params;
  const post = await Post.findOne({ shortId });

  if (req.query.edit) {
    res.render('post/edit', { post });
    return;
  }

  res.render('post/view', { post });
}));

router.post('/', asyncHandler(async (req, res) => {
  const { title, content } = req.body;

  if (!title || !content) {
      throw new Error('제목과 내용을 입력해 주세요');
  }

  const post = await Post.create({ title, content });
  res.redirect(`/posts/${post.shortId}`);
}));

router.post('/:shortId', asyncHandler(async (req, res) => {
  const { shortId } = req.params;
  const { title, content } = req.body;
  if (!title || !content) {
      throw new Error('제목과 내용을 입력해 주세요');
  }

  await Post.updateOne({ shortId }, { title, content });
  res.redirect(`/posts/${shortId}`);
}));

router.delete('/:shortId', asyncHandler(async (req, res) => {
  const { shortId } = req.params;
  await Post.deleteOne({ shortId });
  res.send('OK');
}));

module.exports = router;
```

### ❏ Pagination

1. 데이터가 많아지면 한 페이지의 목록에 모든 데이터를 표현하기 어려움. 따라서 데이터를 균일한 수로 나누어 페이지로 분리하는 것(ex, 10개씩 나누어 1페이지는 10~20, 2페이지는 11~20번까지 보여주기)
2. `page`: 현재 페이지, `perPage`: 페이지 당 게시글 수
3. `/posts?page=1&perPage=10` 처럼 `url query` 를 사용해 전달, `url query` 는 문자열로 넘어가기 때문에 사용시 `number` 로 형 변환을 해줘야 한다.

```javascript
router.get( => {
	const page =
			Number(req.query.page || 1)  // `page`가 없으면 default 1
	const perPage =
			Number(req.query.perPage || 10)  // `perPage`가 없으면 default 10
})
```

4. `mongoDB` 의 `limit`, `skip` 을 사용하여 구현도 가능하다. (`limit`: 검색 결과 수 제한, skip: 검색 시 포함하지 않을 데이터 수)

```javascript
// 데이터의 순서가 유지 될 수 있도록 sort를 사용한다.
// 최신순으로 정렬하고 처음부터 몇개의 게시물을 제외시키고 나머지 게시물은 몇개씩 가져오는지
router.get(... => {
	const total = await Post.countDocument({});
	const posts = await Post.find({})
		.sort({ createdAt: -1 })  // 최신순정렬
		.skip(perPage * (page - 1))
		.limit(perPage);
	const totalPage = Math.ceil(total / perPage);  // 게시글 수 / 페이지 당 게시글 수 = 총 페이지 수
})

// pug
// patination이 필요한 페이지에서 해당 템플릿을 include한 후, + pagination으로 mixin을 사용 함.
// 현재 페이지는 b 태그로 굵게 표시
mixin pagination(path)
p
  - for(let i=1; i<=totalPage; i++)
		a(href=`${path}?page=${i}&perPage=${perPage}`)
			if i == page
				b= i
			else
				= i
      = " "

include pagination
tr
	td
		+pagination("/posts")
```

### ❏ PM2 (Process Manager)

1. `Node.js` 의 작업을 관리해주는 `Process Manager`
2. `node` 명령어로 실행 시 오류 발생이나 실행 상태 관리를 할 수 없음
3. `pm2` 는 작업 관리를 위한 다양한 유용한 기능을 제공해 줌
4. 안정적인 프로세스 실행: 오류발생 시 자동 재실행
5. 빠른 개발환경: 소스 코드 변경 시 자동 재실행
6. 배포 시 편리한 관리: pm2에 모든 프로세스를 한 번에 관리
7. `pm2 init simple`, `pm2 init` 이후 `pm2 start` 명령어 실행 개발 시 `watch` 옵션 사용하여 파일 변경 시 서버 자동 재실행 구성

```javascript
// ecosystem.config.js
module.exports = {
	apps: [{
		name: 'simple-board',
		script: './bin/www',
		watch: '.',  // 모든 경로를 바라본다.
		ignore_watch: 'views',
	}],
}

$ pm2 start
```

---

## 📍 33일차 12.9.목. 실시간 강의

오늘은 `graphQL`, `인증`에 대해서 배웠다. 실습시간 마지막에는 `HTTP / HTTPS(SSL)`의 차이, `cookie-session, JWT` 방식의 차이에 대해서 알려주셨는데 너무 유익했다. `restAPI`와 `graphQL`의 차이는 내겐 스승과도 같으신 <a href='https://blog.toycrane.xyz/rest-api%EA%B0%80-%EA%B0%80%EA%B3%A0-graphql%EC%9D%B4-%EC%99%94%EB%8B%A4-a9e400b77902'>튜터님</a> 미디움을 참고하면 도움이 많이 된다.

### ❏ REST API vs gql API

1. `gql` 은 하나의 `Endpoint` 만 존재
2. `REST API` 는 `End point` 마다 데이터베이스 `SQL` 쿼리가 달라짐
3. `gql API` 는 `gql` 스키마의 타입마다 데이터베이스 `SQL` 쿼리가 달라짐

### ❏ GraphQL

1. FACEBOOK에서 2015년에 발표한 새로운 api 규격
2. `type system` 을 기본적으로 갖추고 있어서 `REST` 보다 훨씬 안정적
3. `Apollo`, `Prisma` 등 방대하고 강력한 오픈 소스 툴들로 양질의 개발자 경험 개선을 기대한다.
4. `SDL(Schema Definition Language)` : 서버에 무엇을 질의하여 값을 돌려받기를 원할 때 `SDL`로 기술(명확한 타입을 정의하여 기술)
5. `CLI` 로 `post` 요청시 쌍 따옴표를 빼도 보내진다.

### ❏ OAuth

1. 접근권한 위임을 위한 공개 표준
2. 유저 진입장벽이 매우 낮아짐(원클릭으로 로그인 가능)
3. 유저가 비밀번호를 기억할 필요가 없어짐
4. 유저 허용 여부에 따라 이메일, 프로필 사진, 닉네임 등의 기본 정보를 얻을 수 있다.

### ❏ 기타 내용들

1. 프로젝트를 할 때 `F/E` 를 나누기보다는 기능별로 담당하자(ex, `login + front + back` / `pay + front + back`)과 같이 수평적으로 제작)
2. 프론트와 백을 나눠서 개발하면 속도에서 차이가 난다. (처음은 백엔드가 느리다. DB, 보안, 인프라 등등... 나중엔 반응형때문에 프론트 개발 속도가 늦어진다. 서로 의견충돌이 난다. 즉, 전체적인 프로젝트가 늦어지기 때문에 친한친구나 숙련된 분들과 하면 기능별로 쪼개서 개발하는것을 권장한다.)
3. 템플릿 엔진: `html` 코드인데, 그 안에서 반복, 조건절로 `view` 를 만들어줄 때 사용한다.(일일이 따로 만들면 중복되는 코드가 많기 때문에 로직을 붙여서 자동으로 `html` 코드를 만들어줄 때) `EJS`, `JADE -> PUG` , `nunjunks` 사용빈도: `nunjunks` → `EJS`

```javascript
1. nunjunks: EJS의 상위호환(html을 닮음), junja2의 영향을 받음(flask에서 나온?)
2. EJS: html을 닮음
3. pug: 문법이 특이해서 따로 공부해야함
```

4. `passport` : 로그인 구현시 편리하게 도와주는 친구, 이게 없으면 `header`, `session` 관리를 직접 해줘야 한다. 써드파티 로그인도 지원한다.
5. 로그인 혹은 마이페이지를 보여주는 기능 등의 서버로부터 인증을 받아야하는 상황일 때 선택지는 크게 3가지 `cookie`, `cookie - session` , `JWT` 방식이 있다. 서버는 절대 한개로 운영하지 않고, 2개 이상으로 운영되는데 요청은 한 곳에서 들어온다. 이때 요청을 여러개의 서버 중 한곳으로 분배해주는 장치가 필요한데, 이것이 `LB(load balancer` 다. `AWS` 에서는 `ELB(elastic load balancer)` 라고 부른다.( `elastic: 탄력적인, 고무의`), `cookie-session` 는 `DB` 가 필요하고, `JWT` 는 `DB` 가 필요하지 않다.
6. `cookie` 방식은 클라이언트에 저장되는 `key - value` 로 이루어진 데이터다. 인증 유효시간을 설정할 수 있고, 유효시간이 정해진다면 클라이언트가 종료되어도 쿠키가 유지된다. 그러나, 중요정보를 쿠키에 담고있으므로 해커에게 탈취당하면 사용자의 정보를 모두 빼앗길 수 있다. 그래서 쿠키자체로는 보안과는 상관없는 개인 장바구니, 자동로그인 설정 등에 사용한다.
7. `cookie-session` 방식은 `client` 에서 요청을 보내면 `server` 에서 `cookie` 의 값을 가지고 있다가 `cookie` 와 일치하는 `session` 을 해당 서버에서 찾고 `cookie` 를 사용자에게 보내준다. 그런데, 여러개의 서버가 연결되어있다고 가정해보자. `server 1`에 현재 `cookie`를 가지고 있다가 연결이 끊겨 다시 `LB` 를 거쳐가서 2번째 `server` 로 연결이 되면, `cookie` 가 없기 때문에 지금 요청한 사용자가 인가된 사용자인지 모른다. 이럴 때는 서버에 `session` 데이터를 저장하지않고, `DB`(redis) 를 이용해 해당 `session` 데이터를 `DB` 에 저장한다. `DB` 에서 쿠키에 맞는 세션데이터를 찾고 해당하는 데이터가 있으면 리퀘스트를 돌려준다. `DB` 단이 붙었기 때문에 요청량이 많아지면 시간이 오래 걸릴 수 있다.
8. `JWT` 방식은 `cookie-session` 방식과 다르게 `DB` 단이 필요없다. `JWT` 는 일종의 신분증이라고 생각하면 편하다. `JWT` 는 `JSON web Token` 를 뜻하는데, 토큰의 특성상 위조가 상당히 어렵다. 그러나 한번 탈취되면 보안에 굉장히 취약해진다. 이를 방지하고자 만료시간이 생겼다. 이때 만료시간은 보통 5-30분 길면 1주일정도로 세팅한다. 요청이 오면 `JWT` 를 발급해준다. `mypage` 로 요청이 날라오면 요청과 함께 온 `JWT` 가 위조되었는지 확인한다. 서버에 저장되어있는 `JWT` 와 일치하면 `mypage` 요청을 같이 보내준다. `cookie-session` 방식처럼 `DB` 단에서 세션 데이터를 확인할 일이 사라진다.
9. `http` (80), `https` (443): 보안 유무, `get` 은 `URL` 에 `post` 는 `http.body` 에 요청이 넘어간다. 그래서 `http.body` 도 `postman` 같은 프로그램으로 열어볼 수 있다. 따라서 `http` 에서 `get`, `post` 의 보안은 안전하지 않다.(`id`, `pw`, `cookie` 가 평문으로 날아간다.) 특히, `cookie` 를 도청하게 되면 다른 사이트에서 재사용할 수 있따. (`cookie` 는 로그인을 성공한 사람에게 넘겨주기때문에 노출되면 위험하다.) `https` 는 이런 `id`, `pw`, `cookie` 가 암호화가 되어 서버로 날아간다. 그래서 중간에 해커가 탈취하기 힘들다. `curl` 명령어
10. `http -> https`: `DNS` 가 담당한다. `http` 로 요청이 날라오면 `DNS` 에서 다시 클라이언트로 반송처리 시키고 클라이언트에서 `DNS` 한테 `https` 로 요청하게 된다. `server` 에서 `client` 로 갈 때 `https` 로 변환한다.(항상 그런것은 아니고 대부분 캐싱이 되어있어서 중간에 다시 옴)
11. `SSL` 인증서: 이 사이트가 안전한지 확인하는 인증서(대표적으로 `AWS` certificate manager에서 발급해준다. 인증기관에 비용을 지불하면 `DNS` 에 붙여준다. 만약, `SSL` 인증서가 없으면 다시 브라우저로 리턴하거나 에러를 발생시킨다.)
12. `node template engine` 은 서버에서 파일을 보내줘서 브라우저단에서 띄우기만 한다. 이런 방식은 `SSR`, 반대로 `CSR` 은 리액트에서 파일을 만들고 데이터만 서버에 요청해서 둘다 합치면 `CSR` 이 된다.
13. `SSR` 은 검색엔진이 데이터를 모두 읽을 수 있다. `CSR` 은 파일을 한번 거쳐서 탐색해야하기 때문에 바로 노출이 되진 않는다(feat. CORS)
14. 리액트는 노드서버에 직접 요청해서 받아오는것은 아니다. 그냥 브라우저로 데이터를 보내주고 데이터는 브라우저에서 서버로 요청하여 브라우저에서 취합한다.
15. 로그인처럼 `DB` 사용하는건 `node.js` 사용하고, 보여주기만 할거면 `CSR`
16. 실 서비스할때는 내부 웹서버보다 `nginx`를 직접 붙이는 편이 더 좋다. `node.js` 는 내부 웹서버도 배포하기 충분하다.
17. `AWS - route 53` 에서 `DNS` 에 `SSL` 을 직접 붙인다. `ELB` 에도 `SSL` 을 붙여야한다. 이후 뒷단에 있는 `EC2` 서버로 넘어간다.
18. `ELB` 를 쓰는 이유는 `autoScaling` 을 쓰기 위함이다.
19. 인스턴스를 늘릴 때는 사용률이 51%를 넘어섰을 때 이때 서버가 터져버리면 다음서버는 `@ + 51%` 가 되는데 다음 서버가 50이면 서버가 터져버린다.

---

## 📍 34일차 12.10.금. 온라인 강의

오늘은 `회원가입`, `passport.js`, `session-store`, `댓글 기능`을 배웠다.

### ❏ 회원가입

1. 이메일, 이름, 패스워드의 간단한 정보만 사용(이메일 형식이 올바른지 확인, 비밀번호 최소 길이 설정, 패스워드와 패스워드 확인 문자가 일치하는지 확인)
2. 회원의 비밀번호를 `DB`에 그대로 저장하면, 관리자가 모든 회원의 비밀번호를 알 수 있고, `DB`가 해킹되면 보안 취약점이 발견하게 되므로 `hash`값으로 비밀번호를 저장한다.(`hash`는 문자열을 되돌릴 수 없는 방식), 비밀번호의 `hash`값을 `DB`에 저장하고, 로그인 시 전달된 비밀번호를 `hash`하여 저장된 값과 비교해 로그인을 처리한다.
3. `node.js`의 기본제공 모듈인 `crypto` 모듈을 사용하여 `hash` 값을 얻을 수 있다. 간단하게 `sha1` 알고리즘을 사용하거나, 보다 강력한 `sha224`, `sha256` 등의 알고리즘도 사용할 수 있다.

```javascript
const hash = crypto.createHash("sha1");
hash.update(password);
hash.digest("hex");
```

4. 회원가입 페이지 구현 -> `script`를 이용해 이메일 형식, 비밀번호 확인 문자 -> `form`을 이용해 `post` 요청 전송 -> 회원가입 처리 및 `redirect`

```javascript
// 비밀번호 hash 값 저장
// 이미 존재하는 회원인지 체크
// 가입 후 메인화면으로 redirect

router.post(... => {
	const { email, name, password } = req.body;
	const pwHash = getHash(password);
	const exists = await User.findOne({ email })

	if (exists){
		throw new Error("이미 가입된 메일입니다.");  // try - catch 문이 아니므로 async request handler를 사용한다.
	}

	await User.create({
		email,
		name,
		password: pwHash,
	})

	res.redirect('/');  // 메인화면으로 보내기
})
```

### ❏ passport란?

1. `express.js` 어플리에키션에 간단하게 사용자 인증 기능을 구현하게 도와주는 패키지, 유지 세션 관리 및 다양한 로그인 방식 추가 기능 제공
2. `passport-local`: 다양한 로그인 방식을 구현하기 위해 `strategy`라는 인터페이스를 제공한다. `strategy`는 인터페이스에 맞게 설계된 다양한 구현체(facebook, google, ...)들이 있다. `passport-local` 은 `username`, `password`를 사용하는 로그인 구현체를 의미한다.

```javascript
1. 로그인 화면 구성
2. passport-local strategy로 로그인 구현하기
3. passport.js 설정하기
4. passport로 요청 처리하기

// passport-local stratgy
// config 정보 전달 -> authenticate 실행(config를 인자로 전달받음 이메일, 패스워드, 완료처리 콜백함수(done)) -> 데이터 찾기

const config = {
	usernameField: 'email',
	passwordField: 'password',
}

const local = new LocalStrategy(config, )

..., async(email, password, done) => {
	try{
		const user = await User.findOne({ email });
		if(!user){
			throw new Error("회원을 찾을 수 없읍니다.");
		}

		if(user.password !== getHash(password)){
			throw new Error("비밀번호가 일치하지 않읍니다.");
		}

	// 세션에 저장되는 유저 정보의 최소화
    // 첫 번째 인자: error, 두번째인자: data
		done (null, {
			shortId: user.shortId,
			email: user.email,
			name: user.name
		});
	}catch(e){
		done(e, null)
	}
}

// passport.js
// 작성한 strategy를 passport.user를 이용해 사용하도록 선언해야 함
// passport.use를 이용해 strategy를 사용하도록 선언한 후 passport.authenticate를 사용해 해당 strategy를 이용해 요청을 처리할 수 있음
const local = require('./strategies/local');
passport.use(local);

// routes/auth.js
router.post('/',
	passport.authenticate('local');
...

// app.js
// passport.authenticate 함수를 http 라우팅에 연결하면 passport가 자동으로 해당하는 strategy를 사용하는 request handler를 자동 생성
// express-session과 passport.session()을 사용하면 passport가 로그인 시 유저 정보를 세션에 저장하고 가져오는 동작을 자동으로 수행해 줌
const session = require('express-session');
app.use(session({
	secret: 'secret',
	resave: false,
	saveUninitialized: true,
}));

app.use(passport.initialize());
app.use(passport.session());
app.use('/auth', authRouter);

// session 유저 활용하기
// session을 이용해 user를 사용할 때는 serializeUser와 deserializeUser를 설정한다.
// 이는 세션에 user정보를 변환하여 저장하고 가져오는 기능을 제공한다.(회원 id만 세션에 저장하고 사용 시 회원정보를 디비에서 찾아서 사용)
// 세션 사용 시 위 두 함수를 작성하지 않으면 passport 로그인이 동작하지 않음
passport.serializeUser((user, callback) => {
	callback(null, user)
})

passport.deserializeUser((obj, callback) => {
	callback(null, obj)
})

// logout
// passport는 req.logout 함수를 통해 세션의 로그인 정보를 삭제하여, 로그아웃 기능을 구현할 수 있다.
router.get('/logout', ... {
	req.logout();
	res.redirect('/');
})

// login 확인 미들웨어
// 로그인을 필수로 설정하고 싶은 경우, 미들웨어를 사용하여 체크할 수 있음
function loginRequired(req, res, next){
	if(!req.user){
		res.redirect('/');
		return;
	}
	next();
}

app.use('/posts', loginRequired, postsRouter)  // 로그인이 확인되면 postsRouter로 넘어간다.
```

### ❏ Session

1. 웹 서버가 클라이언트의 정보를 클라이언트별로 구분하여 서버에 저장하고, 클라이언트 요청시 `session ID`를 사용하여 클라이언트의 정보를 다시 확인하는 기술(클라이언트가 정보를 저장하고 요청시 정보를 보낸 `Cookie`와 대조 됨)
2. 서버는 세션을 생성하여 세션의 구분자인 `session ID`를 클라이언트에 전달함. 클라이언트 요청시 `session ID`를 함께 담아서 전송, 서버는 전달받은 `session ID`로 해당하는 세션을 찾아 클라이언트 정보를 확인함
3. `express-session` 패키지를 사용하여 간단하게 `session` 동작을 구현할 수 있다. 특별한 설정 없이 자동으로 `session`동작을 구현해줌, ㅈ동으로 `session ID`를 클라이언트에게 전달, `session ID`로 클라이언트 정보 확인

### ❏ Session Store를 사용하는 이유

1. `express-session` 패키지는 `session` 을 기본적으로 메모리에 저장함. 따라서 현재 구현된 어플리케이션을 종료 후 다시 실행하면 모든 유저의 로그인 해제됨, 혹은 서버가 여러 대 있을 경우, 서버 간 세션정보를 공유할 수 없음

### ❏ MongoDB - Session Store

1. `connect-mongo` 패키지를 이용해 `MongoDB` 를 `session store` 로 사용할 수 있다.
2. `connect-mongo` 패키지는 `express-session` 패키지의 옵션으로 전달 가능하다. 자동으로 `session` 값이 변경될 때 `update` 되고 `session` 이 호출될 때 `find` 함
3. 재부팅되어도 `data` 가 삭제되지 않기 때문에 `session-data` 를 유지 할 수 있다.
4. 세션데이터를 몽고디비에 저장하고 관리하는 기능을 자동으로 수행해 줌

```javascript
// connect-mongo 패키지를 이용해 express-session 설정시 store 옵션에 전달 및 mongoUrl 설정
const mongoStore = require('connect-mongo');

app.use(session({
	secret: 'secret',
	resave: false,
	saveUninitialized: true,
	store: mongoStore.create({
		mongoUrl: 'mongoUrl',
	}),
});
```

### ❏ 회원과 게시글의 연동

1. 게시글 작성시 로그인된 회원 정보를 작성자로 추가

```javascript
// PostSchema에 author 추가
// populate를 사용하기 위해 ObjectID 사용
// ref를 유저 모델의 이름은 'User'로 선언
author: {
	type: Schema.Types.ObjectId,
	ref: 'User',
	required: true,
}

// 게시글에 작성자 추가
// req.user에는 straegy에는 최소한의 정보인 shortId, email, username만 가지고 있다.
// Post 생성 시 user의 ObjectID를 전달해야하는데, User에서 shortId로 회원을 검색하여 한 번 더 검증
// 객체가 주어지면 자동으로 ObjectID 사용
const author = await User.find({
	shortId: req.user.shortId,
})

if(!author){
	throw new Error('No User')
}

await Post.create({
	title,
	content,
	author,  // author만 들어가있는게 아니고 user객체 data전체가 들어가는데, mongoDB가 여기서 _id만 꺼내서 저장해준다.
})
```

2. 게시글 - 작성자는 populate 하여 사용하도록 구현

```javascript
// populate
// 자동으로 user collection에서 author를 찾아서 넣어준다.
const posts = await Post.find({}).populate("author");

res.render("posts/list", { posts }); // posts를 반복문으로 꺼내 쓸 수 있다.
```

3. 게시글 수정, 삭제 시 로그인된 유저와 작성자가 일치하는지 확인

```javascript
// 수정, 삭제 시 유저 확인
const post = await Post.find({ shortId }).populate("author");

if (post.author.shortId !== req.user.shortId) {
    throw new Error("Not Authorized");
}
```

4. 작성자의 게시글 모아 보기 기능 구현: 기본적으로 `MongoDB` 는 `Document` 검색 시 전체 문서를 하나씩 확인하기 때문에 매우 비효율적인 검색을 수행한다. 데이터가 많아질 경우 속도 저하의 큰 원인이 된다. 검색을 위해 `Document` 를 정렬하는 기능을 제공함. index 를 설정하면 주어진 쿼리를 효율적으로 수행하여 성능을 향상시킬 수 있다.

```javascript
// index: true 옵션을 사용하면 mongoose가 자동으로 MongoDB에 인덱스를 생성해줌
// 이미 데이터가 많을 때 index 추가시 작업시간이 길어져 MongoDB가 응답하지 않을 수 있다. 예상되는 인덱스를 미리 추가하는 것이 좋음(처음부터 설정))
author: {
	type: Schema.Types.ObjectId,
	ref: 'User',
	required: true,
	index: true,
}
```

5. 회원 게시글 라우팅 추가하기: RESTful 한 구성을 위해 /users/{userId}/posts 로 구성, 게시글 목록 view 는 기존에 작성한 posts/list.pug 를 재활용

```javascript
// /routes/users.js
router.get('/:shortId/posts', ... => {
	const { shortId } = req.params;
	const user = await User.find({ shortId });
	const posts = await Post
			.find({ author: user })
			.populate('author');
	res.render('posts/list', { posts, user });
})

h2= user ? `${user.name}의 게시글` : `전체 게시글`
td: a(href=`/users/${post.author.shortId}/posts`)
	= post.author.name
```

### ❏ CSR로 댓글 기능 구현하기

1. 페이지 로드 시 필요한 리소스를 클라이언트에 선언(HTML Template, 브라우저에 표시되지 않는 HTML element를 작성해두고 JS로 이를 화면에 반복적으로 그릴 수 있게 하는 기술)
2. 클라이언트에서 필요한 데이터를 비동기 호출
3. 클라이언트가 전달받은 데이터를 가공, 리소스를 사용하여 화면에 표시
4. `HTML template` 사용하여 한 개의 댓글이 표시될 모양을 선언(JS로 조작하기 위해 `id`, `class` 를 선언하는 것이 유용하다)
5. `CSR` 을 구현하기 위해서는 `HTML` 이 아닌 데이터만 주고받을 수 있는 `API` 를 구성해야한다.(JSON 사용), 댓글 작성 시 댓글목록을 다시 불러와 그리는 형식으로 구현
6. `sub-schema` 를 이용하여 `Post` 스키마에 `Comment` 를 배열로 추가

```javascript
const CommentSchema = new Schema({
	content: String,
	author: {
		type: Schema.Types.ObjectId,
		ref: "User",
	},
}, {
	timestamps: true
});

const PostShema = new Schma({
	...
	comments: [CommentSchema],
  ...
})
```

7. 댓글 작성: `api/posts/{postId}/comments` 경로로 댓글 작성 기능 구현, 게시글 업데이트시 `${push}` 를 사용하여 `comments` 배열에 새로 작성된 댓글 추가(동시에 들어오는 요청을 정확하게 처리), `api` 는 `render` 대신 `json` 으로 응답

```javascript
// 댓글 업데이트
await Post.updateOne(
    { shortId },
    {
        $push: {
            comments: {
                content,
                author,
            },
        },
    }
);

res.json({ result: "success" });

// 댓글 목록
// find에 populate하지 않고, User (model)의 populate를 사용하는 방법도 가능
await User.populate(posts.comments, {
    path: "author",
});
```

8. 비동기 HTTP 요청은 `fetch` 함수를 이용함.

```js
// 댓글 작성하기
// 호출 결과의 성공 여부를 확인하여, 댓글 다시 불러오기 실행
fetch('url', {
	method: "post",
	headers: { ~ },
	body: JSON.stringify({ content }),
})
```

### ❏ MongoDB Aggregation

1. MongoDB에서 Document들을 가공, 연산하는 기능
2. RDMBS에서 SQL로 수행할 수 있는 기능들을 유사하게 구현할 수 있음 (SQL의 GROUP BY, DISTINCT, COUNT, JOIN 등)
3. mongoDB의 find는 검색 필터링과 정렬 이외의 기능을 제공하지 않음, 다른 collection에서 데이터를 가져오거나, 그룹화할때는 Aggregation을 통해 이를 수행할 수 있음

---

## 📍 35일차 12.11.토. 온라인 강의

오늘은 `JWT` 그리고 회원 비밀번호 찾기, `SMTP`를 이용하여 메일 발송기능, 비밀번호 초기화, `OAuth`, 웹 서버 소프트웨어인 `Nginx`에 대해서 배웠다. 나중에 로그인 관련 기능을 구현할 때 써먹으면 도움이 되는 내용이라서 까먹지 않고 기억해야겠다.

### ❏ JWT(Json Web Token)

1. 인증을 위한 정보를 특별한 저장소를 이용하지 않고, 전자 서명을 이용하여 확인하는 방법
2. `header`(토큰의 타입(jwt), 데이터 서명방식), `payload`(전달되는 데이터), `signature` (헤더와 페이로드의 전자서명)로 구성되어 있다.
3. `JWT` 는 `Web Token`, 데이터를 웹에서 사용하기 위한 스펙이므로 웹에서 문제없이 사용할 수 있는 문자열로만 구성된 `base64` 인코딩을 사용한다.
4. `JWT` 의 `payload` 는 단순히 정보를 `base64 encode` → `decode` 시 정보가 노출된다 → 민감한 정보는 제외하고 토큰을 생성한다.
5. 서버는 `JWT` 를 생성할 때, 비공개키를 이용하여 서명을 함. `payload` 를 조작할 경우 서명(signature)이 일치하지 않기 때문에 인증 실패
6. 사용자 로그인 → 서버는 로그인된 유저 정보를 JWT 로 생성하여 클라이언트에 전달 → 클라이언트는 전달받는 JWT 를 이용하여 인증이 필요한 요청에 사용

![](https://images.velog.io/images/abcd8637/post/080642e9-3012-4b15-8761-b2bc72473699/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-11%2009.31.32.png)

### ❏ JWT 사용 이유

1. `session` 은 기본적으로 웹 브라우저를 위한 통신 스펙
2. 모바일 앱 등, 웹 브라우저가 아닌 어플리케이션의 경우 `session` 을 활용하기 부적합함, `JWT` 를 사용하면 어느 클라이언트에서나 동일한 방식의 사용자 인증을 구현 가능

### ❏ JWT + Cookie

1. `cookie`: 웹 서비스에서 사용하는 정보를 클라이언트(브라우저)에 저장하고, `HTTP` 요청시 이를 함께 전송하여 클라이언트 정보를 서버에 전달하는 기술
2. `session`: 클라이언트 정보를 서버 측 저장소에 저장하고 사용(`session id` 로 `session store` 에서 확인해서 클라이언트 정보를 확인함),
3. `session` 을 사용한 유저 로그인: `cookie에 session ID` 저장 → `session store` 에서 유저 정보 가져오기
4. `JWT` 를 쿠키처럼 사용하는 경우: `JWT` 로 요청 → 서명 확인 후 유저 정보 사용(DB 접근이 한단계 줄어서 효율적인 인증 구현 가능)
5. 로그인 로직에서 `JWT` 생성 후 쿠키로 전달 → `passport-jwt` 패키지로 `JWT 로그인 미들웨어` 작성 및 사용

```js
// token 생성 및 미들웨어 선언하기
setUserToken = (res, user) => {
	const token = jwt.sign(user, secret);
	res.cookie('token', token);  // res.cookie 함수를 사용하여 token을 클라이언트 쿠키로 전달
}

---
router.post('/', passport.authenticate('local'),
	(req, res, next) => {
		setUserToken(res, req.user);  // 쿠키를 브라우저에 저장함

	res.redirect('/');
});

// passport-jwt 사용하기
// 요청된 JWT토큰의 서명을 확인하고 인증하는 기능을 구현
const JwtStrategy = require('passport-jwt').Strategy;

const cookieExtractor = (req) => {
	const { token } = req.cookies;

	return token;
};

const opts = {
	secretOrKey: secret,  // import
	jwtFromRequest: cookieExtractor,
}

module.exports = new JwtStrategy(opts, (user, done) => {
	done(null, user)
})

---
passport.use(jwt);
```

6. `JWT` 토큰은 기본적으로 모든 요청에 포함한다. 요청에 토큰이 있는 경우 로그인된 상태로 처리하기 위해 모든 요청에 공통적으로 적용할 수 있는 미들웨어로 `JWT` 로그인을 추가
7. 로그아웃은 간단하게 클라이언트 쿼리를 삭제하여 처리 가능, `token` 값을 `null` 로 전달하고 `cookie` 의 만료시간을 0으로 설정하여 클라이언트가 쿠키를 바로 만료시키도록 전달

```js
// jwt middleware
app.use((req, res, next) => {
    if (!req.cookies.token) {
        next();
        return;
    }

    return passport.authenticate("jwt")(req, res, next); // req.user에 저장
});

// jwt logout
res.cookie("token", null, {
    maxAge: 0, // 쿠키 만료 시키기
});
```

### ❏ 회원 비밀번호 찾기 구현

1. 임의의 문자열로 비밀번호 초기화
2. 초기화된 문자열을 메일로 전달 → 메일 발송기능 개발 필요
3. 초기화 후 첫 로그인 시 비밀번호 변경 요청

### ❏ 메일 발송기능 구현 방법

1. `SMTP` 서버 이용: 네이버 구글 등의 메일서버를 이용하여 무료로 발송 가능, 메일 발송 및 관리 기능 직접 개발 필요
2. 메일 발송 서비스 이용(Mailgun, Sendgrid): 메일 발송 api 제공 및 관리용 웹페이지 제공, 사용량에 따라 유료 과금

### 💡 SMTP란?

1. `Simple Mail Transfer Protocol`: 메일 전송을 위한 표준 규약, `SMTP` 서버란 표준 규약을 통해 메일 전송하는 기능을 구현한 서버
2. `Node.js` 에서 메일 발송하기: `Nodemailer` 패키지를 사용하여 `SMTP` 서버(gmail, naver...)를 통해 메일 발송하기, 직접 만드는 것은 비효율적이다.
3. `Nodemailer` 에서 `gmail` 을 사용하기 위해서는 앱 비밀번호 설정 필요, 한번 설정하면 재 확인 불가

```js
const nodemailer = require("nodemailer");

const transport = nodemailer.createTransport({
    service: "Gmail",
    auth: {
        user: "google account",
        pass: "app password",
    },
});

const message = {
    from: "login account",
    to: "mail address",
    subject: "title",
    text: "message",
};

transport.sendMail(message, (err, info) => {
    if (err) {
        console.error("err", err);
        return;
    }
    cosnole.log("ok", info);
});
```

### ❏ 비밀번호 초기화 기능

```js
// 임의의 문자열을 만들어주는 함수
function generateRandomPassword(){
	return Math.floor(
		Math.random() * (10 ** 8)
		).toString().padStart('0', 8);
}
---

// email을 받아서 generateRandomPassword로 사용자의 비밀번호 초기화 후 메일로 발송
router.post('/reset-password', asyncHandler(... => {
	const { email } = req.body;
	const randomPassword = generateRandomPassword();
	await User.findOneAndUpdate({ email }, {
		password: getHash(password),
	});

	await sendEmail(email, '...', password);
	res.redirect('/');
}));
```

### ❏ 비밀번호 초기화 후 로그인 시 비밀번호 변경 요청

```js
// 비밀번호 변경
const UserSchema = ...
	passwordReset:{
		type: Boolean,
		default: false,
	}
...

---

router.poast('/reset-password', ...
	await User.findOneAndUpdate({
	...
	passwordReset: true
})

// 비밀번호 변경 요청
function checkPasswordReset(req, res, next){
	if(req.user && req.user.passwordReset){
		res.redirect('/update-password');
		return;
	}

	next();
}

router.poast('/update-password', ...
	await User.findOneAndUpdate({
	...
	passwordReset: false
})
```

### ❏ OAuth의 이해

1. `open authorization`: 서비스 제공자가 다른 서비스에게 데이터를 제공하기 위해 서비스 사용자에게 제공하는 사용자 인증방식의 표준
2. 서비스 제공자에게 인증 요청 → 인증 완료 후 사용자 정보를 요청한 서비스로 전달 → 인증 정보를 이용해 서비스 제공자의 데이터 사용
3. 구글 `OAuth` 인증 요청 → 인증된 `OAuth Token` 을 기록 → `OAuth Token` 을 사용하여 구글 캘린더 `API` 사용
4. 웹 서비스 제공자는 ID, PW 로그인을 구현할 필요가 없음
5. 웹 서비스 사용자는 ID, PW 를 입력할 필요가 없음

### ❏ 구글 로그인 구현하기

1. 구글 클라우드 플랫폼 프로젝트 생성
2. API 및 서비스 → OAuth 동의화면 설정
3. 사용자 인증정보 → OAuth 클라이언트 ID 만들기
4. passport-google-oauth20 연동
5. `passport-google-oauth20` : passport-strategy 인터페이스의 구글 로그인 집합체(OAuth 인증을 구현하기 위해서는 인증 요청, 데이터 수신 등의 복잡한 작업 필요), `passport-google-oauth2.0` 은 손쉽게 구글 `OAuth 2.0` 을 구현해주는 패키지

### ❏ Nginx

1. 최근 신규 프로젝트에서 가장 많이 채택되고 있는 웹 서버 소프트웨어(웹 서버 소프트웨어: `HTTP` 요청을 받아 파일이나 프로그램 실행 결과를 `HTTP` 응답으로 보내주는 소프트웨어)
2. `Java - Tomcat`, `PHP - fastcgi` 등 다른 언어가 `HTTP` 요청을 처리를 위한 의존성이 있는 것에 반해, `Node.js` 는 기본적으로 `HTTP` 요청을 수신하고, 응답하는 기능이 이미 있다. 따라서 웹 서버 소프트웨어 없이도 스스로 동작할 수 있다. 하지만, `node.js` 단독으로 사용하게 되면 `HTTPS`, `도메인 연결`, `static file caching` 등의 기능을 `production-level` 서비스를 구축할 수는 없다. 따라서 `node.js` 앞 단에 웹 서버 소프트웨어를 붙여서 사용한다. `HTTP` 요청과 응답은 node.js에서 자체적으로 사용이 가능하다.
3. `Nginx` 의 `reverse-proxy` 기능을 사용해, `Node.js` 와 `Nginix` 를 연결할 수 있다. `reverse-proxy` 는 `HTTP` 요청을 다른 서버에 전달하는 기능인데, `Nginx` 가 요청을 받아, 설정된 내용에 해당하는 요청만 `node.js` 에 전달한다.

![](https://images.velog.io/images/abcd8637/post/9d61eb15-28cf-47e0-9c8e-5b6cdb9ea673/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-11%2016.38.13.png)

```js
// 외부에서 온 모든 요청을 localhost:3000으로 전달하는 설정 파일
// HTTPS, file caching들의 작업은 Nginx의 설정방법을 참고하기
server {
	listen 80;
	server_name www.example.com;

	location / {
		proxy_pass http://localhost:3000;
		proxy_http_version 1.1;
	}
}
```