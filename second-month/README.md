## π 21μΌμ°¨ 11.23.ν.(μ€μκ° κ°μ) (ν΄λ¦°μ½λμ νμμ€ν¬λ¦½νΈ)

μ΄λ²μ£Όλ `ν΄λ¦°μ½λ`μ `typescript`μ `νμ`, `ν΄λμ€`, `μΈν°νμ΄μ€`, `Generic`, `Decorator`μ λν΄μ λ°°μ λ€. μλ¦¬μ€ μμ§λμ΄ SWνΈλμ μ μ²­ν  λΉμ μ μΌ κΈ°λκ° λμλ μ»€λ¦¬νλΌμ΄ μ΄λ²μ£Όμ°¨μ λ°°μ°λ λ΄μ©μ΄μλλ°, λ²μ¨ κ·Έ λ΄μ©μ λ£κ² λλ€λ.. μ΄μ λ³΄λ€ λμ± μ΄μ¬ν λ€μ΄μΌκ² λ€. μ¬λλμ λ§μ°¬κ°μ§λ‘ μ΄λ‘ μμκ³Ό μ€μ΅μμμΌλ‘ λλμλλ°, μ€μ΅μμμ κΉλ³μ²  μ½μΉλμ΄ κ°λ₯΄μ³μ£Όμ¨λ€. μ²μμλ λκ΅°μ§ μ λͺ°λλλ° μκ³ λ¦¬μ¦κ³μμ κ½€ μ λͺν λΆμ΄μ¨λ€. κ°λ°μ μ€νμ±νλ°©μ μ½λ©νμ€νΈ λλΉ μμμ λν΄ λ¬Όμ΄λ³΄λ©΄ ν­μ <a href='https://github.com/tony9402/baekjoon'>tony9402 - μ½λ©νμ€νΈ λλΉ λ¬Έμ μ§</a>λΆν° νλΌλ μκΈ°κ° λ§μλλ° κ·Έ λ ν¬μ§ν°λ¦¬ μ»¨νΈλ¦¬λ·°ν°μ 2λ²μ§Έ(<a href='https://github.com/VSFe'>VSfe</a>)λΆμ΄μ¨λ€. π²π² μ λ² μ΄κ³ μλμ΄ κ°λ₯΄μ³μ£Όμ€λλ μ κΈ°νλλ° μ΄λ²μλ μμ²­ μ κΈ°νλ€.. κ³΅λΆ μμ§κ° νκ» μμμ€λ₯΄λ κ³κΈ°κ° λμλ€.

### β ν΄λ¦°μ½λλ

1. λΉμ¦λμ€ μ λ¬Έκ° β λΆμκ°(μ νκ΄λ¦¬μ / μλΉμ€ κΈ°νμ / νλ‘κ·Έλλ¨Έ) β νλ‘κ·Έλλ¨Έ β μ»΄ν¨ν°
2. μ’μΈ‘ λ°©ν₯μ λͺ©μ  / μΆμμ , μ°μΈ‘ λ°©ν₯μ μλ¨ / κ΅¬μ²΄μ 
3. μκ°μ΄ κ°μλ‘ μ½λλ₯Ό μ°λκ²λ³΄λ€ μ½λ λΉμ€μ΄ λμ΄λλ€.(μ½λ κ°λμ±μ μ€μμ±μ΄ λμ΄λ¨)
4. μ½λ μ¬μ¬μ©(λ°λ³΅λλ λ¬Έμ μ νμ΄λ μ¬μ¬μ© κ°λ₯, SW κ°λ° λΉμ© μ κ°)

### π‘ νμ€νΈ κΈ°λ²

1. μλ νμ€νΈ

-   νμ§ λ΄λΉμκ° UIλ₯Ό μ¬μ©ν΄ κΈ°λ₯ κ²μ¦
-   μ¬λμ μμΌλ‘ μΌμΌμ΄ νμ€νΈνλ€.(μΈκ±΄λΉ μ¦κ°)
-   μννΈμ¨μ΄ νκ·(μκ°μ λ°λΌ κΈ°λ₯μ΄ λ§μμ§λ©΄, μΆκ°ν κΈ°λ₯κ³Ό κΈ°μ‘΄μ κΈ°λ₯κ³Όμ μΆ©λλ‘ μΈν΄ κΈ°μ‘΄μ μλ μ½λμ‘°μ°¨ μ€νμ΄ μλλ νμμ΄ λ°μνλ€.)

2. μΈμ νμ€νΈ

-   λ°°μΉλ μμ€νμ λμμΌλ‘ κ²μ¦
-   μ μ²΄ μμ€ν μ΄μ μ¬λΆ μ λ’°λκ° λμ
-   λμ λΉμ©(μμ± / κ΄λ¦¬ / μ€ν λΉμ©)
-   νΌλλ°± νμ§μ΄ λ?μ(νμμ λλ¬λμ§λ§ μμΈμ μ¨κ²¨μ§)
-   νμ€ν°κ° νμ§ μΈλΆλ₯Ό μ΄ν΄λ³Έλ€.

3. μλ νμ€νΈ

-   κΈ°λ₯μ κ²μ¦νλ μ½λλ₯Ό μμ±
-   νμ€νΈ μ½λ μμ± λΉμ©μ΄ μλΉλμ§λ§ μ€ν λΉμ©μ΄ λ?κ³  κ²°κ³Όμ μ λ’°λκ° λμ
-   νμ€νΈ μ½λ μμ±κ³Ό κ΄λ¦¬κ° νλ‘κ·Έλλ¨Έ μ­λμ ν¬κ² μν₯μ λ°λλ€.

4. λ¨μ νμ€νΈ

-   μμ€ν μΌλΆ(νμ μμ€ν)λ₯Ό λμμΌλ‘ κ²μ¦
-   λ?μ λΉμ©
-   λμ νΌλλ°± νμ§
-   μ μ²΄ μμ€ν μ΄μ μ¬λΆ μ λ’°λκ° λ?μ
-   λ¨μλΌλ¦¬ μ€λ₯κ° λλ κ²½μ°κ° μλ€.
-   νμ€ν°κ° νλ‘κ·Έλ¨μ κΈ°λ₯μ μ΄ν΄λ³Έλ€.

### β νμμ€ν¬λ¦½νΈμ μ­μ¬

1. ES2015λΆν° λͺ¨λ μ€νμ μ κ³΅νκΈ° μμ: νλ‘μ νΈμ κ·λͺ¨ μ¦κ°, κ°λ°νκ²½μ΄ λ³΅μ‘ν΄μ§, `npm` μ λ±μ₯, λ²λ€λ¬ λ±μ₯(Webpack λ±λ±) μ£Όμμ κ±° / νμΌμμΆ / μ΄κΈλ¦¬νμ΄, νΈλμ€νμΌλ¬ λ±μ₯ (Babel, Typescript λ±λ±)
2. `TS` λ `JS` μ λͺ¨λ  κΈ°λ₯μ κΈ°λ³ΈμΌλ‘ μ κ³΅νλ€. (μνΌμ), λͺμμ μΈ λ°μ΄ν°μ λν μ ν μ€λͺ
3. μλ°μ€ν¬λ¦½νΈλ³΄λ€ νμμ λν μΆκ°μ μΈ μ λ³΄λ₯Ό μ»μ μ μλ€.
4. μμ μ± μλ μ½λλ₯Ό μμ±νκΈ° μνμ¬ λ³λμ νμμ²΄ν¬κ° νμν¨
5. μμμΉ λͺ»ν μ€λ₯κ° λ°μν  μ μμ
6. νμ μ²΄ν¬λ₯Ό μν΄ μ½λκ° κΈΈμ΄μ§λ λ¬Έμ  λ°μ
7. μ€μ  μ½λλ₯Ό μ€νμ ν΄λ³΄κΈ° μ κΉμ§ μ€λ₯ μ²΄ν¬ λΆκ°
8. μ€μ  μλΉμ€ λ¨κ³κ° μλ μ»΄νμΌλ¬ κ³Όμ μμ μ€λ₯λ₯Ό νμΈν  μ μλ€.(λλ²κΉ, μλ‘κ³ μΉ¨ κ³Όμ κΉμ§ κ°μ§ μμλ νμΈ κ°λ₯ν¨) λ³΄λ€ μμ ν νλ‘κ·Έλλ° νκ²½μ μ κ³΅λ°μ μ μλ€.

```
JS
 - μΈν°νλ¦¬ν° μΈμ΄(νμ€ νμ€ μ€ν)
 - μ€ν¬λ¦½ν μΈμ΄
 - μ»΄νμΌλ¬ νμ μμ
 - κ°μ²΄ μ§ν₯μ μ΄μ§ μμ, νλ‘ν νμ κΈ°λ°

TS
 - μ»΄νμΌ μΈμ΄
 - κ°μ²΄ μ§ν₯ νλ‘κ·Έλλ° μΈμ΄
 - μ»΄νμΌλ¬ νμ
 - ν΄λμ€ κΈ°λ°, μμ, μΈν°νμ΄μ€, μμ μ μ¬μ© κ°λ₯
```

### β typescriptμ typeμμλ³΄κΈ°

1. μΈν°νμ΄μ€μ κ²½μ°, μ»΄νμΌνλ κ³Όμ μμ μΈν°νμ΄μ€λΌλ¦¬ μ λΆ ν©μ³μ§κ³  ν΄λΉ μΈν°νμ΄μ€μ λμνλ κ°μ²΄λ₯Ό μμ±ν΄μ£Όλ κ³Όμ μ κ±°μΉ©λλ€. (JSμ νΈμ΄μ€νμ λ μ¬λ¦΄ μ μμ§λ§, μ€μ  λμκ³Όμ μ μ½κ° λ€λ¦λλ€. μΌλ°μ μΌλ‘ μΈν°νμ΄μ€, ν΄λμ€ λ±μ μ μλ μ΅μλ¨μ κ³ μ νκ³  νλ¨μ μΆκ°νκ±°λ μμ νλ κ²μ μ§μνλ νΈ μλλ€.)

```typescript
// νμ μ νΈλ¦¬ν°
// 1. Tuple: νν, λ³΄λ€ μκ²©νκ² νμμ μ μνκ³  μΆμ λ μ¬μ©
let x : [number, string];
x = [27, "AYW"];

// enum
enum Color {
	Red, Green, Blue
}

console.log(Color)
ππ½ { 0: 'Red', 1: 'Green', 2: 'Blue', Red: 0, Green: 1, Blue: 2 }

 - κ°μ ν λΉν΄μ£Όμ§ μμΌλ©΄ 0, 1, 2κ° λ€μ΄κ°λ€.

enum Color {
	Red = 2, Green, Blue
  }

console.log(Color[2])
ππ½ Red

// any
let num: any = "123";

// void: ν¨μκ° λ¦¬ν΄νλ κ°μ΄ μμ λ μ¬μ©νλ νμ
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
    /* κΈ°λ₯ */
  }
}

// νμ λ³μΉ­
let x: number = 10;
let xPositina: number = 10;

type YesOrNo = string;
type YesOrNoDetail = "Y" | "N";

let sayMe: YesOrNo = "HI";
let sayYou: YesOrNoDetail = "Y"

// μΈμκ° μκ³  λ¦¬ν΄ κ°μ΄ string νμμΈ type μ§μ 
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

// interfaceλ μμ± κ°λΌλ¦¬ ν©μΉ  μ μλ€.
interface IUser{
  id: number;
  name: Name;
  email: string;
  age: number;
}

interface IUser {address: string}

// type λ³μΉ­μ λΆκ°λ₯νλ€.
type IUser{
  id: number;
  name: Name;
  email: string;
  age: number;
}

type IUser {address: string}
ππ½ Error. Duplicate identifier 'IUser'.

// keyof: νμμ μλ μμ±κ°λ€μ νλμ νμμΌλ‘ λ¬Άλλ€.
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

### β type utility μμλ³΄κΈ°

1. `typescript`λ μΌλ°μ μΈ νμ λ³νμ μ½κ² νκΈ° μν΄μ λͺ κ°μ§ μ νΈλ¦¬ν° νμμ μ κ³΅ν©λλ€. μ΄λ¬ν μ νΈλ¦¬ν°λ μ μ­μΌλ‘ μ¬μ© κ°λ₯ν©λλ€.

```typescript

// Partial<T>: type μ§ν©μ λͺ¨λ  νλ‘νΌν°λ₯Ό μ νμ μΌλ‘ νμμ μμ±νλ€.
// Partial λμ  ?λ₯Ό μ¨λ λλ€.
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

// Readonly<T>: μ²μ μ€μ ν κ°μΈμ μμ±μ μμ  ν  μ μλ€. μ¬ν λΉ κΈμ§
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

ππ½ Cannot assign to 'id' because it is a read-only property.

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
ππ½ Cannot assign to 'gender' because it is a read-only property.

// Record<K, T>: κ°μ²΄μ μμ±κ³Ό νμμ μ μν  λ μ¬μ©νλ λ©μλ
type Grade = "1" | "2" | "3" | "4";
type Score = "A" | "B" | "C" | "D";

const score: Record<Grade, Score> = {
    1: "A",
    2: "B",
    3: "C",
    4: "D",
}

console.log(score)

// Record<K, T>: νμμ νλ‘νΌν° ν€μ μ§ν©μΌλ‘ νμμ μμ±νλ€. κ°μ²΄μ μμ±κ³Ό νμμ μ μν  λ μ¬μ©νλ λ©μλ
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

// Pick<T, K>: Typeμμμ Keyκ°μ μ ννμ¬ μλ‘ typeμΌλ‘ μ νλ κΈ°λ₯
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

// Omit<T, K>: Typeμμμ Keyκ°μ μ ννμ¬ μ¬μ©νμ§ λͺ»νκ² νλ€.
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

// Exclude<T1, U>: μμ± λμ  Typeμ key κ°μ μ μΈνλ€.
type T1 = string | number | boolean;
type T2 = Exclude<T1, number | string>;

let isNum: T2 = 3;
ππ½ Type 'number' is not assignable to type 'T2'.

let isNum: T2 = true;

// NonNullable<T>: undefinedμ null νμμ μ κ±°νλ€.
type T1 = string | null | undefined | void;
type T2 = NonNullable<T1>;

let empty: T2 = null;
ππ½ Type 'null' is not assignable to type 'T2'.
let empty: T2 = "Hi";

// Parameters<T>: ν¨μ νμμ μΈμλ‘ λ°μμ νννμμΌλ‘ λ¦¬ν΄ν΄μ£Όλ λ¬Έλ²
type T0 = Parameters<() => string>;  // []
type T1 = Parameters<(s: string) => void>;  // [string]
type T2 = Parameters<(s: string, i: number) => number>

let T1Arr: T1 = ["123"];

// ReturnType<T>: return typeκ°μ μ μνλ λ¬Έλ²
type T0 = ReturnType<() => string>;

function returnString(): T0{
    return "123"
}

type T7 = ReturnType<any> // any
type T8 = ReturnType<never> // any

// Required<T>: partialκ³Ό λ°λλλ κΈ°λ₯μΌλ‘ typeμ§ν©μ λͺ¨λ  νλ‘νΌν°λ₯Ό νμλ‘ μ€μ νλ€.
interface User {
    id: number;
    name?: string
}

let admin: Required<User> = {
    id: 1,
}

ππ½ Property 'name' is missing in type '{ id: number; }' but required in type 'Required<User>'.

let admin: Required<User> = {
    id: 1,
		name: "AYW"
}
```

### β νμμ€ν¬λ¦½νΈμ ν¨μ

1. μΌκΈκ°μ²΄(first-class object): ν¨μλ₯Ό λ³μλ‘ μ μΈνκ³ , ν¨μμ μΈμλ₯Ό ν¨μλ‘ λκΈΈ μ μκ³ , ν¨μμ λ¦¬ν΄κ°μ ν¨μλ‘ μ€μ ν  μ μλ κ²μ μΌκΈκ°μ²΄λΌ λΆλ¦λλ€. `JS` μ `TS` λ λͺ¨λ μΌκΈκ°μ²΄μλλ€.
2. μΌκΈκ°μ²΄μ νΉμ§ λλ¬Έμ κ³ μ°¨ν¨μ, μ½λ°±ν¨μλ₯Ό λ§λ€ μ μλ€.

```ts
// ν¨μ μμ²΄λ₯Ό κ°μΌλ‘ μ μ₯νλ€.
let sum = function (a, b) {
    return a + b;
};

function ul(child) {
    return `<ul>${child}</ul>`;
}

// ν¨μλ₯Ό λ¦¬ν΄ν  μ μλ€.
function makeLi(container, contents) {
    const liList = [];

    for (const content of contents) {
        liList.push(`<li>${content}</li>`);
    }

    return container(liList.join(""));
}

// ν¨μλ₯Ό ν¨μμ μΈμλ‘ λ£μ΄μ€ μ μλ€.
const htmlUl = makeLi(ul, ["μ", "ν", "μ", "λͺ©", "κΈ", "ν ", "μΌ"]);
```

3. ν¨μμ μ μΈλ¬Έ, μ μΈμ

```ts
// ν¨μ μ μΈλ¬Έ
function sum(a, b) {
    return a + b;
}

// ν¨μ ννμ
const myFunc = function (a, b) {
    return a + b;
};
```

4. ν¨μμ κ°λ³μΈμ

```ts
function sum(a, b) {
    return a + b;
}

const abcSum = sum(10, 20, 30);

// κ°λ³ μΈμμ
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

4. ν¨μ νΈμΆ

```ts
// callκ³Ό applyλ μΈμλ₯Ό νλμ© λκ²¨μ£Όλ λ°°μ΄λ‘ λκ²¨μ£Όλμ μ°¨μ΄
sum(10, 20, 30, 40);
// μ»¨νμ€νΈ null
sum.call(null, 10, 20, 30, 40);

arr = [10, 20, 30, 40];
sum.apply(null, arr);
```

5. ν¨μμ μ’λ₯

```ts
// μ¦μ μ€ν ν¨μ
(function () {
    console.log(123);
});

// μΌλ°ν¨μμ νμ΄νν¨μμ μ°¨μ΄:  μ»¨νμ€νΈμ μ°¨μ΄μ 
const sumV2 = (a, b, ...args) => {};

const ten = () => 100;
const hundred = (x) => 100 + x;

// μμ±κΈ° ν¨μ(generate function): ν¨μλ₯Ό νλ²μ μ€νμν€λ κ²μ΄ μλλΌ νμ λκ³  μ€νν  λ
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

6. ν¨μ μμ±μ λ°ν νμ λͺμ κΆμ₯(νμλ μλ, `TS` μ»΄νμΌλ¬λ λ°©μ μμ νμͺ½μλ§ νμμ΄ μλλΌλ νμμ μΆλ‘ ν  μ μλ€.)
7. λ§€κ°λ³μμ μΈμμ νμμ΄ νΈν κ°λ₯νκ² μμ±, μΈμ νμμ μ λ¬μ΄ μλͺ»λ κ²½μ° μ€λ₯ λ°μ

```ts
// ν¨μλ₯Ό μμ νκ² λ§λ€ μ μλ€.
interface MathFn {
    (a: number, b: number): number;
    operator: string;
};

const sum: MathFn = (a, b) => a + b;
sum.operator = "+";

1. void: λ°νκ°μ΄ μλ ν¨μμλλ€. (κ·Έλ₯ μΆλ ₯νκ±°λ, μνλ₯Ό λ°κΏ λ μμ£Ό μλλ€.)
2. never: ν¨μκ° μ’λ£λμ§ μμ΅λλ€. (λ¬΄νλ£¨νλ₯Ό λκ±°λ, Errorλ₯Ό λμΈ λ μ¬μ©ν©λλ€.)
```

8. ν¨μμ λ§€κ°λ³μ: ν¨μμ μ£Όμ΄μ§ μΈμμ κ°μλ ν¨μκ° κΈ°λνλ λ§€κ°λ³μμ μμ μΌμΉν΄μΌ ν¨

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
ππ½ "Bob Smith"


[LOG]: "Bob Smith"
[LOG]: "Bob Ted"

console.log(result2)
console.log(result3)

undefinedκ° λμ΄κ°λ©΄ lastNameμ΄ μλ€κ³  νλ¨λμ§λ§, nullμ΄ λ€μ΄κ°λ©΄ lastNameμ΄ μλ€κ³  νλ¨μ ν©λλ€.
(undefinedλ κ° μμ²΄κ° μλ€κ³  νλ¨νλ, nullμ κ°μ μλλ° μλ―Έμλ νΉλ³ν κ°μ΄ λ€μ΄μλ€κ³  λ³΄μλ©΄ μ’μ κ² κ°μμ.)
+ undefinedλ λ―Έλ¦¬ μ μΈλ global variableμ΄λ, nullμ ν€μλμλλ€.
```

### β κ°μ²΄ μ§ν₯ νλ‘κ·Έλλ°(OOP)

1. `OOP` λ μ»΄ν¨ν° νλ‘κ·Έλ¨μ κ°μ²΄μ λͺ¨μμΌλ‘ νμνλ €λ νλ‘κ·Έλλ° ν¨λ¬λ€μ
2. νλ‘κ·Έλ¨μ μ μ°νκ³ , λ³κ²½μ΄ μ©μ΄νκ³ , κ°λ°κ³Ό λ³΄μλ₯Ό κ°νΈνκ² λ§λ λ€, μ§κ΄μ μΈ μ½λ λΆμμ΄ κ°λ₯ν΄μ§λ€.
3. ν΄λμ€ μμ: νλ(field), μμ±μ(constructor, κ°μ²΄κ° μ²μ μμ±λ  λ νΈμΆ, λ©€λ² λ³μ μ΄κΈ°ν), λ©μλ(method)
4. μΈμ€ν΄μ€: `new` μ°μ°μμ μν΄μ μμ±λ κ°μ²΄

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

### β ν΄λμ€ λ§λ€κΈ°

1. μμ±μμ λ§€κ°λ³μμ `public` κ³Ό κ°μ μ κ·Ό μ νμλ₯Ό λΆμ΄λ©΄ ν΄λΉ λ§€κ°λ³μμ μ΄λ¦μ κ°μ§ μμ±μ΄ ν΄λμ€μ μ μΈλ κ²μ²λΌ λμν©λλ€.

```ts
// public μ κ·Ό μ νμ
class Information {
  constructor(public name: string, public age: number){}
}

const myInfo = new Information("AYW", 27);
console.log(myInfo)
ππ½ { name: 'AYW', age: 27 }

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
ππ½ { name: 'AYW', age: 27 }
```

### β ν΄λμ€ μμλ°κΈ°

1. λΆλͺ¨ ν΄λμ€λ₯Ό μμλ°λ ν€μλ: `extends`

```ts
class AYW extends Information{
  constructor(public name: string, public age: number, gender: "male" | "female"){
    super(name, age)
  }

  sayHello(): void {
    console.log(`μ  μ΄λ¦μ ${this.name}μλλ€.`)
  }
}

const myInfo: AYW = new AYW("AYW", 27, "male")
console.log(myInfo);
ππ½ AYW { name: 'AYW', age: 27 }

myInfo.sayHello();
ππ½ μ  μ΄λ¦μ AYWμλλ€.
```

### β μΆμ ν΄λμ€

1. μΆμ ν΄λμ€λ μμ μ μμ±μ΄λ λ©μλ μμ `abstract`λ₯Ό λΆμ¬ λλ₯Ό μμνλ λ€λ₯Έ ν΄λμ€μμ μ΄ μμ±μ΄λ λ©μλλ₯Ό κ΅¬ννκ² ν©λλ€.

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
        console.log(`μ  μ΄λ¦μ ${this.name}μλλ€.`);
    }
}

const myInfo: AYW = new AYW("AYW", 27, "male");
console.log(myInfo);
ππ½ AYW { name: 'AYW', age: 27 }

myInfo.sayHello();
ππ½ μ  μ΄λ¦μ AYWμλλ€.
```

---

## π 22μΌμ°¨ 11.24.μ.(μ¨λΌμΈ κ°μ)

μ€λμ μ΄μ  λ°°μ λ λ΄μ©μ κ°μλ₯Ό ν΅ν΄ λ€μ νλ² λ°°μ°λ μκ°μ κ°μ‘λ€. ν΄λ¦°μ½λ, νμμ€ν¬λ¦½νΈ μ μ, `type`, `utility` λ±λ±μ λν΄μ λ€μ λ°°μλ³΄μ.

### β ν΄λ¦°μ½λλ

1. ν΄λ¦° μ½λλ λ§ κ·Έλλ‘ κΉ¨λνκ² μμ±λ μ½λλ₯Ό μλ―Έν©λλ€. κΉ¨λνκ² μμ±λ μ½λλ μ§μ μ μ΄κ³  λ¨μνμ¬ μ½κΈ°κ° μ½κ³ , μ½λ μμ±μκ° μλ λκ° λ³΄λλΌλ μλκ° λͺνν λλ¬λλ μ½λμλλ€. μ΄λ¬ν μ½λλ κ°λμ±μ΄ μ’κ³ , μμ‘΄μ±μ μ΅λν μ€μ¬ μ μ§λ³΄μκ° μ¬μ΄ νΉμ§μ΄ μμ΅λλ€.
2. νλ‘κ·Έλλ¨Έλ μμ± κΈ°νμ λ§μΆκΈ° μν΄μ λμ μ½λλ₯Ό μμ°ν  μλ°μ μλ€κ³  μκ°ν©λλ€. νμ§λ§ λμ μ½λλ₯Ό μμ°νλ©΄ κ²°κ΅­ κΈ°νμ λ§μΆμ§ λͺ»ν©λλ€. μ€νλ € μλ§μ§μ°½μΈ μ½λ λλ¬Έμ κ°λ° μλκ° λλ €μ§κ³  κ²°κ΅­ κΈ°νμ λμΉ©λλ€. κΈ°νμ λ§μΆλ μ μΌν λ°©λ²μΒ μΈμ λ μ½λλ₯Ό μ΅λν κΉ¨λνκ² μ μ§νλ κ²μλλ€.

### β ν΄λ¦°μ½λμ νμμ€ν¬λ¦½νΈ

1. μλ°μ€ν¬λ¦½νΈλ νμμ΄ μκΈ° λλ¬Έμ μ€ν νμ νμ μλ¬λ₯Ό νμΈν  μ μμ΅λλ€. λ°λ©΄ νμμ€ν¬λ¦½νΈλ κ°μ μ½λμ λν΄ μλμ κ°μ΄ μ€νμ νκΈ° μ μ, λ―Έλ¦¬ μλ¬λ₯Ό νμΈν  μ μμ΅λλ€. μλ°μ€ν¬λ¦½νΈμ λ°νμ λ¨κ³μμ λ°μνλ νμ μλ¬λ₯Ό νμμ€ν¬λ¦½νΈμμλ μ»΄νμΌ λ¨κ³μμ λ―Έλ¦¬ νμΈνκ³  κ³ μΉ  μ μλ€. λ§μ½, λ°νμ λ¨κ³μμ λ°μνλ μλ¬λ‘ μΈν΄ νλ‘κ·Έλ¨μ΄ λ©μΆλ©΄, μ΄μλλ μλΉμ€μ ν° μ°¨μ§μ΄ μκΈΈ μ μλ€. νμμ€ν¬λ¦½νΈλ₯Ό μ¬μ©νλ©΄ μλ¬λ₯Ό λ―Έλ¦¬ λ°©μ§ν  μ μλ€.
2. νμμ μ μν¨μΌλ‘μ¨ κ°λ°μμ μ€μλ₯Ό μ€μΌ μ μκ³ , λͺμλ νμμ λ³΄κ³  ν΄λΉ λ³μμ μλ£νμ΄ λ¬΄μμΈμ§ μ½κ² μ΄ν΄ν  μ μλ€. κ²°κ³Όμ μΌλ‘ μ΄λ μ©λλ‘ μ½λκ° μμ±λμκ³ , λ¬΄μμ μλ―Ένλμ§ νμνκΈ° ν¨μ¬ μ©μ΄νκΈ° λλ¬Έμ μ μ§λ³΄μμ μ λ¦¬νκ³  μμ°μ€λ½κ² κ°λ° μλλ λΉ¨λΌμ§κ² λλ€.

### β νμμ€ν¬λ¦½νΈλ?

1. `microsoft` μμ κ°λ°ν μ€ν μμ€ μΈμ΄
2. μλ°μ€ν¬λ¦½νΈμ μμ μ§ν©, JSμ νκ³λ₯Ό ν΄κ²°
3. νμμ€ν¬λ¦½νΈλ₯Ό μ€ννλ €λ©΄ μλ°μ€ν¬λ¦½νΈλ‘ λ³ννλ μ»΄νμΌκ³Όμ μ΄ νμνλ€.
4. λμ νμμ μ μ μΌλ‘ μ¬μ©κ°λ₯
5. νμ μ μΆλ‘ νμ μ μ΄ κ°λ₯
6. μ»΄νμΌ μμ μ μ€λ₯ ν¬μ°© κ°λ₯
7. JSμμ μ°Ύμ μ μλ μΆκ°μ½λ κΈ°λ₯ μ κ³΅

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
b = "b"; // Error(μ»΄νμΌ μμ )

const sum = (a: number, b: number) => {
    return a + b;
};

sum(1, 2); // 12
```

### β νμμ€ν¬λ¦½νΈμ κΈ°λ³Έ Type

1. JSμ½λμ λ³μ ν¨μ λ±μ type μ μ κ°λ₯
2. νμ νκΈ°(type annotation)μ μ¬μ©νλ€.
3. κΈ°λ³Έμλ£ν(primitive type): `string`, `boolean`, `number`, `null`, `undefined`, `symbol(ES6)`

```typescript
// string
let str: string = "hi";

// boolean
let isSucceeded: boolean = true;

// number: 2μ§μ, 8μ§μ, 10μ§μ, 16μ§μ μ¬μ© κ°λ₯
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

4. μ°Έμ‘°μλ£ν(reference type): object, array, function

```typescript
// κ°μ²΄, λ°°μ΄, ν¨μ λ±κ³Ό κ°μ Object νμμ νμ, λ©λͺ¨λ¦¬μ κ°μ μ£Όμλ‘ μ μ₯νκ³ , μΆλ ₯μ λ©λͺ¨λ¦¬ μ£Όμμ μΌμΉνλ κ°μ μΆλ ₯
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

5. μΆκ° μ κ³΅ μλ£ν: tuple, enum, any, void, never

```typescript
// tuple: κΈΈμ΄μ κ° μμμ νμμ΄ μ ν΄μ§ λ°°μ΄μ μ μ₯νλ νμ
let arr: [string, number] = ["Hi", 122];
arr[1].concat("1")  // Error: 'number' does not have 'concat'
arr[3] = "hello"  // Error: Property '3' does not exist on type [string, number]

// enum: νΉμ  κ°λ€μ μ§ν©μ μ μ₯νλ νμ
enum Car {BUS, TAXI, SUV};
let bus: Car = Car.BUS;
let taxi: string = Car[2];

console.log(bus, taxi)
ππ½ 0 "SUV"

enum Car {BUS = 2, TAXI, SUV};
let bus: Car = Car.BUS;
let taxi: string = Car[3];

console.log(bus, taxi)
ππ½ 2 "TAXI"

// any: λͺ¨λ  νμ μ μ₯ κ°λ₯, μ»΄νμΌ μ€ νμ κ²μ¬λ₯Ό νμ§ μμ
let str: any = "hi";
let num: any = 1;
let arr: any = [1, 2, 3];

// void: λ³΄ν΅ ν¨μμμ λ°ν κ°μ΄ μμ λ μ€μ νλ νμ
let unknown: void = undefined;
function sayHi(): void {
  console.log("hi")
}

// never: μ λ λ°μν  μ μλ νμ, μ’λ£λμ§ μλ ν¨μ, ν­μ μ€λ₯λ₯Ό λ°μμν€λ ν¨μ
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

### β νμμ€ν¬λ¦½νΈμ Utility

1. Typescriptλ κ³΅ν΅ νμ λ³νμ μ©μ΄νκ² νκΈ° μν΄ μ νΈλ¦¬ν° νμμ μ κ³΅νλ€.
2. μ νΈλ¦¬ν° νμμ μ μ­μΌλ‘ μ¬μ© κ°λ₯νλ€
3. `Partial<T>`, `Readonly<T>`, `Record<T>`, `Pick<T, K>`, `Omit<T, K>`, `Exclude<T, U>`. `Extract<T, U>`, `NonNullable<T>`, `Parameters<T>` , `ConstructorParameters<T>`, `ReturnType<T>`, `Required<T>`
4. μ λ€λ¦­μ΄λ μ΄λ€ ν¨μλ ν΄λμ€κ° μ¬μ©ν  νμμ μμ± λ¨κ³κ° μλ μ¬μ© λ¨κ³μμ μ μνλ νλ‘κ·Έλλ° κΈ°λ²μλλ€.

```typescript
// Partial<T>: νλ‘νΌν°λ₯Ό μ νμ μΌλ‘ λ§λλ νμμ κ΅¬μ±νλ€.
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
ππ½ { title: 'organize desk', description: 'clear clutter' } { title: 'organize desk', description: 'throw out trash' }

// Readonly<T>: νλ‘νΌν°λ₯Ό μ½κΈ° μ μ©μΌλ‘ μ€μ νλ€.
interface Todo {
  title: string;
}

const todo1: Readonly<Todo> = {
  title: 'organize desk',
}

todo1.title = "Hello" // Error: Cannot assign to 'title' because it is a read-only property.

// Record<T>: νλ‘νΌν°μ μ§ν© Kλ‘ νμμ κ΅¬μ±νλ€. νμμ νλ‘νΌν°λ€μ λ€λ₯Έ νμμ λ§€νμν€λλ° μ¬μ©νλ€.
interface PageInfo {
  title: string;
}

type Page = "home" | "about" | "contact";

const x: Record<Page, PageInfo> = {
  about: {title: 'about'},
  contact: {title: 'contact'},
  home: {subTitle: 'home'}  // Error: Type '{ subTitle: string; }' is not assignable to type 'PageInfo'.  Object literal may only specify known properties, and 'subTitle' does not exist in type 'PageInfo'
}

// Pick<T, K>: νλ‘νΌν° Kμ μ§ν©μ μ νν΄ νμμ κ΅¬μ±νλ€.
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

// Omit<T, K>: λͺ¨λ  νλ‘νΌν°λ₯Ό μ νν λ€μ Kλ₯Ό μ κ±°ν νμμ κ΅¬μ±νλ€.
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

// Exclude<T, U> : νμ Tμμ Uμ κ²ΉμΉλ νμμ μ μΈν νμμ κ΅¬μ±ν©λλ€.
// Extract<T, U> : νμ Tμμ Uμ κ²ΉμΉλ νμλ§ ν¬ν¨νμ¬ νμμ κ΅¬μ±ν©λλ€.
// NonNllable<T> : T νμμμ nullκ³Ό undefinedλ₯Ό μ μΈν νμμ κ΅¬μ±ν©λλ€.
// Parameter<T> : ν¨μ νμ Tμ λ§€κ°λ³μμ νμλ€μ ννλ‘ νμμ κ΅¬μ±ν©λλ€.
// ConstructorParameters<T> : ν΄λμ€μ μμ±μλ₯Ό λΉλ‘―ν μμ±μ νμμ λͺ¨λ  λ§€κ°λ³μ νμμ μΆμΆν©λλ€.
// ReturnType<T> : ν¨μ Tκ° λ°νν νμμΌλ‘ νμμ κ΅¬μ±ν©λλ€.
// Required<T> : νμ Tμ λͺ¨λ  νλ‘νΌν°κ° νμλ‘ μ€μ λ νμμ κ΅¬μ±ν©λλ€.
```

### β ν¨μ μ¬μ©νκΈ°

1. ν¨μλ₯Ό μ μ ν  λ μ¬μ©λλ λ³μλ λ§€κ°λ³μμ΄κ³  νΈμΆ ν  λ μ¬μ©λλ κ°μ μΈμλΌκ³  νλ€.

```typescript
function add(x, y) {
    // λ§€κ°λ³μ
    return x + y;
}

add(2, 5); // μΈμ
```

2. μΌκΈκ°μ²΄(first-class object): λ€λ₯Έ κ°μ²΄λ€μ μΌλ°μ μΌλ‘ μ μ© κ°λ₯ν μ°μ°μ λͺ¨λ μ§μνλ κ°μ²΄

```typescript
1. λ€λ₯Έ ν¨μμ λ§€κ°λ³μλ‘ μ κ³΅ν  μ μλ€.
2. ν¨μμμ λ°νμ΄ κ°λ₯νλ€
3. λ³μμ ν¨μλ₯Ό ν λΉν  μ μλ€.
```

3. ν¨μ μ μΈμ, ν¨μ ννμ

```typescript
// ν¨μ μ μΈμ
function world(name) {}

// ν¨μ ννμ
const hi = function (name) {};

// ν¨μ μμ±μλ λλλ‘ μ¬μ©μ κΆνμ§ μλλ€
let world5 = new Function();
```

4. `TS` μμ ν¨μ μμ±μ λ°ν νμμ μΆλ‘ νλλ‘ νλκ±Έ κΆμ₯νλ€.
5. `TS` μ»΄νμΌλ¬λ λ°©μ μμ νμͺ½μλ§ νμμ΄ μμ΄λ νμμΆλ‘ μ΄ κ°λ₯νλ°, μ΄λ₯Ό `contextual typing` μ΄λΌκ³  λΆλ₯Έλ€. μ΄λ₯Ό ν΅ν΄ νλ‘κ·Έλ¨μμ νμμ μ μ§νκΈ° μν λΈλ ₯μ μ€μΌ μ μλ€.

### β ν¨μμ λ§€κ°λ³μ

1. κΈ°λ³Έ λ§€κ°λ³μ: ν¨μμ μ£Όμ΄μ§ μΈμμ μλ ν¨μκ° κΈ°λνλ λ§€κ°λ³μμ μμ μΌμΉν΄μΌ νλ€.

```typescript
function buildName(firstName: string, lastName: string) {
    return firstName + lastName;
}

let result1 = buildName("a", "b");
let result2 = buildName("a", "b", "c"); // Error: Expected 2 arguments, but got 3.
```

2. μ νμ  λ§€κ°λ³μ: `JS` μμλ μΈμκ° μμΌλ©΄ `undefined` λ‘ μ μΈμ΄λλ€. `TS` μμλ λ³μλͺ λ€μ `?` λ₯Ό μ¬μ©νλ©΄ λ³μλ₯Ό μ νμ μΌλ‘ μ¬μ©ν  μ μλ€.
3. κΈ°λ³Έ-μ΄κΈ°ν λ§€κ°λ³μ: `TS` μμ κ°μ μ κ³΅νμ§ μκ±°λ, `undefined` λ‘ νμ λ λ§€κ°λ³μμ κ° ν λΉ κ°λ₯

```typescript
function buildName(firstName: string, lastName: string = "TED") {
    return firstName + lastName;
}

let result1 = buildName("a"); // aTED
let result1 = buildName("a", undefined); // aTED
let result1 = buildName("a", "morning"); // amorning
```

4. λλ¨Έμ§ λ§€κ°λ³μ: `...` μ λ£μ΄μ£Όμ΄ λ§€κ°λ³μμ μλ₯Ό λ¬΄νμΌλ‘ μ·¨κΈν  μ μλ€. μλ¬΄κ²λ λκ²¨μ£Όμ§ μμΌλ©΄ `[]` μ΄ ν λΉλλ€.

```typescript
function buildName(firstName: string, ...lastName: string[]) {
    return firstName + lastName;
}

let result1 = buildName("a", "SON", "Ted"); // aSON,Ted
```

### β OOP

1. κ°μ²΄ μ§ν₯ νλ‘κ·Έλλ°: μ»΄ν¨ν° νλ‘κ·Έλ¨μ κ°μ²΄μ λͺ¨μμΌλ‘ νμνλ €λ νλ‘κ·Έλλ° ν¨λ¬λ€μμ΄λ€. κ°μ²΄λ€μ μλ‘ λ©μΈμ§λ₯Ό μ£Όκ³  λ°μΌλ©° λ°μ΄ν°λ₯Ό μ²λ¦¬ν  μ μλ€.
2. μ₯μ : νλ‘κ·Έλ¨μ μ μ°νκ³ , λ³κ²½μ΄ μ©μ΄νκ² λ§λ€μ΄μ§λ©°, κ°λ°κ³Ό λ³΄μλ₯Ό κ°νΈνκ² λ§λ λ€, μ§κ΄μ μΈ μ½λ λΆμμ κ°λ₯νκ² νλ€.
3. μ€μν νΉμ±: κ°ν μμ§λ ₯κ³Ό μ½ν κ²°ν©λ ₯μ μ§ν₯νλ€.

### β Class

1. ν΄λμ€μ μμ: λ©€λ², νλ, μμ±μ, λ©μλ
2. μΈμ€ν΄μ€: `new` μ°μ°μμ μν΄ μμ±λ κ°μ²΄

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

### β Class μ κ·Ό μ μ΄μ

1. μμ±, λ©μλλ‘μ μ κ·Όμ μ ννκΈ° μν΄ μ¬μ©νλ€.
2. `public`, `protected`, `private`
3. `Java` μ λ€λ₯΄κ² `package` κ°λμ΄ μμ΄ `default` μ κ·Ό μ μ΄μλ μλ€.
4. `public`: νλ‘κ·Έλ¨ λ΄ μ μΈλ λ©€λ²λ€μ΄ μμ λ‘­κ² μ κ·Όν  μ μλ€. κΈ°λ³Έμ μΌλ‘ `public` μΌλ‘ μ μΈλλ€. λͺμμ μΌλ‘ `public` μ μΈλ κ°λ₯νλ€.

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

5. `private` :λ©€λ²κ° ν¬ν¨λ ν΄λμ€ μΈλΆμμ μ κ·Όμ λ§λλ€.

```typescript
class Person {
    private name: string;
    constructor(name: string) {
        this.name = name;
    }
}

new Person("TED").name; // Error: Property 'name' is private and only accessible within class 'Person'.
```

6. `protected`: λ©€λ²κ° ν¬ν¨λ  ν΄λμ€μ κ·Έ νμ ν΄λμ€ μΈλΆμμμ μ κ·Όμ λ§λλ€. (λ΄λΆμμλ μ κ·Όμ΄ κ°λ₯νμ§λ§, μΈλΆμμμ μ κ·Όμ λΆκ°νλ€)

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

### β Class μμ

1. μμμ μ΄μ©νμ¬ μ‘΄μ¬νλ ν΄λμ€λ₯Ό νμ₯ν΄ μλ‘μ΄ ν΄λμ€λ₯Ό μμ±ν  μ μλ€. `extends`
2. νμλ ν΄λμ€λ νμν΄λμ€(subclass), κΈ°μ΄ ν΄λμ€λ μμ ν΄λμ€(super class)λΌκ³  λΆλ₯Έλ€.

```typescript
class Animal {
    move(distanceInMeters: number) {
        console.log(`Animal moved ${distanceInMeters}m.`);
    }
}

class Dog extends Animal {
    makeSound() {
        console.log(`λ©λ©`);
    }
}

const dog = new Dog();
dog.move(10);
```

### β Getters & Setters

1. λΉκ³΅κ°λ‘ μ€μ νλ €λ μμ±μ `private` λ‘ μ€μ νκ³ , μμ±κ°μ μ½κ³  μμ νλ `getter/setter` ν¨μλ₯Ό μ¬μ©νλ€.
2. `class` μ μ§μ  μ μ©νλκ²μ λ§κ³ , ν¨μλ₯Ό μ¬μ©ν΄ κ°μ λ°μμ€κ±°λ μμ νλ€. μμ±μ μ§μ  μ κ·Όν΄ μμ νλ©΄ λ°μ΄ν° λ¬΄κ²°μ±μ΄ κΉ¨μ§ μ μλ€. (μΊ‘μν κΆμ₯)
3. κ° κ°μ²΄μ λ©€λ²μ μ κ·Όνλ λ°©λ²μ μΈλ°νκ² μ μ΄ν  μ μλ€.

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

### β Readonly

1. μ½κΈ°λ§ κ°λ₯ν μμ±μ μ μΈνκΈ° μν΄ μ¬μ©νλ€. (λ³κ²½ ν  μ μλ€.)
2. μ μΈλ  λλ μμ±μμμ κ°μ μ€μ νλ©΄ μ΄ν μμ ν  μ μλ€.

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

### β static

1. μ μ­ λ©€λ²λ₯Ό μ μΈν  λ μ¬μ©νλ€. (μ μ­λ©€λ²: κ°μ²΄λ§λ€ ν λΉλμ§ μκ³ , ν΄λμ€μ λͺ¨λ  κ°μ²΄κ° κ³΅μ νλ λ©€λ²)
2. μΈμ€ν΄μ€κ° μλ ν΄λμ€ μμ²΄μμ λ³΄μ΄λ μ μ­ λ©€λ²λ₯Ό μμ±νλ€.
3. λ²μ©μ μΌλ‘ μ¬μ©λλ κ°μ μ€μ νλ€.
4. `ν΄λμ€λͺ.` μ μμ λΆμ¬ `static` λ©€λ²μ μ κ·Όν  μ μλ€.
5. `ES6` μμ λ©μλ μ μ© μμ±μλ μ μΈμ΄ μλμμΌλ, `TS` μμλ μ¬μ©κ°λ₯νλ€.

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

### β μΆμν΄λμ€

1. λ€λ₯Έ ν΄λμ€λ€μ΄ νμλ  μ μλ κΈ°μ΄ν΄λμ€
2. μ§μ  μΈμ€ν΄μ€ν λ  μ μλ€.
3. `abstract` ν€μλλ μΆμ ν΄λμ€λ μΆμ λ©μλλ₯Ό μ μνλλ° μ¬μ©λλ€.
4. μΆμ λ©μλλ ν΄λμ€μλ κ΅¬νλμ΄ μμ§ μκ³ , νμλ μμ ν΄λμ€μμ κ΅¬νν΄μΌ νλ€.

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
        super(name); // νμλ ν΄λμ€μ μμ±μλ λ°λμ super()λ₯Ό νΈμΆ
    }

    makeSound(): void {
        console.log(this.name + "λ©λ©");
    }
}

const animal = new Animal("animal"); // Error: Cannot create an instance of an abstract class.
const dog = new Dog("μ§λκ°"); // Dog { name: 'μ§λκ°' }
```

### π‘Β μΆμ ν΄λμ€λ₯Ό νμ©ν λμμΈ ν¨ν΄

1. νλ‘κ·Έλ¨μ μΌλΆλΆμ μλΈ ν΄λμ€λ‘ μΊ‘μνν΄ μ μ²΄ κ΅¬μ‘°λ₯Ό λ°κΎΈμ§ μκ³  νΉμ  λ¨κ³μ κΈ°λ₯μ λ°κΎΈλ κ²
2. μ μ²΄μ μΈ μκ³ λ¦¬μ¦μ μμ ν΄λμ€μμ κ΅¬ννκ³ , λ€λ₯Έ λΆλΆμ νμ ν΄λμ€μμ κ΅¬ννλ€.
3. μ μ²΄ κ΅¬μ‘°λ μ μ¬νμ§λ§, λΆλΆμ μΌλ‘ λ€λ₯Έ κ΅¬λ¬Έμμ μμ±λ λ©μλμ μ½λ μ€λ³΅μ μ΅μν ν  μ μλ€.

```typescript
abstract class Parent {
  public do(){
    console.log("Parentμμ μ€ν - μ") ;
    this.hook();
    console.log("Parentμμ μ€ν - ν");
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

ππ½
Parentμμ μ€ν - μ
child
Parentμμ μ€ν - ν
```

---

## π 23μΌμ°¨ 11.25.λͺ©(μ€μκ° κ°μ)

μ€λμ `interface`, `generic` λ¬Έλ²μ λν΄μ λ°°μ λ€.

### β Interface

1. νμ μ²΄ν¬λ₯Ό μν΄ μ¬μ©λλ©° λ³μ, ν¨μ, ν΄λμ€μ μ¬μ© κ°λ₯
2. μ§μ  μΈμ€ν΄μ€λ₯Ό μμ±ν  μ μμ. λͺ¨λ  λ©μλλ μΆμ λ©μλλ€. (μ΄λ `abstract` ν€μλλ₯Ό μ¬μ©νμ§ μλλ€)
3. μ μΈλ§ μ‘΄μ¬νλ€. (JSλ‘ λ³νλλ©΄ μΈν°νμ΄μλ μ¬λΌμ§λ€.)
4. `interface` κ°μ `extends` λ₯Ό μ¬μ©νμ¬ λ€μ€ μμ κ°λ₯(classμ λΉμ·)
5. μΆμ ν΄λμ€μ λ€λ₯Έμ : μΆμ `class`λ μ μ²΄μ μΈ κ΅¬μ‘°, `interface`λ νλ‘κ·Έλλ¨Έ κ°μ νμ κ°λ°μ ν  λ μ¬μ©
6. ν¨μμ λ§€κ°λ³μ(νλΌλ―Έν°λ‘)λ‘ μ¬μ©
7. `API` μλ΅μμ λ°μ΄ν°μ κ΅¬μ‘°λ₯Ό κ²°μ ν  λ μ¬μ©

```typescript
// ν€ κ°μ λ€μμ²λΌ μ ν΄μ£Όλ©΄ ν€ κ°μ μ νμ΄ μλ€.
interface User {
    [grade: number]: "A" | "B" | "C" | "D";
}

let user: User = {
    1: "A",
    2: "B",
    5: "D",
};
```

8. μ νμ  νλ‘νΌν°(?): `?`κ° λΆλ κ²½μ°λ λ°λμ κ΅¬νλμ§ μκ³  μ νκ°λ₯

```typescript
// ν€ κ°μ λ€μμ²λΌ μ ν΄μ£Όλ©΄ ν€ κ°μ μ νμ΄ μλ€.
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

9. ν΄λμ€ μ μΈλ¬Έμ `implements` λ₯Ό λΆμ¬μ μ¬μ© κ°λ₯(μΈν°νμ΄μ€λ₯Ό κ΅¬ννλ ν΄λμ€μ μΌκ΄μ±μ μ μ§ν  μ μλ μ₯μ μ κ°μ§)

```typescript
// λͺ¨λ  λ©μλλ μΆμ λ©μλμ¬μΌ νλ€.
// μΈν°νμ΄μ€μμ μ μν νμμ ν΄λμ€ μμμλ λͺ¨λ μ μ©ν΄μΌνλ€.
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
        console.log(`μλνμΈμ!!`);
    }
}

const today = new Todo(1, "TED", true); // μΈμ€ν΄μ€
console.log(today); // Todo { id: 1, content: 'TED', completed: true }
today.sayHello(); // μλνμΈμ!!
```

9. ν¨μμ λ³μμμλ λνμμ΄ μ μ©λλ€.(λ νμ΄ν: νμ μ²΄ν¬μμ μ€μν κ²μ κ°μ μ€μ  κ°μ§κ³  μλλμ κ΄ν κ², μΈν°νμ΄μ€μμ μ μν νλ‘νΌν°λ λ©μλλ₯Ό κ°μ§κ³  μλ€λ©΄ κ·Έ μΈν°νμ΄μ€λ₯Ό κ΅¬νν κ²μΌλ‘ μ¬κΉ λ νμ΄ν λλ κ΅¬μ‘°μ νμ΄νμ΄λΌ λΆλ¦)

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

### β λμμΈν¨ν΄

1. μμ±ν¨ν΄: κ°μ²΄λ₯Ό μμ±νλλ° κ΄λ ¨ν ν¨ν΄
2. κ΅¬μ‘°ν¨ν΄: νλ‘κ·Έλ¨μ κ΅¬μ‘°μ κ΄λ ¨ν ν¨ν΄
3. νμν¨ν΄: λ°λ³΅μ μΌλ‘ μ¬μ©λλ κ°μ²΄λ€μ μνΈμμ© ν¨ν΄

```typescript
// μ λ΅ ν¨ν΄
interface Weapon {
    attack: () => void;
}

class Sword implements Weapon {
    public attack() {
        console.log("κ² κ³΅κ²©");
    }
}

class Spear implements Weapon {
    public attack() {
        console.log("μ°½ κ³΅κ²©");
    }
}

class Bow implements Weapon {
    public attack() {
        console.log("ν κ³΅κ²©");
    }
}

class GameUser {
    private weapon: Weapon | null = null;

    public setWeapon(weapon: Weapon) {
        this.weapon = weapon;
    }

    public attack() {
        if (this.weapon === null) {
            console.log("λ§¨μ κ³΅κ²©");
        } else {
            this.weapon.attack();
        }
    }
}

const testUser = new GameUser();
testUser.setWeapon(new Spear());
testUser.attack(); // μ°½

testUser.setWeapon(new Bow());
testUser.attack(); // ν κ³΅κ²©

testUser.setWeapon(new Sword());
testUser.attack(); // κ² κ³΅κ²©

testUser.setWeapon(null);
testUser.attack(); // λ§¨μ κ³΅κ²©
```

### β μ λ€λ¦­(Generic)

1. λ°μ΄ν°νμμ μΌλ°ν ν¨
2. μλ£νμ μ νμ§ μκ³  μ¬λ¬ νμμ μ¬μ©ν  μ μκ² νλ€.(λ²μ©μ μΈ ν¨μλ₯Ό μ°κ³  μΆμ λ?, μ¬λ¬κ°μ§ νμμ μ¬μ©νκ³  μΆμ λ)
3. μ¬μ¬μ©μ±μ΄ λμ ν¨μλ₯Ό λ§λ€μ΄μ€λ μ¬μ©λ¨
4. νκ°μ§ νμλ³΄λ€ μ¬λ¬κ°μ§ νμμμ λμνλ ν¨μλ₯Ό μμ±νλ€.

```typescript
// class λ¬Έλ²μμμ μ λ€λ¦­
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

// μΈμ€ν΄μ€μ νμμ μ μ°νκ² μ€μ ν  μ μλ€.
const numberStack = new Stack<number>();
const stringStack = new Stack<string>();
numberStack.push(1);
stringStack.push("a");

// ν¨μμμμ μ λ€λ¦­
function getSize<T>(arr: T[]): number {
    return arr.length;
}

const arr1 = [1, 2, 3];
getSize<number>(arr1);

const arr2 = ["a", "b", "c"];
getSize<string>(arr2);
```

5. μ λ€λ¦­ν λ³μλ₯Ό μΆκ°νκ³  μΆμ λ `<T, U>`

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

// ν¨μμμμ μ λ€λ¦­
// <T>λ textμ μΈμλ Tλ‘ λ°κ³  λ¦¬ν΄κ°λ T νμμΌλ‘ ν΄μ€λ€.
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

// μ λ€λ¦­ μμ
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

### β Non-null assertion operator

1. `Null` μ΄ μλ μ΄μ μ μ°μ°μλ νΌμ°μ°μκ° `null` μ΄ μλλΌκ³  μ»΄νμΌλ¬μκ² μ λ¬νμ¬ μΌμμ μΌλ‘ `Null` μ μ½μ‘°κ±΄μ μνν©λλ€. κΆμ₯νμ§ μλ λ¬Έλ²μ΄κ³  λμ  `&&` μ μ¬μ©νλ€.

### β Union type

```typescript
// example1
function getAge(age: number | string) {
    return typeof age === "number" ? age.toFixed() : age;
}

const myAge = getAge(28);
console.log(myAge);

const yourAge = getAge("25");
console.log(yourAge);

// union κΈ°νΈ
interface Person {
    name: string;
    age: number;
}

interface Developer {
    name: string;
    skill: string;
}

// κ²ΉμΉλ μμ±λ§ μ¬μ© κ°λ₯
function introduce(someone: Person | Developer) {
    someone.name;
    someone.age; // Error
    someone.skill; // Error
}

// λͺ¨λ  μμ± μ¬μ© κ°λ₯
function introduce(someone: Person & Developer) {
    someone.name;
    someone.age; // μ¬μ© κ°λ₯
    someone.skill; // μ¬μ© κ°λ₯
}
```

### β μ μ½ μ‘°κ±΄(constraints / keyof)

1. μ λ€λ¦­ νμμ μ΄λμ λ ννΈλ₯Ό μ£Όκ³  μ μ½μ κ±ΈκΈ° μν΄ μ¬μ©, μ΅μν `length` μμ±μ΄ μμ΄μΌ μλ¬κ° λμ§ μλλ€

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
  console.log(text.area);  // κ³΅ν΅λλ μμ±μ΄ μλλ―λ‘ Errorκ° λλ€.
}

function logText1<T extends LengthWise & Rect>(text: T){
  console.log(text.length);
  console.log(text.area);  // λͺ¨λ  μμ± μ¬μ© κ°λ₯νλ―λ‘ Errorκ° λμ§ μλλ€.
```

### β keyofλ₯Ό μ¬μ©ν μ μ½

1. κ°μ²΄μ μμ±μ μ μ½νκ³  μΆμ λ μ¬μ©

```typescript
// κ°μ²΄ μμμμ μμ±λ§ μ¬μ©νλ λ¬Έλ²
function getProperty<T, O extends keyof T>(obj: T, key: O) {
    return obj[key];
}

let obj = { a: 1, b: 2, c: 3 };
// 'a' | 'b' | 'c'
console.log(getProperty(obj, "c"));
```

### β κΈ°ν κΈ°λ₯ λ° κ°λ

1. Type Assertion: νμ μΆλ‘ κΈ°λ₯μ κ°λ ₯νμ§λ§ νκ³ μ‘΄μ¬, νμλ¨μΈ(type assertion)μ νμμ€ν¬λ¦½νΈκ° μΆμ νμ§ λͺ»νλ λΆλΆκΉμ§ κ°λ°μκ° μ μΈνλκ²
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
// ν¨μ
function doSomeThing(id: string | number) {
    if (typeof id === "string") {
        console.log(id.trim());
    } else {
        console.log(id);
    }
}

// ν΄λμ€
class Diner {}
class Merchant {}

function doSomething(user: Diner | Merchant) {
    if (user instanceof Diner) {
    } else {
    }
}

// λ©μλ
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

// νμ νμΈ
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

### β μ€μ΅

1. ν΄λμ€ vs μΆμν΄λμ€: μ΄λ€ λ©μλλ κ·Έλ₯ κ΅¬νν΄λ λκ³ , μ΄λ€ λ©μλλ μ μ λμ§ μμ λ©μλ μΌ μ μλ€.(μ¬μ©νλ €λ©΄ μμμ΄ νμνλ€)
2. μΈν°νμ΄μ€: μΆμν΄λμ€μ λ¬λ¦¬ `abstract` λ₯Ό μ¬μ©νμ§ μμ. κ΅¬μ±λλ κ²μ νμλ§ λͺμν΄μ(μμ±μλ λ©μλ κ΅¬νμ μμ±ν  νμκ° μλ€.) (νλμ interfaceμ μ¬λ¬ λ°μ΄ν°κ° λ­μΉμ§ μλλ‘ λΆμ°μν¬ μ μκΈ° λλ¬Έμ λ€μ€μμμ΄ κ°λ₯νλ€.)
3. `interface` vs `type` vs `abstract`

```typescript
// μΈν°νμ΄μ€: μμμ΄ κ°λ₯νλ©°, λ€μ€ μμλ κ°λ₯νλ€. λ΄λΆμμ λ©μλ κ΅¬νμ ν  μ μλ€.
interface Test {
	name: string;
	id: number;
	introduce(): void;
}

// μμμ΄ λΆκ°λ₯νλ€. λ΄λΆμμ λ©μλ κ΅¬νμ ν  μ μλ€.
type Test {
	name: string;
	id: number;
	introduce(): void;
}

// ν΄λμ€μ΄κΈ° λλ¬Έμ μμμ κ°λ₯νμ§λ§, λ€μ€ μμμ λΆκ°νλ€. μνλ λ©μλλ κ΅¬νμ ν  μ μλ€.
abstract class Test {
	name: string;
	id: number;
  abstractintroduce(): void;
}
```

4. `T extends number | string` : 2κ° μ΄μ μμμ΄ κ°λ₯ν¨.
5. `interface` νμ© μμ: λ°μ΄ν°λ² μ΄μ€ μ‘°μ(λ‘κ·ΈμΈ, κ²μλ¬Ό, λ±λ±)
6. ORM: SQLλ¬Έμ λμ ν΄μ λ΄κ° μκ³ μλ νλ‘κ·Έλλ° μΈμ΄λ‘ DBλ‘ μ‘°μνλ λ°©λ²(λμ€μ SQLλ¬ΈμΌλ‘ λ³νλλ€)

### β Generic

1. μ μΈν μμ μ νμμ μ¬μ©νλκ²μ΄ μλλΌ μ¬μ© ν  λ λͺ¨λ  νμμ λ§μλλ‘ λ£μ μ μλ€.
2. νμμ μ νμ κ±ΈκΈ° μν΄ `<T extends string | number>` μ²λΌ μ¬μ©ν  μ μλ€.

### β μλ°μ€ν¬λ¦½νΈμ λμ μΈ νμ μμ

1. `true == "true"`: `false` abstract equality composition (νΌμ°μ°μμ `number` μμ°κ³  λΉκ΅νλ€)
2. `010-03=5`, 0λΆμ΄μ 8μ§μκ° λλ€. (16μ§μλ ox, 2μ§μλ ob)
3. `1+'1' = '11'`(`+` λ λ¬Έμμ΄ μ°μ μμ), `11-'1' = 10`(`-` λ `Number`λ§ μ§μνλ€.)
4. `0/0=NaN` , μ«μλ‘ μ·¨κΈνμ§ μλλ€.
5. `1 / 0 > 10 * 1000 = true` : True, infinityλ νν λ²μλ₯Ό λμ΄μλ©΄ μ·¨κΈνλ€
6. `true++=>Error` : κ°μλ€κ° λΆμ΄λκ² μλλΌ λ³μμλ€ μ μΈν΄μΌνλ€.
7. `1+2+"3" = 33`

---

## π 24μΌμ°¨ 11.26.κΈ(μ¨λΌμΈ κ°μ)

μ€λμ `interface`μ `generic`μ λν κ°λμ κ°μλ‘ λ°°μ λ€.

### β Interfaceλ?

1. μΌλ°μ μΌλ‘ λ³μ, ν¨μ, ν΄λμ€μ νμ μ²΄ν¬λ₯Ό μν΄ μ¬μ©λλ€.
2. μ§μ  μΈμ€ν΄μ€λ₯Ό μμ±ν  μ μκ³ , λͺ¨λ  λ©μλκ° μΆμ λ©μλμ΄λ€.
3. μΆμ ν΄λμ€μ μΆμ λ©μλμ λ¬λ¦¬ `abstract` ν€μλλ μ¬μ©ν  μ μλ€.
4. `ES6` λ μΈν°νμ΄μ€λ₯Ό μ§μνμ§ μμ§λ§, `Typescript` λ μΈν°νμ΄μ€λ₯Ό μ§μνλ€.
5. μ μν νλ‘νΌν° κ°μ λλ½νκ±°λ, μ μνμ§ μλ κ°μ μΈμλ‘ μ λ¬νλ©΄ μ»΄νμΌμ μλ¬κ° λ°μνλ€.

### β interfaceλ₯Ό μ¬μ©νλ μ΄μ 

1. νμμ μ΄λ¦μ μ§κ³  μ½λ μμ κ³μ½μ μ μνλ€.
2. νλ‘μ νΈ μΈλΆμμ μ¬μ©νλ μ½λμ κ³μ½μ μ μνλ κ°λ ₯ν λ°©λ²μ΄λ€.

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

### β Properties

1. μ»΄νμΌλ¬λ νλ‘νΌν°μ λ κ°μ§ μμλ₯Ό κ²μ¬νλ€. (νμμμ νλ‘νΌν°μ μ λ¬΄, νλ‘νΌν° νμ)
2. μλ μμ½μ΄λ‘ νλ‘νΌν°λ₯Ό μΈλ°νκ² μ»¨νΈλ‘€ ν  μ μλ€.(?, readonly)

### β Optional Properties

1. νλ‘νΌν° μ μΈ μ μ΄λ¦ λμ `?` λ₯Ό λΆμ¬ νμνλ€.
2. μΈν°νμ΄μ€μ μνμ§ μλ νλ‘νΌν°μ μ¬μ©μ λ°©μ§νλ©΄μ, μ¬μ© κ°λ₯ν νλ‘νΌν°λ₯Ό κΈ°μ ν  λ μ¬μ©νλ€.
3. κ°μ²΄ μμ λͺ κ°μ νλ‘νΌν°λ§ μ±μ ν¨μμ μ λ¬νλ `option bags` κ°μ ν¨ν΄μ μ μ©νλ€.

### β Readonly Properties

1. κ°μ²΄κ° μ²μ μμ±λ  λλ§ κ° μ€μ μ΄ κ°λ₯νκ³ , μ΄ν μμ μ΄ λΆκ°λ₯νλ€.
2. νλ‘νΌν° μ΄λ¦ μμ `readonly` λ₯Ό λΆμ¬ μ¬μ©νλ€.

```typescript
interface Point {
    readonly x: number;
    readonly y: number;
}

let point: Point = { x: 10, y: 20 };
point.x = 5; // Error: Cannot assign to 'x' because it is a read-only property.
```

3. readonly μ const μ κ³΅ν΅μ : μμ± ν λ°°μ΄μ λ³κ²½νμ§ μμμ λ³΄μ₯νλ€. λ³μμλ const, νλ‘νΌν°μλ readonly λ₯Ό μ¬μ©νλ€.

### β interface Type

1. TSμμ μΈν°νμ΄μ€λ ν¨μ, ν΄λμ€μμ μ¬μ©ν  μ μλ€.

```typescript
// function type: ν¨μμ μΈμ νμ, λ°νκ° νμ μ μ
interface CountStar {
    (star: string[]): number;
}

const myStars = ["*", "*", "*"];

const getCountStar: CountStar = (stars) => {
    return stars.length;
};

console.log(getCountStar(myStars));

// class type: ν΄λμ€κ° νΉμ  κ³μ½μ μΆ©μ‘±νλλ‘ λͺμμ μΌλ‘ κ°μ νλ€.
interface Animal {
    makeSound(): void;
}

class Dog implements Animal {
    makeSound(): void {
        console.log("λ©λ©");
    }
}
```

2. μΈν°νμ΄μ€μ ν΄λμ€λ μΈν°νμ΄μ€κ°μ νμ₯μ΄ κ°λ₯νλ€.

```typescript
interface Animal {
    makeSound(): void;
}

interface Dog extends Animal {
    speed: number;
}

class Bulldog implements Dog {
    makeSound(): void {
        console.log("λ©λ©");
    }
}
```

3. hybrid type: JS μ ν΄λ‘μ λ₯Ό TS λ‘ κ΅¬νν λ¬Έλ²

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

### β λμμΈν¨ν΄

1. κ°μ²΄κ° ν  μ μλ νμλ€μ μ λ΅μΌλ‘ λ§λ€μ΄λκ³ , λμ μΌλ‘ νμμ μμ μ΄ νμν κ²½μ° μ λ΅μ λ°κΎΈλ κ²λ§μΌλ‘ μμ μ΄ κ°λ₯νλλ‘ λ§λ  ν¨ν΄μ΄λ€.
2. νλ¨μ μ½λλ₯Ό μ΄ν΄λ³΄λ©΄ λ©μλλ₯Ό μ§μ  λ³κ²½νλκ²μ΄ μλλΌ μλ‘μ΄ `interface` λ₯Ό μμ±νκ³  ν΄λΉ `interface` λ₯Ό μ μ©νλ©΄ `Pay` λ©μλλ₯Ό κ΅¬νν  μ μλ€.

### β μ λ€λ¦­μ΄λ?

1. μ μ  `type` μΈμ΄λ ν΄λμ€λ ν¨μλ₯Ό μ μ ν  λ `type` μ μ μΈν΄μΌ νλ€.
2. `Generic` μ μ½λλ₯Ό μμ±ν  λκ° μλλΌ μ½λκ° μνλ  λ νμμ λͺμνλ€. μ½λλ₯Ό μμ±ν  λ μλ³μλ₯Ό μ¨μ μμ§ μ ν΄μ§μ§ μμ νμμ νμνλ€. (μΌλ°μ μΈ μλ³μλ `T`, `U`, `V` λ₯Ό μ¬μ©νλ€.)

### β μ λ€λ¦­μ μ¬μ©νλ μ΄μ 

1. μ¬ μ¬μ©μ±μ΄ λμ ν¨μμ ν΄λμ€λ₯Ό μμ±ν  μ μλ€.(μ¬λ¬ νμμμ λμκ°λ₯, μ½λμ κ°λμ± ν₯μ)
2. μμμΉ λͺ»ν μ€λ₯λ₯Ό μ½κ² ν¬μ°©νλ€. (`any` : νμμ μ²΄ν¬νμ§ μμ κ΄λ ¨ λ©μλμ ννΈλ₯Ό μ»μ§ λͺ»νλ€. μ»΄νμΌ μ μ»΄νμΌλ¬κ° μ€λ₯λ₯Ό μ°Ύμ§ λͺ»νλ€.)
3. `Generic` μ νμμ μ²΄ν¬ν΄ μ»΄νμΌλ¬κ° μ€λ₯λ₯Ό μ°Ύμ μ μλ€.
4. `any` λ₯Ό μ§μνκ³  λ€μν νμμ μ¬μ©νλ €λ©΄ `Generic` νΉμ `Union` λ¬Έλ²μ κΆμ₯νλ€.

### β GenericμΌλ‘ ν¨μμ ν΄λμ€ λ§λ€κΈ°

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
    // μ λ€λ¦­μ νμ©νμ¬ push()μ pop() λ©μλλ₯Ό κ΅¬νν΄μ£ΌμΈμ.
    push(item: T) {
        this.data.push(item);
    }

    pop(): T | undefined {
        return this.data.pop();
    }
}

const numberQueue = new Queue<number>(); // nunberQueueμμ κ΅¬μ±λ νμμ number νμ΄λ€.

numberQueue.push(0);
console.log(numberQueue.pop());
```

### β Union

1. `|` μ μ¬μ©νμ¬ λ κ° μ΄μμ νμμ μ μΈνλ λ°©μ
2. `union` κ³Ό `generic` μ λͺ¨λ μ¬λ¬ νμμ λ€λ£° μ μλ€. (`union` μ κ³΅ν΅λ λ©μλλ§ μ¬μ©κ°λ₯νλ€, λ¦¬ν΄κ°μ μ μΈλ `union` νμμΌλ‘ μ§μ λλ€.)

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

### β μ μ½μ‘°κ±΄(constraints / keyof)

1. μνμ§ μλ μμ±μ μ κ·Όνλ κ²μ λ§κΈ° μν΄ `Generic` μ μ μ½μ‘°κ±΄μ μ¬μ©νλ€.
2. `Constraints`: νΉμ  νμλ€λ‘λ§ λμνλ `Generic` ν¨μλ₯Ό λ§λ€ λ μ¬μ©νλ€.
3. `Keyof`: λ κ°μ²΄λ₯Ό λΉκ΅ν  λ μ¬μ©νλ€.

```typescript
// constraints: Generic Tμ μ μ½ μ‘°κ±΄μ μ€μ νλ€.(string | number)
// μ μ½ μ‘°κ±΄μ λ²μ΄λλ νμμ μ μΈνλ©΄ μλ¬κ° λ°μνλ€
const printMessage = <T extends string | number>(message: T) => {
    return message;
};

printMessage<number>(1322);
printMessage<string>("hello");
printMessage<boolean>(true); // Error: Type 'boolean' does not satisfy the constraint 'string | number'

// keyof: λ κ°μ²΄λ₯Ό λΉκ΅ν  λ μ¬μ©νλ€.
// Uμ κ°μΈ `not in obj` κ° `T`μ ν€ κ° μ€ μ‘΄μ¬νμ§ μκΈ° λλ¬Έμ μ€λ₯κ° λ°μνλ€.
const printMessage = <T extends object, U extends keyof T>(obj: T, key: U) => {
    return obj[key];
};

console.log(printMessage({ a: 1, b: 2, c: 3 }, "a"));
console.log(printMessage({ a: 1, b: 2, c: 3 }, "not in obj")); // Error: Argument of type '"not in obj"' is not assignable to parameter of type '"a" | "b" | "c"'.
```

### β λμμΈ ν¨ν΄

1. `Factory Pattern`: κ°μ²΄λ₯Ό μμ±νλ μΈν°νμ΄μ€λ§ λ―Έλ¦¬ μ μνκ³  μΈμ€ν΄μ€λ₯Ό λ§λ€ ν΄λμ€μ κ²°μ μ μλΈ ν΄λμ€κ° λ΄λ¦¬λ ν¨ν΄
2. μ¬λ¬κ°μ μλΈ ν΄λμ€λ₯Ό κ°μ§ μνΌ ν΄λμ€κ° μμ λ, μλ ₯μ λ°λΌ νλμ μλΈ ν΄λμ€μ μΈμ€ν΄μ€λ₯Ό λ°ννλ€.

---

## π 25μΌμ°¨ 11.27.ν (μ¨λΌμΈ κ°μ)

μ€λμ `typescript` μ¬ν κ·Έλ¦¬κ³  `decorator`μ λν΄μ λ°°μ λ€. μ§κΈκΉμ§μ νλ‘μ νΈλ₯Ό νλ©΄μ λ§μ΄ μ ν΄λ³΄μ§ μμ λ΄μ©μ΄ μ΄λ ΅κ² λκ»΄μ‘λ€. λμ€μ κΈ°μ΅μ μ λ¨μΌλ €λ©΄ μ€μ μμ λ§μ΄ μ¬μ©ν΄μΌκ² μ§??

### β Union Type, Intersection type

1. κΈ°μ‘΄ νμ, μΈν°νμ΄μ€μ λ³κ²½μ μ΄λ―Έ κ·Έ νμμ μ¬μ©νκ³  μλ μ½λμ λκ°μ λ³κ²½μ κ°ν΄μ€μΌ νλ€. λ§μ½, ν΄λΉ νμμ μ°λ λͺ¨λ  μ½λμ λ³κ²½μ κ°νμ§ μκ³  νΉμ  μ½λλ§ μμ λ‘­κ² νμμ νμ₯νκ³  μΆμ λ μ΄λ»κ² ν΄μΌν κΉ?

```typescript
// Animal μΈν°νμ΄μ€μ λ©μλλ₯Ό μΆκ°νκ² λλ©΄ ν΄λΉ μΈν°νμ΄μ€λ₯Ό implementsνλ λ€λ₯Έ classλ€μλ λμΌν λ©μλλ₯Ό μΆκ°ν΄μΌ νλ€.
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

2. κ·Έλ΄λλ `Intersection(And)`, : Aνμμ΄λ©΄μ Bνμ `Union(Or)` Aνμ, Bνμ λ μ€ νλλ₯Ό μ¬μ©νλ€.

### β Union

1. `|` λΆνΈλ₯Ό μ¬μ©νλ€.

```typescript
// oneμ νμμ stringκ³Ό number λ μ€ νλ
let one: string | number;
```

2. μ¬λ¬ νμ μ€ νλκ° μ¬ κ²μ΄λΌκ³  κ°μ ν  λ μ¬μ©νλ€. λ¨, μΈν°νμ΄μ€μ μ λμ¨ νμμ μ¬μ©νλ κ²½μ° μΈν°νμ΄μ€λ μ λμ¨ νμμ νμ₯νμ§ λͺ»ν¨. μ΄λ΄ λλ `type` κ³Ό `&` λ₯Ό μ¬μ©ν΄μΌ νλ€.

```typescript
// μλ¬ μΌμ΄μ€
type A = string | number;

interface StrOrNum extends A {
    // Error: An interface can only extend an object type or intersection of object types with statically known members.
    a: string;
}

// μ μ μΌμ΄μ€(μ λμ¨ νμμ νμ₯)
type A = { a: string & (string | number) };

interface StrOrNum extends A {
    a: string;
}
```

3. Union Type μ£Όμν  μ : λμμ μ¬λ¬ νμμ΄ λ  μ μλ€.

```typescript
// HumanμΈμ§ DogμΈμ§ νμ ν  μ μμ΄μ μ»΄νμΌ λ¨κ³μμ μλ¬
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

### β Intersection type

1. `&` μ¬μ©
2. `A` νμμ΄λ©΄μ `B` νμμ΄λΌλ μλ―Έ

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

3. `Intersection type` μ κΈ°μ‘΄ νμμ λμ²΄νμ§ μμΌλ©΄μ, κΈ°μ‘΄ νμμ μλ‘μ΄ νλλ₯Ό μΆκ°νκ³  μΆμ λ μ¬μ©νλ€.

```typescript
// Student λ©μλλ₯Ό μΆκ°νκ³  μΆμ λ
// μ 
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

// ν
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

4. κ° νμμ κ²ΉμΉλ νλκ° μλ€λ©΄ μ΄λ¨κΉ?

```typescript
// νμμ΄ κ°μ λ
type Developer = {
    output: string;
    develop: () => void;
};

type Designer = {
    output: string;
    design: () => void;
};

const κ°μμ΄λ: Developer & Designer = {
    output: "λ μ©",
    develop() {
        console.log("I'm working");
    },
    design() {
        console.log("I'm working");
    },
};

// νμμ΄ λ€λ₯Ό λ
type Developer = {
    output: number;
    develop: () => void;
};

type Designer = {
    output: string;
    design: () => void;
};

const λ μ©: Developer & Designer = {
    output: "λ©°μ©", // Error: Type 'string' is not assignable to type 'never'.
    develop() {
        console.log("I'm working");
    },
    design() {
        console.log("I'm working");
    },
};

// νμμ΄ ν¬ν¨κ΄κ³ μΌ λ
type Developer = {
    output: number;
    develop: () => void;
};

type Designer = {
    output: number | string;
    design: () => void;
};

const λ μ©: Developer & Designer = {
    // output : "λ©°μ©",  Error: Type 'string' is not assignable to type 'number'.
    output: 28,
    develop() {
        console.log("I'm working");
    },
    design() {
        console.log("I'm working");
    },
};
```

### β Type Guard

1. λ°μ΄ν°μ νμμ μ μ μκ±°λ, λ  μ μλ νμμ΄ μ¬λ¬ κ°λΌκ³  κ°μ ν  λ μ‘°κ±΄λ¬Έμ ν΅ν΄ λ°μ΄ν°μ νμμ μ’νλκ°λ κ²
2. λ°μ΄ν°μ νμμ λ°λΌ λμνμ¬ μλ¬λ₯Ό μ΅μν ν  μ μμ. νμμ ν΅ν΄ κ°λνλ μ½λ, λ°©μ΄μ μΈ μ½λλ₯Ό μ§€ μ μμ

```typescript
// HumanμΈμ§ DogμΈμ§ νμ ν  μ μμ΄μ μ»΄νμΌ λ¨κ³μμ μλ¬
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

// νμμ€ν¬λ¦½νΈκ° νμμ μΆλ‘ ν  μ μλλ‘ λ¨μλ₯Ό μ€λ³΄λ©΄ μ΄λ¨κΉ
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

3. κ΅¬λ³λ μ λμ¨μΌλ‘ νμ κ°λνλ λ°©λ²: μ‘°κ±΄λ¬Έμ ν΅ν΄ μ΄λ€ νμμΈμ§ μΆλ‘ νλ€.

```typescript
// μλ²μμ μ€λ μλ΅ λλ ν¨μμ κ²°κ³Όκ° μ¬λ¬ κ°λλ‘ λλ  λ μ¬μ©
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

4. `instanceof`: `TS` μμ ν΄λμ€λ νμμ΄λ€. κ°μ²΄κ° μ΄λ€ ν΄λμ€μ κ°μ²΄μΈμ§ κ΅¬λ³ν  λ μ¬μ©νλ μ°μ°μ

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

5. `typeof` : λ°μ΄ν°μ νμμ λ°ννλ μ°μ°μ (`data==null` λλ±μ°μ°μλ₯Ό μ¬μ©νλ©΄ `null`, `undefined` λλ€ μ²΄ν¬νλ€. κ·Έλ¬λ, `null` κ³Ό `undefined` λ λ°λ‘ μ²΄ν¬νλ μ΅κ΄μ κΈ°λ₯΄μ, )

```typescript
const add = (arg?: number) => {
    if (typeof arg === "undefined") {
        return 0;
    }
    return arg + arg;
};
```

6. `in` : μ€λΈμ νΈμ `key`μ€μ λ¬Έμμ΄ `A` κ° μ‘΄μ¬νλμ§ νμΈν  λ

```typescript
// λ¬Έμμ΄ Aλ key(field, property μ΄λ¦)μ μλ―Ένλ€.
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

8. `type-guard` μ μ μ©ν μ€νμμ€

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

### β Optional Chaning

1. μ κ·Όνλ κ°μ²΄μ νλ‘νΌν°κ° `null` λλ `undefined` μΌ μ μλ `optional property` μΈ κ²½μ° `if` λ¬Έμ μ¬μ©νμ§ μκ³  λμ΄κ°κ² νλ μ²΄μ΄λ λ°©λ²
2. `es2020` μμ μΆκ°λ λ¬Έλ²μ΄λ©°, κ°μ²΄κ° `null` λλ `undefined` μ΄λ©΄ `undefined` λ₯Ό λ¦¬ν΄, κ·Έλ μ§ μμ κ²½μ° λ°μ΄ν° κ°μ λ¦¬ν΄
3. `&&` μ `?.` μ μ°¨μ΄μ : `&&` λ `falsy` ν κ° μ²΄ν¬, `?.` λ `null` κ³Ό `undefined` λ§ μ²΄ν¬

```typescript
// κ°μ΄ μμ λλ§ λ°ννλ€.
type Cat = {
	sitDown?: () => void;
}

function trainCat(cat: Cat){
	cat.sitDown?.();
}

// λΆκΈ°μ²λ¦¬ optional Chaining
type Tail = {
	μ΄λμ΄λ: () => void;
}

type Human = {
	call: (dogName: string) => void;
]

type Dog = {
	name: string;
	tail?: Tail;
	μ£ΌμΈ?: Human;
}

function petDog(dog: Dog){
	dog.μ£ΌμΈ?.call(dog.name);
	dog.tail?.μ΄λμ΄λ();
}

// optional chaining refactory
// μ 
function petDog(dog?: Dog) {
  if (dog && dog.tail && dog.tail.μ΄λμ΄λ) {
    dog.tail.μ΄λμ΄λ();
  }
}

// ν
function petDog(dog?: Dog) {
	dog?.tail?.μ΄λμ΄λ?.();
}
```

### β Nullish Coalescing Operator

1. `es2020` μμ μΆκ°λ λ¬Έλ²μ΄λ©°, μ’ν­μ΄ `null`, `undefined` μΈ κ²½μ°μλ§ `B` λ₯Ό λ¦¬ν΄
2. `A ?? B`: `falsy` κ°μ κ·Έλλ‘ λ¦¬ν΄νκ³  μΆμ κ²½μ° μ¬μ©

```typescript
// priceκ° 0μΈ κ²½μ° -1 λ°ν
function getPrice1(product: { price?: number }) {
    return product.price || -1;
}

// priceκ° 0μΈ κ²½μ° 0 λ°ν
function getPrice2(product: { price?: number }) {
    return product.price ?? -1;
}

console.log(0 ?? -1); // 0
console.log(0 || -1); // -1
```

3. falsyν κ°(falseλ‘ νκ°λλ κ°) 0κ³Ό empty string(ββ)μ΄ μ¬ μ μλ λ³μμΒ **`||`**Β λ₯Ό μ°λ©΄ 0, ββλ₯Ό falseλ‘ μΈμνκΈ° λλ¬Έμ μλμΉ λͺ»ν κ²°κ³Όλ₯Ό μ΄λν  μ μμ΅λλ€. μ€λ¬΄μμ ννκ² μ μ§λ₯΄λ μ€μμ΄κΈ°λ ν©λλ€. default κ°μ μ§μ ν΄μ€ λλΒ **`||`**Β μ΄ μλλΌΒ **`??`**μ μ°λ κ²μ κΆμ₯ν©λλ€.

### β Function overloading

1. νλΌλ―Έν°μ νμλ§ λ€λ₯΄κ³  λΉμ·ν μ½λκ° λ°λ³΅λκ³  μλ μν©, μ½λμ μ€λ³΅μ μ€μ΄κ³  μ¬μ¬μ©μ±μ λμΌλ μ¬μ©
2. νλΌλ―Έν°μ ννκ° λ€μν μ¬λ¬ μΌμ΄μ€μ λμνλ κ°μ μ΄λ¦μ κ°μ§ ν¨μλ₯Ό λ§λλ κ², ν¨μμ λ€νμ±μ μ§μνλ κ²
3. ν¨μμ μ΄λ¦μ΄ κ°μμΌνλ€. λ§€κ°λ³μμ μμλ κ°μμΌνλ€. λ°ν νμμ΄ κ°μμΌ νλ€. `function` ν€μλλ‘λ§ κ°λ₯νλ€,
4. ν¨μ μ€λ²λ‘λ©μ νμ μ μΈλΆλ λ°νμμμ μ κ±°λκ³  κ΅¬νλΆλ§ λ¨κΈ°λλ¬Έμ, μ€μ  κ΅¬ν, μ μνλ ν¨μλ νλμ¬μΌλ§ νλ€.

```typescript
// λ§€κ°λ³μκ° κ°μ λ
class User {
    constructor(private id: string) {}

    setId(id: string): void;
    setId(id: number): void;
    setId(id: string | number): void {
        this.id = typeof id === "number" ? id.toString() : id;
    }
}

// λ§€κ°λ³μμ κ°μκ° λ€λ₯Ό λ(μμλ§ μ§μΌμ£Όλ©΄ λλ€.)
class User {
    constructor(private id: string) {}

    setId(id: string): void;
    setId(id: number, radix: number): void;
    setId(id: string | number, radix?: number): void {
        this.id = typeof id === "number" ? id.toString(radix) : id;
    }
}
```

μ λ€λ¦­μ μ¬μ©νλ μμ (μ λ€λ¦­, μΈν°νμ΄μ€, ν΄λμ€ λ±λ±), ν¨μ μ€λ²λ‘λ©μ νμμ μ μΈνλ μμ (ν¨μ, λ©μλ)

### β Type assertion

1. νμμ€ν¬λ¦½νΈκ° μΆλ‘ νμ§ λͺ»νλ νμμ `as keyword` λ₯Ό ν΅ν΄ λͺμν΄μ£Όλ κ²
2. `type casting`: λ°μ΄ν°μ νμμ λ³ν, `type assertion` : λ°μ΄ν°μ νμμ λͺμ

```typescript
let someValue: unknown = "this is a string";

// κΊ½μ κ΄νΈλ react JSXκ° μΈμμ μ λͺ»ν¨.
let strLength: number = (<string>someValue).length;

// asνκ·Έ
let strLength: number = (someValue as string).length;
```

3. νμλ¨μΈ: νμμ€ν¬λ¦½νΈκ° κ°λ°μμ λ§λ§ λ―Ώκ³  `Duck` νμμΌλ‘ μΈμνμ¬ λΉ κ°μ²΄μμλ μλ¬λ₯Ό λ±μ§ μμ
4. νμμ μΈ: κ°μ²΄ νλ‘νΌν°λ₯Ό λͺ¨λ μ±μ°λλ‘ κ°μ νκΈ° λλ¬Έμ μ€μλ₯Ό μ μ§λ₯Ό μνμ΄ λ?μ

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

### β Index Signatrue

1. κ°μ²΄μ νΉμ  `value` μ μ κ·Όν  λ κ·Έ `value` μ `key` λ₯Ό λ¬Έμμ΄λ‘ μΈλ±μ±ν΄ μ°Έμ‘°νλ λ°©λ²
2. κ°μ²΄μ νλ‘νΌν°λ€μ λͺννκ² μ μ μμ λ μ¬μ©νλ€.
3. μ΄λ€ νμμ΄ μ¬μ§ μ μ μλ€λ©΄ μ ννκ² νμμ μ μνλκ²μ΄ μ€μλ₯Ό λ°©μ§ν  μ μλ€.
4. μΈλ±μ€ μκ·Έλμ²λ§ μ¬μ©ν  μ, νμμ νμν΄μ€ λΉ κ°μ²΄μ μλ¬κ° λμ§ μμ΅λλ€.

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

### β Decorator

1. ν¨μκ° ν κ°μ§ μΌλ§νλ©΄μ κ°λμ±μ λμ΄κ³  λ°λ³΅λλ μ½λλ₯Ό μ€μΌ λ μ¬μ©νλ€.
2. ν¨μλ₯Ό κ°μΈλ ν¨μ: κΈ°μ‘΄ ν¨μλ₯Ό λ°κΎΈμ§ μκ³  ν¨μλ₯Ό κ΄μ°°, μμ , μ¬μ μ(μ€λ²λΌμ΄λ©)ν  μ μλ ν¨μ
3. `babel` νλ¬κ·ΈμΈμ μ¬μ©ν΄μ λ°μ½λ μ΄ν° κΈ°λ₯μ μ¬μ©νλ€. `tsconfig.json` μ `experimentDecorator` μ΅μμ `true` λ‘ μ€μ ν΄μ€μΌ νλ€.
4. λ¨μΌμ±μμμΉ νμ ν¨μμ κΈ°λ₯μ νμ₯ν  μ μλ€.
5. `JS` `stage2` μ μλ κΈ°λ₯μ΄λ―λ‘, `TS` μμλ μ€νμ  κΈ°λ₯μΌλ‘μ¨ μ¬μ© κ°λ₯.

### β λ°μ½λ μ΄ν°λ₯Ό μ°κΈ° μ  μμμΌ ν  μλ°μ€ν¬λ¦½νΈ κ°λ

1. μΌκΈκ°μ²΄
2. ν΄λ‘μ : μΈλΆν¨μμ μ€νμ΄ λλλ λ΄λΆν¨μμμ μΈλΆν¨μμ `context` μ μ κ·Όν  μ μλ κ²
3. κ³ μ°¨ν¨μ: ν¨μλ₯Ό νλΌλ―Έν°λ‘ λ°μ λ°ννλ ν¨μ.

### β κ³ μ°¨ ν¨μμ μ©λ

1. μ»€λ§: ν¨μμ λ§€κ°λ³μλ₯Ό λ°λ μμ μ λ¦μΆ λ
2. ν¨μμ μ€ν μμ μ λ―Έλ£° λ(`jest - expect`, `react - onClick`)
3. ν©ν λ¦¬ ν¨μ(μΈμ€ν΄μ€ κ°μ²΄λ ν¨μλ₯Ό μμ±νμ¬ λ°ννλ ν¨μ)λ₯Ό λ§λ€ λ
4. ν, λ°μ½λ μ΄ν°λ₯Ό λ§λ€ λ
5. λ°λ³΅λλ μ½λλ₯Ό μ€μΌ λ
6. ν΄λμ€ λ©μλλ κ³ μ°¨ ν¨μμ νλΌλ―Έν°λ‘μ μ λ¬νμ λ λ©μλλ μΈμ€ν΄μ€μ λν `this` λ°μΈλ©μ μμ΄λ²λ¦°λ€. λ°λΌμ `higher order`ν¨μλ₯Ό νΈμΆν  λ μΈμ€ν΄μ€μ λ©μλλ₯Ό ν¨κ» μΈμλ‘ μ λ¬ν΄μ€μΌ ν¨

### β Decorator Factory

1. λ°μ½λ μ΄ν°λ₯Ό μ¬μ©νλ €λ©΄ `tsconfig.json - experimentalDecorators: true`, `emitDecoratorMetadata: true` `yarn add reflect-metadata` μ€μ 
2. κ³ μ°¨ν¨μ: ν¨μλ₯Ό λ°ννλ ν¨μ
3. ν©ν λ¦¬: μ΄λ€ μΈμ€ν΄μ€λ₯Ό μ¬μ©νμ¬ λ°ννλ ν¨μ, λ©μλ
4. λ°μ½λ μ΄ν° ν©ν λ¦¬: λ°μ½λ μ΄ν° ν¨μλ₯Ό λ°ννλ ν¨μ
5. νΉμ  μΈμλ§ λ°λλ€. μΆκ°μ μΈ μΈμλ₯Ό μ£Όκ³  μΆλ€λ©΄ κ³ μ°¨ν¨μμ λ§€κ°λ³μλ₯Ό μΆκ°νμ¬ λ°μ½λ μ΄ν° ν¨μ λ΄λΆμμ μ¬μ©ν  μ μλ€.

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

// decoratorFacotry ν¨μλ₯Ό μ μΈν΄μ£ΌμΈμ.
function decoratorFactory(value: string) {
    return function (
        target: any,
        propertyKey: string,
        propertyDescriptor: PropertyDescriptor
    ) {
        console.log(value);
    };
}
// string νμμ΄κ³  μ΄λ¦μ΄ valueμΈ λ§€κ°λ³μλ₯Ό λ°μ΅λλ€.
// λ©μλ λ°μ½λ μ΄ν° ν¨μλ₯Ό λ°νν©λλ€.
// λ©μλ λ°μ½λ μ΄ν° ν¨μμ λ§€κ°λ³μ 'target: any, propertyKey: string, propertyDescriptor: PropertyDescriptor'
// λ©μλ decorator ν¨μ λ΄λΆμμ valueλ₯Ό μΆλ ₯ν΄μ£ΌμΈμ.

class ExampleClass {
    @decoratorFactory("λ£°λ£¨λλΌ ν΄κ·Όμ΄λ€")
    static method() {}
}

ExampleClass.method();
```

### β ν΄λμ€ λ°μ½λ μ΄ν°

1. μμ±μ ν¨μλ₯Ό κ΄μ°°, μμ , μ€λ²λΌμ΄λ©(μ¬μ μ) νλ€.
2. κΈ°μ‘΄ ν΄λμ€μ μ½λλ₯Ό λ³κ²½νμ§ μκ³  `property` λ₯Ό μΆκ°νκ±°λ, μμ±μ ν¨μμμ κΈ°λ₯μ μΆκ°νκ³  μΆμ λ μ¬μ©νλ€.
3. ν΄λμ€ μ μΈ μ§μ μ μ μΈλλ€.
4. λ°νμμ ν¨μλ‘μ νΈμΆλλ€. `class` μ `property`λ₯Ό μΆκ°ν΄λ `type system` μμλ μμ§ λͺ» ν¨
5. μμ±μ ν¨μμ μ μ©λλ€.
6. `target` λ§€κ°λ³μλ μμ±μ ν¨μμ΄λ€.
7. `d.ts` νμΌ(νμ μ μΈ νμΌ), `declare class`μλ λ°μ½λ μ΄ν°λ₯Ό μ¬μ©νμ§ λͺ»ν¨(`experimentalDecorators: true`)λ₯Ό ν΄λ μλλ€.

```typescript
declare type ClassDecorator = <TFunction extends Function>(
    target: TFunction
) => TFunction | void;
```

### β method Decorator

1. λ©μλλ₯Ό κ΄μ°°, μμ , μ€λ²λΌμ΄λ© ν  μ μλ€.
2. λ©μλμ `property descriptor` λ₯Ό μμ νκ±°λ κΈ°μ‘΄ λ©μλ μ λ€λ‘ κΈ°λ₯μ μΆκ°νκ³  μΆμ λ μ¬μ©νλ€.

```typescript
import { UserGroup, User, Context } from "./types";

function permission(group: UserGroup) {
    return function (
        target: any,
        propertyKey: string,
        descriptor: PropertyDescriptor
    ) {
        const originFn = descriptor.value;

        // decorator functionμ μμ±ν΄μ£ΌμΈμ.
        descriptor.value = function (this: any, ...args: any[]) {
            // viewerμ groupμ΄ λ§€κ°λ³μμ groupλ³΄λ€ λμ κ²½μ°(κΆνμ΄ μλ κ²½μ°) ν¨μλ₯Ό μ€ννμ§ μκ³  μλ¬λ©μμ§λ₯Ό μΆλ ₯ν΄μ£ΌμΈμ.
            const user = this.context.viewer;
            if (user.group > group) {
                console.log(
                    "permission is denied. viewer group is " + user.group
                );
                return;
            }
            // viewerμ groupμ΄ λ§€κ°λ³μμ group μ΄νμΈ κ²½μ° μλ ν¨μλ₯Ό κ·Έλλ‘ μ€νν΄μ£ΌμΈμ.
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
// "permission is denied. viewer group is 2" μΆλ ₯
userService.deactivateUser(normal);
userService.updateName(normal, "elice");
console.log(normal.name);
```

### β Accessor Decorator

1. μ κ·Όμ(`getter`, `setter`) λ°μ½λ μ΄ν°λ μ κ·Όμλ₯Ό κ΄μ°°, μμ , μ€λ²λΌμ΄λ© ν  μ μλ€.
2. μ κ·Όμμ νλ‘νΌν° μ€λͺμμ μ μ©λλ€. μ λ¬λ°λ λ§€κ°λ³μκ° λ©μλ λ°μ½λ μ΄ν°μ λκ°λ€.(`target`, `propertyKey`, `propertyDescriptor`)
3. `method decorator` μ κ°μ΄ `ES5` λ³΄λ€ λ?μΌλ©΄ `undefined` μ΄ λλ€. λν λ°νκ°λ λ¬΄μλλ€.
4. κ°μ νλ‘νΌν°μ λν μ κ·Όμ `get`, `set` μ€ νλμλ§ λ°μ½λ μ΄ν κ°λ₯

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
        // setter ν¨μλ₯Ό κ΅μ²΄νλ €λ©΄ descriptorμ μ΄λ€ νλ‘νΌν°μ μ μ©ν΄μΌν κΉμ?
        const actualFunction = descriptor.set!; // λλνλ νμμ€ν¬λ¦½νΈμ setν¨μκ° μλ€κ³  κ°μ νλ€. (option )

        const decoratorFunc = function (this: any, value: number) {
            // valueκ° maximumλ³΄λ€ μ»€μ§λ©΄ `exceed the maximum number: ${maximum}`λ₯Ό λ©μμ§λ‘ λ©μμ§λ‘ νλ Errorλ₯Ό throwν΄μ£ΌμΈμ
            if (value > maximum) {
                throw new Error(`exceed the maximum number: ${maximum}`);
            }

            // maximum μ΄νμΌ λλ ν¨μλ₯Ό μ μμ μΌλ‘ μ€νν΄μ£ΌμΈμ
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

### β Property Decorator

1. νλ‘ν°νΌλ₯Ό κ΄μ°°, μμ , μ€λ²λΌμ΄λ© ν  μ μλ€.
2. νλ¬νΌν°μ `property Descriptor` λ₯Ό μμ ν  λ μ¬μ©ν  μ μλ°.
3. νλ‘νΌν° μ μΈ μ§μ μ μ μΈλλ€.
4. μΈμ€ν΄μ€κ° μλ ν΄λμ€ νλ‘ν νμμ νλ‘νΌν°μ μ μ©λλ€.
5. `taget`, `propertyKey` λκ°μ§ μΈμλ₯Ό λ°λλ€.
6. `property Descriptor` λ₯Ό μ¬μ©νμ§ μλμ΄μ : νλ‘νΌν°μ κ²½μ°, μΈμ€ν΄μ€ν λκΈ° μ κΉ μ§ νλ‘νΌν°κ° μ΄κΈ°νλλ κ²μ κ΄μ°°νκ±°λ μμ ν  μ μμ. λλ¬Έμ νλ‘νΌν° λ°μ½λ μ΄ν°λ νλ‘νΌν°κ° `ν΄λμ€` μ μ μΈλμμμ κ΄μ°°νλλ°λ§ μ¬μ©ν  μ μλ€.

```typescript
declare type PropertyDecorator = (
    target: Object,
    propertyKey: string | symbol
) => void | PropertyDecorator;

// νλ‘ν νμ κ³΅μ 
function μνΌκ΅νμ(target: any, propertyKey: string) {
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
    @μνΌκ΅νμ
    public name: string;

    constructor(name: string) {
        this.name = name;
    }
}

const νμ€ν° = new Human("νμ€ν°");
const κ·Έλ = new Human("κ·Έλ");

κ·Έλ.name = "λ―Όμμ¨";
console.log(νμ€ν°.name); // λ―Όμμ¨: μΈμ€ν΄μ€κ° μλ ν΄λμ€ νλ‘ν νμμ νλ‘νΌν°μ μ μ©λκΈ° λλ¬Έμ κ°μ΄ κ³΅μ λλ€.

// νλ‘ν νμ Symbol
function μνΌκ΅νμ(target: any, propertyKey: string) {
    const uniqueKey = Symbol(); // λ§€λ² uniqueκ°μ μμ±

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
    @μνΌκ΅νμ
    public name: string;

    constructor(name: string) {
        this.name = name;
    }
}

const νμ€ν° = new Human("νμ€ν°");
const κ·Έλ = new Human("κ·Έλ");

κ·Έλ.name = "λ―Όμμ¨";
console.log(νμ€ν°.name); // νμ€ν°
```

1. νλ‘νΌν°κ° `null` λλ `undefined` μΌ λ κΈ°λ³Έκ°μ λ°ννλ `Default` λ°μ½λ μ΄ν°λ§λ€κΈ°

```typescript
function Default(initalValue: any) {
    return function (target: any, propertyKey: string) {
        // λ΄λΆ ν¨μμμ μ°μΌ valueλ₯Ό μ μΈν΄μ£ΌμΈμ.
        let value: any;
        // valueμ νμμ anyλ‘ μ€μ ν΄μ£ΌμΈμ

        // getter, setter ν¨μλ₯Ό μμ±ν΄μ£ΌμΈμ
        // getter: valueκ° null λλ undefinedλ©΄ initalValueλ₯Ό λ°νν΄μ£ΌμΈμ
        function getter() {
            return value ?? initalValue;
        }

        // setter: setter ν¨μμ λ§€κ°λ³μ _valueλ₯Ό κ·Έλλ‘ valueμ ν λΉν΄μ£ΌμΈμ
        function setter(_value: any) {
            value = _value; // thisλ₯Ό λΆμ΄μ§ μμλ λ¨.
        }

        // propertyDescriptorλ₯Ό λ°νν΄μ£ΌμΈμ
        // enumerable, configurableμ ν¨κ» μ€μ ν΄μ£ΌμΈμ
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
    @Default(["μ§±μ΄μμ", "λ©μ Έμ"])
    public comments?: any[];
}

const post = new Post();
console.log(post.comments);
```

### β Parameter Decorator

1. ν΄λμ€μ μμ±μ ν¨μ λλ λ©μλ μ μΈ ν¨μμ μ μ©λλ€.
2. λ§€κ°λ³μκ° λ©μλμμ μ μΈλμλ€λ κ²μ κ΄μ°°νλλ°μλ§ μ¬μ© κ°λ₯. κ·Έ μ΄μμ `reflect-metadata` λΌμ΄λΈλ¬λ¦¬λ₯Ό μ¬μ©ν΄μΌ νλ€.
3. λ§€κ°λ³μ μ μΈ μ§μ μ μ¬μ©λλ€.
4. 3κ°μ§ μΈμλ₯Ό λ°λλ€. λ°νκ°μ λ¬΄μλλ€.
5. `reflect-metatdata` λ₯Ό ν΅ν΄ νλΌλ―Έν°μ λν λ©νλ°μ΄ν° μμ§, μ μ₯.
6. λ©μλ λ°μ½λ μ΄ν°λ ν΄λμ€ λ°μ½λ μ΄ν°μ ν¨κ» μ¬μ©ν  μ μμ
7. νλΌλ―Έν° λ°μ½λ μ΄ν° ν¨μμμ λ°ννλ κ°μ λ¬΄μλ©λλ€. (λ°νκ°μ΄ void)
8. νλΌλ―Έν° λ°μ½λ μ΄ν°λ λ©μλμμ λ§€κ°λ³μκ° μ μΈλμλ€λ κ²λ§ μ μ μμ΅λλ€.

```typescript
// targetμ method(any, object), propertyKeyλ λ©μλμ μ΄λ¦(string, symbol), λ§€κ°λ³μμ μΈλ±μ€(μμ)
declare type ParameterDecorator = (
    target: Object,
    propertyKey: string,
    parameterIndex: number
) => void;

function watch(target: Object, propertyKey: string, parameterIndex: number) {
    console.log(
        `λ©μλ μ΄λ¦: ${propertyKey}, λ°μ½λ μ΄ν° μΈλ±μ€: ${parameterIndex}`
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
        // Reflect.getOwnMetadataλ₯Ό μ¬μ©ν΄ λ©νλ°μ΄ν°λ₯Ό κ°μ Έμμ£ΌμΈμ
        const immutableParams: number[] = Reflect.getOwnMetadata(
            immutableKey,
            target,
            propertyName
        );
        // λ©νλ°μ΄ν°μλ paramIndexκ° μ μ₯λμ΄μμ΅λλ€.

        const args = Array.from(arguments as any);
        // μλ°μ€ν¬λ¦½νΈ ν¨μ λ΄λΆμμ μ κ³΅λλ argumentsμμ λ©νλ°μ΄ν°μ paramIndexλ§ νν°λ§ ν΄μ£ΌμΈμ. κ·Έλ° λ€ params λ³μμ ν λΉν΄μ£ΌμΈμ.
        const params = args.filter((val, idx) => immutableParams.includes(idx));

        // params λ°°μ΄μ μννλ©° Object.freezeλ‘ κ°μ²΄λ₯Ό μμ νμ§ λͺ»νκ² λ§μμ£ΌμΈμ.
        // map: λ°°μ΄μ itemμ λ³ννμ¬ λ°°μ΄μ λ°ν
        // forEach: λ°°μ΄μ λ°ννμ§ μκ³  κ° itemμ ν¨μλ₯Ό μ μ©ν  λ
        params.forEach((param) => Object.freeze(param));
        return method.apply(this, arguments);
    };
}
```

### β Decoratorμ λμ

1. μ¬λ¬ κ°μ λ°μ½λ μ΄ν°λ₯Ό ν λ²μ μ°λ κ²(ν©μ± ν¨μ `g(fx))` μ κ°μ λ§€μ»€λμ¦
2. `Reflect.decorate` λ₯Ό μΈ μ μμΌλ©΄ νΈμΆ, μμΌλ©΄ μΈμμ κ°μμ λ°λΌ λ§€κ°λ³μλ₯Ό λ€λ₯΄κ² μ£Όμ΄ λ°μ½λ μ΄ν°λ₯Ό νΈμΆνλ€.(μ΄λ νΈμΆμ μλμμ μλ‘, ν©μ±ν¨μμ λ§€μ»€λμ¦μ²λΌ μμ©νκΈ° λλ¬Έ)

```typescript
// νκ°(μ μΈ): μμμ μλλ‘, log -> timer
// μ μ©(νΈμΆ): μλμμ μλ‘, timer -> log
class Human {
	constructor(){}
	@log()
	@timer()
	hello(name: string){}

	const elice = new Human();
	elice.hello("elice")
}
```

3. μ¬λ¬κ°μ λ°μ½λ μ΄ν°μ μ€ν μμ

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

// μμ: 1 -> 3 -> 4 -> 2
first(): factory evaluated
second(): factory evaluated
second(): called
first(): called
```

---

## π 26μΌμ°¨ 11.30.ν(μ€μκ° κ°μ)

μ€λλΆν°λ `FE`κ° μλ `BE`μ λν΄μ κ°λ΅νκ² λ°°μ΄λ€. μ¬λ¬ νλ μμν¬ μ€ `Node.js`μ λν΄μ λ°°μ°λλ° νλ² μμλ³΄μ. μ€μκ° κ°μ λλ μ£Όλ‘ μ€μ΅μ νλλΌ μ΄λ‘ μ λ§μ΄ λ°°μ°μ§ λͺ»νλ€. λ΄μΌ μ¨λΌμΈ κ°μμμ λ μμΈνκ² μμλ΄μΌκ² λ€.

### β Node.js

1. Chrome V8 javscript μμ§μΌλ‘ λΉλλ `javascript` λ°νμμλλ€.
2. `Node.js`μ λ©μΈμ€λ λλ νλμ΄λ€. `JS`κ° λ¨μΌμ°λ λμΈκ²μ²λΌ `node.js`λ ν λ²μ νμ€μ© μ€ννλ€.
3. `Docker`, `Auto scaling` λ±μ μ΄μ©ν΄ `node.js`μ λ¨μΌ μ€λ λμ λ¨μ μ λ³΄μ ν  μ μλ€.
4. `offLoading`: λ©μΈμ€λ λμ μ΄λ²€νΈ λ£¨νλ μλ‘ μν₯μ λ°μ§ μκ³  κ³μ μ€νλλ€.(μ μμ€μ μ€λ κ±Έλ¦¬λ μΌμ `node.js`μκ², κ³ μμ€μ λ‘μ§μ λ©μΈμ€λ λμμ μ€ννλ€.)
5. `LinkedIn`, `NETFLIX`, `UBER` λ±μμ `node.js`λ₯Ό μ¬μ©νλ€.
6. <a href='https://glitch.com/'>Glich</a> μ¬μ΄νΈλ₯Ό ν΅ν΄ μ¨λΌμΈμμ λ¬΄λ£λ‘ `node.js` νκ²½μ κ΅¬μΆν  μ μλ€.
7. μμ μ `JS`λ νΌν¬λ¨Όμ€κ° κ΅μ₯ν λ¨μ΄μ‘λ€. -> μ΄μν μ½λλ₯Ό μ§μ΄λ£μΌλ©΄ ννμ΄μ§κ° λλ €μ§λ€. -> `firefox - spidermonkey`λ‘ μΈν΄ μ±λ₯μ΄ λ§€μ° μ’μμ‘λ€. > `microsoft - node.js`λ ν΄λΉ νκ²½μ λΈλΌμ°μ κ° μλ λ‘μ»¬νκ²½μμ μλμν€κΈ° μν΄ λ§λ€μλ€.
8. λ°νμ νκ²½: μ»΄ν¨ν°κ° μ€νλλ λμ νλ‘μΈμ€λ νλ‘κ·Έλ¨μ μν μννΈμ¨μ΄ μλΉμ€λ₯Ό μ κ³΅νλ κ°μ λ¨Έμ  μν
9. μ»΄νμΌ μλ¬: νλ‘κ·Έλ¨ λμ μ μ λ°μνλ μλ¬
10. λ°νμ μλ¬: νλ‘κ·Έλ¨μ΄ μ λμνλ€κ° μ€κ°μ λ°μνλ μλ¬
11. `prettier`: κ°λ°μκ° μμ±ν μ½λλ₯Ό ν΅μΌμν€λ λ°©λ²
12. `eslint`: μμν λ¬Έλ²μ μ‘μμ€λ€. μ½λλ₯Ό λΆμνμ¬ λ¬Έλ²μ μΈ μ€λ₯, μν° ν¨ν΄γλ₯΄ μ°Ύμμ€λ€.
13. `npm init`: `package.json` μμ±
14. `npm init`: `package.json` μμ±
15. `npm i eslint --save-dev`: eslint μ€μΉ
16. λΌμ΄λΈλ¬λ¦¬ ESLint μ€μΉ
17. `npm i -g npm`
18. `./node_modules/.bin/eslint --init` : eslint νκ²½μ€μ 
19. `npm i prettier`: νλ¦¬ν°μ΄ μ€μΉ
20. `./node_modules/.bin/prettier filename`
21. `./node_modules/.bin/prettier filename write`
22. `format`: format on save
23. `formatter`: μ΄λ€ λ¬Έλ²κ·μΉμΌλ‘ μ λ¦¬ν μ§ μ ννλ κΈ°λ₯
24. `npm i eslint-plugin-airbnb`: airbnb λ¬Έλ² μ¬μ©

```javascript
const http = require("http"); // http λͺ¨λ νΈμΆ
const port = 9999;

http.createServer((req, res) => {
    res.end("Hello, world!"); // end: λ΄κΈΈλ°μ΄ν° λ€ λ΄κ²ΌμΌλκΉ μμ²­ κΈμλ₯Ό λ³΄λΈλ€.
}).listen(port, () => {
    console.log("μλ²κ° μΌμ‘μ΄μ!!!");
});

// μ΄ν F5 -> node.jsμ€ν
// res.end("<p style='color:red'>gimotti!!!</p>");μ²λΌ innerHTMLμ κ°μ μ½λλ‘λ λ³΄λΌ μ μλ€.
```

25. `commonJS` λ°©μμ `Node.js`μμ μ¬μ©νλ λ°©μμΌλ‘ ES2015 μ λͺ¨λ κ°λμ΄ λμ€κΈ° μ λΆν° μ¬μ©λ¨. κΈ°λ³Έμ `CommonJS` μ΄λ, `package.json`μ μμ νλ©΄ μ¬μ©ν  μ μμ

```javascript
// CommonJS(default)
const http = require("http");

// ES2015, but μ€μ§μ μΈ μ¬μ©μ 2019λλΆν°
import http from "http";
```

26. λμΌν `IPμ£Όμ` μ¬λ ν¬νΈλ²νΈλ₯Ό ν΅ν΄ λ€λ₯΄κ² μ°κ²° ν  μ μλ€.(default: 80)
27. `JS: Express.js` , `TS: Nest.js + Typescript` (ν΄μΈμμ λ§μ΄ μ°μ΄κ³ , κ΅­λ΄μμλ μ€νλ§μ λ§μ΄ μ΄λ€. μ€νλ§μ μ μμ λΆμμ κΆμ₯νλ νλ μμν¬λΌμ λ§μ΄ μ¬μ©λλ€. λ¬λμ»€λΈκ° μλΉν λΉ‘μΈλ€.)
28. docker: μλ²μ λ¬΄μμΈκ°λ₯Ό μ€μΉν  λ μ€λ₯κ° λ°μν¨. μ΄λ° λ¬Έμ λ₯Ό μ€μ΄κΈ° μν΄ λμλ€. μ€μΉκ° μ΄λ―Έ μλ£λ μ»¨νμ΄λλ₯Ό κ°μ§κ³  μλ€. μλΉμ€μ μ¬λ¦¬κΈ°λ§ νλ©΄ λ°λ‘ μ¬μ©κ°λ₯ν¨. λͺ¨λ  κΈ°μ μ νμμ μν΄ λμκΈ° λλ¬Έμ μ κΈ°μ μ μ¬μ©νλμ§μ λν΄ μμλμ.
29. μμ¦ κ°λ°μ μλ²μ νλ‘ νΈλ₯Ό μ»¨νμ΄λ μμ λκ³  κΉνλΈμμ μμ±ν μ½λ μ»€λ° β νμ€νΈ β λΉλ β μλμΌλ‘ μλ²μ μ¬λ¦°λ€. μ΄λ¬ν κ³Όμ μ `CI/CD` λΌκ³  λΆλ₯Έλ€.

### β λ΄μ₯ λͺ¨λ

1. `node.js` λ΄λΆμμ μ κ³΅νλ λͺ¨λ
2. λͺ¨λλͺμ΄ κ°μΌλ©΄ νμ¬ ν΄λλ₯Ό κΈ°μ€μΌλ‘ κ°μ₯ κ°κΉμ΄ λͺ¨λμ λ¨Όμ  κ°μ Έμ¨λ€.
3. `require('fs').readFileSync`: λκΈ°μ μΌλ‘ νμΌμ λΆλ¬μ¨λ€. (μλ¬΄λ° μΈμ½λ©μ νμ§ μμΌλ©΄ `byte` ννλ‘ κ°μ λΆλ¬μ¨λ€. `Buffer`: 16μ§μ νν)

```javascript
const fs = require("fs");
const result = fs.readFileSync("./test");
const buf = Buffer.from([97, 98, 99, 100, 101]);
console.log(buf.compare(result)); // 0: μλ‘ κ°μΌλ©΄ 0μ λ°ν, 1μ΄λ©΄ `buf` κ° λ ν¬κ³ , -1μ΄λ©΄ `result`κ° λ ν¬λ€.

// μλ¬μ²λ¦¬λ try-catchλ¬ΈμΌλ‘ μ€ν
```

4. `node.js` λ°μ΄ν° κ΅¬μ‘°: `stream` : λ°μ΄ν°λ₯Ό μμ μ²­ν¬λ‘ μͺΌκ° μ²λ¦¬νλ€. ν° λ°μ΄ν°λ₯Ό μ²λ¦¬νκ±°λ λΉλκΈ°μ μΌλ‘ μ»μ μ μλ λ°μ΄ν°λ₯Ό μ²λ¦¬ν  λ μ μ©νλ€.

```javascript
const fs = require("fs");
const stream = fs.createReadStream("src/test");
stream.pipe(process.stdout);
```

5. `__filename`, `__dirname`: νμΌ κ²½λ‘, ν΄λ κ²½λ‘ νμνλ λͺλ Ήμ΄

```javascript
console.log("__dirname", __dirname);
cosnole.log("__filename", __filename);
```

6. `dns`: `dns` μ λ³΄μ κ·Ό

```javascript
// family: verson(IPv4, IPv6...)
const dns = require("dns");
dns.lookup("google.com", (err, address, family) => {
    console.log(address, family);
});
```

7. `path`: κ²½λ‘μ€μ 

```javascript
const path = require("path");
const fs = require("fs");

// μ λ κ²½λ‘ λ£κΈ°
const filePath = path.resolve(__dirname, "./test.txt");
const fileContent = fs.readFilSync(filepath, "utf-8");
```

---

## π 27μΌμ°¨ 12.1.μ(μ¨λΌμΈ κ°μ)

μ€λμ 2021λ λ§μ§λ§ ν΄μ μ²« λ μ΄λ€. κ·Έλ  λ°°μ΄ λ΄μ©λ€μ λ³΅μ΅νλ κΈλ 27λ²μ§Έ μ°κ³ μλλ°, 22λ 2μκΉμ§ νλ£¨λ λΉ μ§μμ΄ λ³΅μ΅νλ κΈμ μμ±νμΌλ©΄ μ’κ² λ€. νμμ λ°μ΄λ€μ΄μ λ³Ό μ§κΈμ κΈλ€μ΄ λ°€ν¨μ΄λλ§ λμμ΄ λλ€λ©΄ λμ λͺ©νλ λ¬μ±ν κ²μ΄λ€. κ°μμμλ μ΄μ  μ€μκ° κ°μλ‘ κ°λ΅νκ² λ°°μ λ `node.js`, `express.js`, `module` λ±μ λν΄μ μ‘°κΈ μμΈνκ² λ°°μ λ€.

### β node.jsμ λ±μ₯ λ°°κ²½

1. μΉμ λ°μ μ μν΄ λ±μ₯ν¨. λ¨λ°©ν₯ ν΅μ  μμ£Όμλ `WEB1.0` μμ μ¬μ©μμ μνΈμμ©νλ `WEB2.0` μΌλ‘ λ°μ νκ² λλ©΄μ μΉνμ΄μ§μ λμμ λμ± λ³΅μ‘ν΄μ‘κ³ , λ³΅μ‘ν `JS` λ₯Ό μ€ννκΈ°μν΄ κ³ μ±λ₯μ `JS` μ€νκΈ°κ° νμν΄μ‘λ€. ν¬λ‘¬μμλ μΉλΈλΌμ°μ λ₯Ό μν `V8` μμ§μ λ§λ€κ² λ¨ `V8` μμ§μΌλ‘ μΈν΄ `JS` μλκ° μλΉν λΉ¨λΌμ§κ² λκ³ , `V8` μμ§μ μ΄μ©ν΄μ μΉ λΈλΌμ°μ μμλ§ μ¬μ©νλκ²μ΄ μλ μ΄λ νκ²½μμλ λμμν¬ μ μλλ‘ λ§λ€μ΄μ§κ²μ΄ `node.js` μ΄λ€. μ¦, `js` λ₯Ό μ΄λνκ²½μμλ μ€νν  μ μκ² ν΄μ£Όλ μ€νκΈ°λΌκ³  ν  μ μλ€.
2. λΈλΌμ°μ μμμ `JS`: λΈλΌμ°μ μμ μ€ν, μΉ λ΄λΆ μ νλ λμ, μΉ νλ‘ νΈ κ°λ°μμ μΈμ΄
3. `node.js`: ν¬λ‘μ€ νλ«νΌ μ€ν, μ ν μλ λμ, λ€μν μ΄νλ¦¬μΌμ΄μ κ°λ°, λͺ¨λ  κ°λ°μμ μΈμ΄κ° λμλ€.
4. `FE` : React.js, `BE`: Express.js,(μ΅κ·Ό κ°μ₯ μΈκΈ° μλ μΉμλΉμ€ κ΅¬μ±), `Mobile`: React-native,(νκ°μ§ μ½λλ‘ IOSμ Android κ°λ°), `Desktop-app`: Electron(discord, slack λ± μ±κ°λ°), `Machine-Learning`: Brain.js (JSλ‘ κ΅¬ννλ λ₯λ¬λ)

![](https://images.velog.io/images/abcd8637/post/ad5ca1e3-ba08-42f4-83a8-47bf8ff67d4b/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-01%2009.20.00.png)

### β node.jsμ νΉμ§

1. μ±κΈ μ€λ λ - λΉλκΈ° - μ΄λ²€νΈ κΈ°λ°
2. μ€λ λ: λͺλ Ήμ μ€ννλ λ¨μ, μ±κΈμ€λ λλ ν λ²μ ν κ°μ§ λμλ§ μ€ν κ°λ₯, λ©ν°μ°λ λλ λμμ μ¬λ¬ λμ μν κ°λ₯νλ€.
3. μ₯μ : μ€λ λκ° λμ΄λμ§ μκΈ° λλ¬Έμ λ¦¬μμ€ κ΄λ¦¬μ ν¨μ¨μ 
4. λ¨μ : μ€λ λ κΈ°λ°μ μμλ€μ ν¨μ¨μ΄ λ¨μ΄μ§(CPU μ°μ° μμ)
5. κ·Έλμ `node.js` λ λΉλκΈ° λμμΌλ‘ μ€λ λ κΈ°λ°μ μμμ μ΅μννλ€.
6. λΉλκΈ°: λμμ μ€νν ν μλ£κ° λκΈΈ κΈ°λ€λ¦¬μ§ μλ λ°©μ, λμμ μλ£λ₯Ό κΈ°λ€λ¦¬μ§ μκΈ° λλ¬Έμ λ€λ₯Έ λμμ λ°λ‘ μ€ν κ°λ₯, `node.js` λ μ±κΈ μ€λ λμ΄κΈ° λλ¬Έμ λΉλκΈ° λ°©μμ μ¬μ©ν¨.
7. λ©ν°μ€λ λλ νλ²μ μ¬λ¬κ°μ§ λμμ μννκΈ° λλ¬Έμ λμμ μννκ³  μλ£λ₯Ό κΈ°λ€λ¦¬λ λμ `CPU` λ¦¬μμ€κ° λ­λΉλλ λ°λ©΄, μ±κΈμ€λ λλ νλ²μ μ¬λ¬κ°μ§ λμμ μνν  μ μμ§λ§ λμμ μλ£λ₯Ό κΈ°λ€λ¦¬μ§ μκΈ° λλ¬Έμ `CPU` λ¦¬μμ€λ₯Ό ν¨μ¨μ μΌλ‘ μ¬μ©ν  μ μλ€.
8. μ΄λ²€νΈ κΈ°λ°: λΉλκΈ° λμμ μλ£λ₯Ό μ²λ¦¬νλ λ°©λ². λΉλκΈ° λ°©μμ νΉμ  λμμ μ€νν ν, ν΄λΉ λμμ μ ν μ κ²½μ°μ§ μμ. λμ  ν΄λΉ λμμ΄ μλ£λ  κ²½μ° μ€ν ν  ν¨μλ₯Ό λ―Έλ¦¬ λ±λ‘ν¨. λΉλκΈ° λμμ΄ μλ£λλ©΄ λ―Έλ¦¬ λ±λ‘λ ν¨μλ₯Ό μ€ννλ€.
9. `node.js` λ μ±κΈ μ€λ λκΈ° λλ¬Έμ λΉλκΈ° λμμ΄ νμνκ³  λΉλκΈ° λμμ κ΅¬ννκΈ° μν΄ μ΄λ²€νΈ κΈ°λ°μ λμ λ°©μμ μ¬μ©νλ€.

![](https://images.velog.io/images/abcd8637/post/099e18f8-03f5-482c-a601-06272f907e33/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-01%2009.27.01.png)

### β node.js μμνκΈ°

1. `node.js` λ λΉ λ₯΄κ² κ°λ° μ€μ΄λ―λ‘ λ³΄μ μ΄μ λ° λ²κ·Έ μμ , μ΅μ κΈ°μ μ λΉ λ₯΄κ² μ μ©νλ€. κΈλ³νλ κΈ°μ μ κ°μ₯ μμ μ μΈ μ΅μ  λ²μ μ μ ννλ κ²μ΄ μ΅μ μ΄λ€.
2. `LTS(Long-term support)`: `node.js` μ μμ μ μ΄κ³ , μ€λ μ§μνλ λ²μ  λͺ
3. κ°μ₯ μ΅μ μ κΈ°μ λ³΄λ€ μμ μ μ΄κ³  μ΅μ μ λ²μ μ μ ννμ.

### β ES6

1. `ECMA6` λ²μ  μ΄νλ₯Ό ν΅νμ΄ μΌλ°μ μΌλ‘ `ES6` λΌκ³  λΆλ¦
2. `ECMAScript`: κ³μν΄μ λ°μ ν΄κ°λ `JS` μ νμ€λ¬Έλ², 2015λ `ES6` μ΄ν λ§μ νλμ μΈ λ¬Έλ²μ΄ μΆκ°λ¨
3. `let`, `const`: μμμ λ³μ κ΅¬λΆ κ°λ₯
4. `Template String`: κΈ°μ‘΄μλ μ€ λ°κΏμ `\n` λ₯Ό μ¬μ©νμΌλ `backtick` μ¬μ©μ `\n`μ μ¬μ©νμ§ μμλ λλ€. λ³μλ `${}` μ κ°μ΄ μ¬μ©ν  μ μλ€.
5. `arrow-function`: κΈ°μ‘΄ ν¨μλ `function` μΌλ‘ μ μΈνμΌλ, `()=>{}` μ κ°μ΄ κ°κ²°νκ² νν κ°λ₯νλ€.
6. `class`: κΈ°μ‘΄μλ κ°μ²΄ μ§ν₯μ κ΅¬ννκΈ° μν΄ `function` κ³Ό `prototype` μ μ¬μ©νλ€. `class` λ `function` μΌλ‘ μ μΈνκ³  ν΄λμ€μ λ©€λ²λ λ©μλλ₯Ό κ΅¬νν  λλ `prototype` μ μ¬μ©νλ€. μ΄λ μ§κ΄μ μ΄μ§ μκ³  κ°λμ±μ΄ λ¨μ΄μ‘λ€. `ES6` μμ `class` ννλ‘ κ°μ²΄ μ§ν₯μ μΈ μ½λλ₯Ό μμ±ν  μ μλ€.
7. `destructing`: `Object` μμ κ°μ κΊΌλΌ λ μΌμΌμ΄ μμ±νμ§ μκ³  `{} = obj` μ²λΌ λ³μλ₯Ό κΊΌλΌ μ μλ€.

### β λΉλκΈ° μ½λ©

1. λΉλκΈ°: μ΄λ²€νΈ κΈ°λ° λμμ μ½λλ‘ κ΅¬ννλ λ°©λ²
2. `callback`: μ ν΅μ μΈ `JS` μ μ΄λ²€νΈ κΈ°λ° μ½λ© λ°©μ

```javascript
// callback
// getUsersλ‘ λκΈ°λ ν¨μκ° μ΄λ²€νΈ ν¨μμ΄κ³ , μ΄λ¬ν ννλ₯Ό μ½λ°±μ΄λΌ λΆλ₯Έλ€.
// μΏΌλ¦¬κ° μλ£λλ©΄ μ€λ₯κ° μλμ§, νΉμ μ±κ³΅νλμ§ μ¬λΆλ₯Ό μΈμννλ‘ λ°λλ€.
// μλ¬μ κ²°κ³Όλ₯Ό κ°μ΄ μ λ¬νλ κ²μ΄ νμ€μΌλ‘ μλ¦¬μ‘ν μμ

db.getUsers((err, users) => {
	console.log(users)
});

// callback-hell
// async1, async2, async3...μ λκΈ°μ μΌλ‘ μ€νν΄μΌ νλ κ²½μ°, node.jsλ κΈ°λ³Έμ μΌλ‘ λΉλκΈ° λμμ callbackμΌλ‘ μ²λ¦¬νκΈ° λλ¬Έμ μ½λ°±μ§μ₯ νμμ΄ μΌμ΄λλ€.
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

3. `Promise`: callback μ λ¨μ μ λ³΄μν λΉλκΈ° μ½λ© λ°©μ

```javascript
// promise: ν¨μμ λμμ΄ μλ£λλ©΄ thenμ λ±λ‘λ callbackμ μ€ννλ€. μ€λ₯κ° λ°μν κ²½μ° catchλ¬Έμ callback μ€ν
// promise.chaningμΌλ‘ μ½λλ₯Ό κ°κ²°νκ², short-hand ννμΌλ‘ λμ± κ°κ²°νκ² νν κ°λ₯
db.getUsersPromise()
	.then((users) => {
		return promise1(users);
})
	.then(r1 => promise2(r1))
	.catch(... );

// callbackμ promise ν¨μλ‘ λ³κ²½νκΈ°
// async1 ν¨μμ μ€ν κ²°κ³Όμ λ°λΌ resolve, rejectλ‘ λΆλ¦¬
// rejectλ catchμ λ±λ‘λ callback μ€ν, resolveλ thenμ λ±λ‘λ callback μ€ν
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

4. `Async-await`: `promise` μ λ¨μ μ λ³΄μν λΉλκΈ° μ½λ© λ°©μ, `promise` μ λ€λ₯Έ λ¬Έλ²

```javascript
// async-await: λ¦¬ν΄ κ°μ promise
// await ν promise ν¨μκ° μλ£λ  λκΉμ§ λ€μ λΌμΈμΌλ‘ λμ΄κ°μ§ μμ
// μμ°¨μ  νλ‘κ·Έλλ°μ²λΌ μμ± κ°λ₯νλ€.
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

// errμ²λ¦¬
async function doSomething(msg) => {
	try {
		const r1 = await promise1();
		console.log(r);
	}catch(e){
		console.log(e)
	}
}

// parallel run: promise ν¨μλ₯Ό λμμ μ€νμν€κ³  λ±λ‘λ λͺ¨λ  ν¨μκ° λ§λ¬΄λ¦¬λλ©΄ κ²°κ³Όκ°μ νκΊΌλ²μ λ°ν
// μ΄ 2μ΄μ μκ° μμ
async function parallel(){
	const [r1, r2] = await Promise.all([
		promise1(),
		promise2(),
	]);
	console.log(r1, r2);
}

// μ΄ 3μ΄μ μκ° μμ
async function doSomething() => {
	const r1 = await promise1();
	const r2 = await promise2();
	console.log(r1, r2)
}
```

5. `callback-hell` : `promise chaining` μΌλ‘ ν΄κ²°
6. `promise-hell`: `async-await` μΌλ‘ ν΄κ²°
7. λλΆλΆ κ°λμ±μ΄ μ’μ `async-await` μ μ¬μ©νμ§λ§, μν©μ λ°λΌ `callback`, `promise` λ₯Ό κ΅¬μ¬ν  μ€ μμμΌ νλ€.

### β μ΄λ²€νΈ λ£¨ν

1. μ΄λ²€νΈλ₯Ό μ²λ¦¬νλ λ°λ³΅λλ λμ(loop)
2. `node.js` κ° λΉλκΈ° - μ΄λ²€νΈ λμμ μ²λ¦¬νλ μΌλ ¨μ λ°λ³΅ λμμ΄λ©°, λΉλκΈ° μ½λ©μ΄ μ΄λ€ μμλ‘ μνλλμ§μ λν΄ μ΄ν΄ν  μ μλ€.
3. λΈλΌμ°μ μ `node.js` μ μ΄λ²€νΈ λ£¨νλ κΈ°λ³Έμ μΈ λμλ°©μμ ν° μ°¨μ΄κ° μμ. μ΄λ²€νΈλ£¨νμ κΈ°λ³Έμ μΈ λμ μλ¦¬λ₯Ό μ΄ν΄νλ κ²μ΄ μ€μνλ€.
4. `call stack`: `LIFO` μ€ν, μ΄λ²€νΈ λ£¨νλ μ½μ€νμ΄ λΉμ΄μμ λκΉμ§ μ€νμ ν¨μλ₯Ό μ€ννλ€.
5. `message queue`: `setTimeout` κ°μ μ§μ°μ€ν ν¨μλ₯Ό λ±λ‘νλ `FIFO` ν, μ½μ€νμ΄ λΉμ΄μμ κ²½μ° μ΄λ²€νΈ λ£¨νμ μν΄ λ±λ‘λ ν¨μλ₯Ό μ½ μ€νμ μΆκ°νλ€.(setTimeoutμ μ½μ€νμ΄ λΉμ΄μμ λ μ€ν)
6. `job queue`: `Promise` μ λ±λ‘λ μ½λ°±μ λ±λ‘νλ `FIFO` ν, μμ ν¨μκ° μ’λ£λκΈ° μ μ μ½μ€νμ΄ λΉμ΄μμ§ μλλΌλ μ‘νμ λ±λ‘λ μ½λ°±μ μ½μ€νμ μΆκ°νλ€.(promiseλ μμν¨μκ° μ’λ£λκΈ° μ  μ€ν)

### β npm

1. `npm(node package manager)`: `node.js` νλ‘μ νΈλ₯Ό κ΄λ¦¬νλ νμμ μΈ λκ΅¬(μ¨λΌμΈ μ μ₯μ + μ»€λ§¨λλΌμΈ λκ΅¬)
2. `npm μ μ₯μ`: νμν λΌμ΄λΈλ¬λ¦¬λ λκ΅¬λ₯Ό μμ½κ² κ²μ κ°λ₯. `node.js` μ μΈκΈ°λ‘, κ±°λν μνκ³λ₯Ό λ³΄μ 
3. μ»€λ§¨λλΌμΈ λκ΅¬: νλ‘μ νΈ κ΄λ¦¬λ₯Ό μν λ€μν λͺλ Ήμ΄ μ κ³΅(νλ‘μ νΈ μ€μ  / κ΄λ¦¬, νλ‘μ νΈ μμ‘΄μ± κ΄λ¦¬)
4. `npm init`: ν΄λΉ λλ ν λ¦¬ μμμ `package.json` μ΄λΌλ νμΌμ λ§λ€κ³ , μ΄ λλ ν°λ¦¬λ `node.js` νλ‘μ νΈκ° λλ€.
5. `package.json`: νλ‘μ νΈ κ΄λ ¨ μ λ³΄λ€μ΄ μ μ₯λλ νμΌ. μ΄ νμΌμ μ§μ  μμ νκ±°λ `npm` λͺλ Ήμ΄λ₯Ό μ¬μ©νμ¬ νλ‘μ νΈμ μ λ³΄λ₯Ό μμ ν  μ μμ
6. μμ‘΄μ±: νλ‘μ νΈ λ΄μμ λΌμ΄λΈλ¬λ¦¬λ₯Ό κ΄λ¦¬νλ λ°©λ², νλ‘μ νΈκ° μ€νλκΈ° μν΄ λΌμ΄λΈλ¬λ¦¬μ μμ‘΄νκΈ° λλ¬Έμ μ΄λ¬ν λΌμ΄λΈλ¬λ¦¬λ€μ `dependency(μμ‘΄μ±)` μ΄λΌκ³  λΆλ₯Έλ€.
7. λΌμ΄λΈλ¬λ¦¬: νΉμ  κΈ°λ₯μ μννλ μ½λμ λ¬Άμ, λ³΅μ‘ν κΈ°λ₯μ μ§μ  μμ±νμ§ μκ³ , λ€λ₯Έ μ¬λμ΄ κ΅¬νν κ²μ μ¬μ©νλ λ°©λ²(`node.js` μμλ ν¨ν€μ§λΌκ³ λ λΆλ₯Έλ€.)
8. `npm install`(μ½μ΄ `npm i`): νλ‘μ νΈ μμ‘΄μ± κ΄λ¦¬ κ°λ₯(μμ‘΄μ± μΆκ°, μμ‘΄μ± λ΄λ €λ°κΈ°, κ°λ°μ© μμ‘΄μ± μΆκ°, μ μ­ ν¨ν€μ§ μΆκ°)
9. `npm install [package-name]`: νμν ν¨ν€μ§λ₯Ό νλ‘μ νΈμ μΆκ°νλ€. μΆκ°λ ν¨ν€μ§λ `package.json` μ `dependencies` μμ μΆκ°λλ©°, `node_modules` λλ ν°λ¦¬μ μ μ₯λλ€.
10. `npm install [package-name] --save-dev`: κ°λ°μ© μμ‘΄μ±μ λ°°ν¬ μ κΉμ§λ§ μ¬μ©νλ μμ‘΄μ±(μ λ νμ€νΈ λΌμ΄λΈλ¬λ¦¬ λ±)μΈλ°, `--save-dev` μ΅μμ μ΄μ©νλ©΄ κ°λ°μ© μμ‘΄μ±μ μΆκ°ν  μ μλ€. κ°λ°μ© μμ‘΄μ±μ `package.json-devDependencies` μ μΆκ°λλ€. κΈ°λ³Έμ μΌλ‘ `node_modules` λλ ν°λ¦¬λ μ½λ κ΄λ¦¬λ λ°°ν¬μμ μλ‘λ νμ§ μλλ°, μμ‘΄μ±μ΄ λ§μμ§λ©΄ μ©λμ΄ λλ¬΄ μ»€μ§κ³  μ΄μμ²΄μ λ³λ‘ μ€νλλ μ½λκ° λ€λ₯Έ κ²½μ°κ° μ‘΄μ¬νκΈ° λλ¬Έμ΄λ€.
11. `npm install --production`: νλ‘μ νΈ λ°°ν¬μ κ°λ°μ© μμ‘΄μ±μ ν¬ν¨νμ§ μκ³  λ΄λ €λ°λλ€. `package.json-dependencies` λ§ `node_modules` μ λ΄λ €λ°λλ€.
12. `npm install [package-name]@[version]`: `~1.13.0`: 1.13.xλ²μ  μ€μΉ, `~^1.13.0`: 1.x.x λ²μ  μ€μΉ, κ°μ₯ μΌμͺ½μ 0μ΄ μλ λ²μ μ κ³ μ , `0.13.0`: 0.13.0 λ²μ λ§ μ€μΉ(λ²μ μ΄ λ¬λΌ μ€λ₯κ° λ  λ μ£Όλ‘ μ¬μ©)
13. νλ‘μ νΈμ μμ‘΄μ±μ μΆκ°νλ©΄ `package-lock.json` μ΄λΌλ νμΌμ΄ μμ±λ¨. νλ‘μ νΈμ μμ‘΄μ±μ μΆκ°νλ©΄ μλμΌλ‘ `^`μ΅μ λ²μ μΌλ‘ μΆκ°κ° λλλ°, μμ‘΄μ± λ²μ μ΄ κ°μκΈ° λ³κ²½λμ§ μλλ‘, μ€μΉλ λ²μ μ κ³ μ νλ μ­ν μ νλ€.
14. `npm install [package-name] βglobal`: ν¨ν€μ§λ₯Ό μ μ­ ν¨ν€μ§ λλ ν λ¦¬μ λ΄λ €λ°λλ€. μ»€λ§¨λλΌμΈ λκ΅¬λ€μ μ£Όλ‘ μ μ­ ν¨ν€μ§λ‘ μΆκ°ν΄μ λ°μ(`express-generator,pm2`)
15. λ‘μ»¬ ν¨ν€μ§: `package.json` μ μ μΈλμ΄ μκ³ , `node_modules` μ μ μ₯λ ν¨ν€μ§
16. μ μ­ ν¨ν€μ§: `npm install -g` λ₯Ό ν΅ν΄ λ΄λ €λ°μ, μ μ­ ν¨ν€μ§ μ μ₯μμ μ μ₯λ ν¨ν€μ§
17. μ μ­ ν¨ν€μ§λ νλ‘μ νΈμμ μ¬μ©ν  μ μμΌλ, νλ‘μ νΈμ μμ‘΄μ±μ΄ `package.json` λ΄μ λͺμμ μΌλ‘ μ μΈλμ΄ μλ κ²μ΄ νλ‘μ νΈ κ΄λ¦¬μ μ’μ λ°©ν₯μ΄λ€.
18. `npm remove [package-name]`: μμ‘΄μ± ν¨ν€μ§λ₯Ό μ­μ νλ€. `dependencies`, `devDependencies` μμ μ­μ νκ³  `node_modules` μμλ μ­μ νλ€.
19. `npm run [script-name]` : μ€ν¬λ¦½νΈ(κ°λ¨ν λμμ μννλ μ½λ)λ₯Ό μ€ννλ€.
20. `npm script` : μμ‘΄μ± ν¨ν€μ§λ₯Ό μ¬μ©ν  μ μμ
21. `npm test`: μ½λ μ λνμ€νΈ λ±μ μ¬μ©
22. `npm start`: νλ‘μ νΈ μ€ν
23. `npm stop`: νλ‘μ νΈ μ’λ£
24. `run` μ μ μΈνκ³  μ¬μ©ν  μ μμλΏ, `npm` λ΄λΆμ μΌλ‘ μ½λλ₯Ό μ κ³΅ν΄ μ£Όλκ²μ μλλ€.

### β npx

1. `npm` ν¨ν€μ§λ₯Ό μ€μΉνμ§ μκ³  μ¬μ©ν  μ μκ² ν΄μ£Όλ λκ΅¬, νλ‘μ νΈμ μΆκ°νκ±°λ μ μ­ ν¨ν€μ§λ‘ μΆκ°νμ§ μκ³  `npx` λ₯Ό μ΄μ©νμ¬ λ°λ‘ μ€νν  μ μμ
2. `gist` μ½λλ₯Ό λ€μ΄λ°μ§ μκ³  λ°λ‘ μ€ν κ°λ₯(μ½λλ₯Ό μ νμΈνκ³  μ€νν΄μΌ ν¨)

```javascript
// npm
npm i cowsay -g
cowsay hi

// npx
npx cowsay hi
npx node@12 index.js
```

### β module

1. κ°λ¨ν νλ‘κ·Έλ¨μ΄λΌλ©΄ νμΌ νλλ‘λ κ°λ₯, νλ‘μ νΈκ° μ»€μ§λ©΄ κΈ°λ₯μ λ§κ² μ½λλ₯Ό λΆλ¦¬νλ κ²μ΄ μ€μνλ€. λͺ¨λμ μ½λλ₯Ό λΆλ¦¬νκΈ° μν λ°©λ²
2. λ°λ³΅λλ μ½λλ λͺ¨λλ‘ λΆλ¦¬νμ¬ μ¬μ©(μ¬μ¬μ©μ± μ¦κ°)
3. ν¨ν€μ§λ λͺ¨λμ λͺ¨μ, `npm` ν¨ν€μ§λ€μ λ§μ λͺ¨λμ ν¬ν¨νκ³  μλ μ½λ λͺ¨μ
4. `process`: νμ¬ μ€ννλ‘μΈμ€ κ΄λ ¨ κΈ°λ₯ μ κ³΅(`arch`, `argv`, `env`, `abort`, `kill`, `exit`)
5. `fs`: νμΌ μμΆλ ₯μ νκΈ° μν΄ μ¬μ©(`readFile`, `writeFile`, `watch` λ‘ νμΌ / λλ ν°λ¦¬ λ³κ²½ μ΄λ²€νΈ κ°μ§)
6. `http`: `http` μλ², ν΄λΌμ΄μΈνΈλ₯Ό μν΄ μ¬μ©, `createServer` ν¨μλ‘ μλ² μμ±, `request` ν¨μλ‘ `http` μμ²­ μμ±
7. κΈ°ν κΈ°λ³Έμ κ³΅ λͺ¨λ νμΈνκΈ°: <a href='https://nodejs.org/dist/latest-v14.x/docs/api/'>node.js/doc</a>

### β λͺ¨λμ μμ±κ³Ό μ¬μ©

1. `require` ν¨μλ₯Ό ν΅ν΄ λͺ¨λμ `load` ν  μ μμ
2. μμ‘΄μ± ν¨ν€μ§, μ§μ  μμ±ν λͺ¨λ μ¬μ© κ°λ₯
3. `node.js` μ λͺ¨λμ μ²« `require` μ `cache` , λ λ² μ€ννμ§ μμ
4. λͺ¨λ μ½λλ₯Ό μ¬λ¬ λ² μ€ννκΈ° μν΄μ  ν¨μ λͺ¨λλ‘ μμ±
5. μμ‘΄μ± ν¨ν€μ§λ€μ `require('package-name')` λ‘ `load` κ°λ₯νλ€. ν¨ν€μ§λ₯Ό μ¬μ©νλ €λ©΄ `node_modules` μ λ΄λ €λ°μμ Έ μμ΄μΌ ν¨

```javascript
const name = "elice";
const age = 5;
const nationality = "korea";

// λͺ¨λμ κΈ°λ³Έμ μΈ μ¬μ©λ²
// λͺ¨λμ΄ load λ  λ μ¬μ©λ  κ°μ module.exportsλ‘ λ΄λ³΄λ
module.exports = {
    name,
    age,
    nationality,
};

// λ³μλͺμΌλ‘ export νλ λͺ¨λ μμ±νκΈ°
// λͺ¨λμ objectλ‘ λ§λ€κ³ , κ° key - valueλ₯Ό μ§μ ν΄μ λ΄λ³΄λ
exports.name = name;
exports.age = age;
exports.nationality = nationality;

const student = require("./elice"); // { name: "alice", age: 5, nationality: "korea" }

// ν¨μλ₯Ό exportνλ λͺ¨λ
module.exports = (name, age, nationality) => {
    return {
        name,
        age,
        nationality,
    };
};

// npm ν¨ν€μ§ λͺ¨λ
const dayjs = require("dayjs");
console.log(dayjs());

// μ§μ  μμ±ν λͺ¨λ
const myModule = require("./my-module");
console.log(myModule);

// ν¨μν λͺ¨λ: ν¨μνμ loadν μ¦μ μ€νλμ§ μμ
const myFunctionModule = require("./my-function-module");
console.log(myFunctionModule(name, age, nationality));

// json λͺ¨λ: jsonνμΌλ loadκ°λ₯, objectλ‘ μλνμ±
const myData = require("./my-data");
console.log(myData);
```

### β ES Module

1. ES6μμ λ±μ₯ν JSμ κ³΅μμ μΈ νμ€ λͺ¨λ
2. JSλ κΈ°λ³Έμ μΌλ‘ λͺ¨λμ μ κ³΅νμ§ μμλ€.
3. `node.js` λ λμμ μΈ λ°©μμ ν΅ν΄ λͺ¨λμ μ§μνκ³  μμλ€(common js)
4. ES moduleμ λ±μ₯μΌλ‘ `node.js` μμλ 2κ°μ§ λͺ¨λμ μ§μν΄μΌνλ€.
5. `commonjs` λ `module.exports`, `require` λ‘ λͺ¨λμ μ¬μ©, `ES module` μ `export` μ `import` λ‘ λͺ¨λμ λ§λ€κ³  μ¬μ©
6. νμ¬ `ES Module` μ `node.js` μμ κΈ°λ³Έμ μΌλ‘ μ¬μ©νκΈ°μ μ μ½μ΄ λ§λ€.(νλ‘μ νΈ νμμ `module` λ‘ λ³κ²½, `commonjs` λͺ¨λ `import` μ λ¬Έμ  λ°μ λ±)

### β μΉμ μ΄ν΄

1. μΉ μλΉμ€λ κΈ°λ³Έμ μΌλ‘ `HTTP` μμ²­κ³Ό μλ΅μ λ°λ³΅μΌλ‘ μ΄λ£¨μ΄μ§. `HTTP` μμ²­μ μ¬μ©μκ° μ΄λ€ λ°μ΄ν°κ° νμνμ§λ₯Ό μλ²μκ² μλ¦¬λ μ­ν , `HTTP` μλ΅μ `HTTP` μμ²­μ ν΄λΉνλ μ μ ν λ°μ΄ν°λ₯Ό μ λ¬νλ μ­ν 

![](https://images.velog.io/images/abcd8637/post/8709385a-0f67-4f2c-9cb0-b856268bea83/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-01%2013.54.35.png)

2. μ μ  μΉ(Web 1.0): μ¬μ©μμ μνΈμμ©νμ§ μλ νμ΄μ§ - λ¨λ°©ν₯ ν΅μ , `Link` λ₯Ό ν΅ν νμ΄μ§ μ΄λ μ λλ§ κ°λ₯, μΌλ°μ μΌλ‘ λ³νμ§ μλ `html` νμΌλ‘ μ κ³΅
3. λμ  μΉ(Web 2.0): μ¬μ©μμ μνΈμμ©μ ν¨ - μλ°©ν₯ ν΅μ , κ΅¬κΈ λ§΅, μΉ, μ±ν λ± μ¬μ©μκ° λ€μν κΈ°λ₯μ μνν  μ μμ, `FE` μ `BE` κ° μ κΈ°μ μΌλ‘ ν΅μ νλ©° λμνλ€. νλμ μΈ μΉμ λλΆλΆ λμ  μΉμ΄λ€.
4. `CSR` : νλ‘ νΈμλμμ μ¬μ©μκ° νμ΄μ§μμ λ³΄λ λμ μΈ λΆλΆμ λλΆλΆ μ²λ¦¬νλ λ°©μ(μ¬μ΄νΈκ° λ³νλ λΆλΆμ νλ‘ νΈμλμμ μ²λ¦¬, νμ΄μ§ λ¦¬μμ€λ€μ΄ λ―Έλ¦¬ μ μ, `API` ν΅μ μ΄μ©, `API` νΈμΆμ΄ μλ£λ νμ λ³΄μ¬μ€λ€. λ³΅μ‘ν νλ‘μ νΈ κ΅¬μ±, κ°λ° μ¬μ΄μ¦κ° μ»€μ§λ€.)
5. `SSR`: λ°±μλμμ νμ΄μ§ λλΆλΆμ μμ­μ μ²λ¦¬ν΄μ νλ‘ νΈμλλ‘ μ λ¬νλ λ°©μ(νλ‘ νΈμλλ `HTTP` μλ΅μ λ°μ νλ©΄μ νμ, λ°±μλμμ νμν λ°μ΄ν°κ° ν¬ν¨λ νμ΄μ§λ₯Ό λ§λ€μ΄μ `HTTP` μλ΅μ μ λ¬, λ°±μλμμ `HTML` νμΌμ μμ±ν΄μ νλ‘ νΈλ‘ μ λ¬, μ¬μ΄ κ΅¬μ±, μμ κ°λ°μ¬μ΄μ¦, λ‘λ©μ΄ λλ €λ³΄μ΄κ³ , νμ΄μ§κ° μ΄λνλ©΄ νμ΄μ§κ° κΉλΉ‘μΈλ€.)
6. μΉμλ²λ `HTTP` μμ²­κ³Ό `HTTP` μλ΅μΌλ‘ μ΄λ£¨μ΄μ§λλ° ν΄λΌμ΄μΈνΈλ μλ²λ‘ `HTTP` μμ²­μ λ³΄λ΄κ³ , μλ²λ `HTTP` μλ΅μ λ³΄λΈλ€.

### β μΉ νλ μμν¬

1. μΉ μλΉμ€μ νμν κΈ°λ₯λ€μ μ κ³΅ν΄μ£Όλ λ€μν λκ΅¬λ€μ λͺ¨μ, νμν λΆλΆλ§ μ§μ€ν΄μ κ°λ° ν  μ μμ
2. `HTTP μμ²­`, `HTTP μλ΅`, `λΌμ°ν`, `HTML Templating`
3. λΌμ°ν: `HTTP` μμ²­μ λ°λΌ μλ§μ μλ΅μ λ³΄λ΄μ£Όλ κ²½λ‘λ₯Ό μ€μ νλ μΌ
4. `HTML Templating`: `SSR` μ κ΅¬ννκΈ° μν λ°©λ², `SSR` μμ μλ΅μΌλ‘ λ³΄λΌ `HTML` μ μλ²μμ μμ±νκΈ° μν΄ `HTML Template` λ₯Ό ν΅ν΄ λ―Έλ¦¬ νμ΄μ§μ λΌλλ₯Ό μμ± κ°λ₯
5. `node.js` μ λ€μν μΉ νλ μμν¬: `Express.js`, `Koa.js`, `Nest.js`, `Hapi`, `Sails.js`, `Meteor.js` λ±λ±

### β Express.js μμνκΈ°

1. `node.js` μΉ νλ μμν¬ μ€ κ°μ₯ μ λͺν μΉ νλ μμν¬
2. νμμ λ°λΌ μ μ°νκ² κ΅¬μ‘° μ€μ  κ°λ₯
3. λ€μν λ―Έλ€μ¨μ΄λ₯Ό ν΅ν΄ νμν κΈ°λ₯μ κ°λ¨νκ² μΆκ° κΈ°λ₯
4. λͺ¨λ  λμμ΄ λͺμμ μΌλ‘ κ΅¬μ±λκΈ° λλ¬Έμ, μΉ νλ μμν¬μ λμ λ°©μμ μ΄ν΄νκΈ° κ°μ₯ μ’μ νλ μμν¬
5. `npm init express`
6. `express-generator`: νλ‘μ νΈ μμ±κΈ°, λ¦¬μ‘νΈμ `CRA` μ λΉμ·ν¨

```javascript
// npm μμ
npm i -g express-generator
express my-web
cd my-web
npm i
npm start

// npx μμ
npx express-generator
cd my-web
npm i
npm start
```

### β Express.js κ΅¬μ‘°

![](https://images.velog.io/images/abcd8637/post/0d5266c7-d607-4288-8b5a-0b8863ae3cfe/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-01%2014.21.14.png)

### β Express.js λμλ°©μ

1. `express-generator` λ‘ λ§λ€μ΄μ§ νλ‘μ νΈ λλ ν λ¦¬μ μ κ·Όνμ¬, `npm start` λ‘ `Express.js` νλ‘μ νΈλ₯Ό μ€νν μ μκ³  `[localhost:3000](http://localhost:3000)` μ μ μνμ¬ νμ΄μ§λ₯Ό νμΈν  μ μλ€.

```javascript
1. localhost:3000 μ μ
2. app.js -> app.use('/', indexRouter);
3. routes/index.js -> router.get('/', ...)
4. routes/index.js -> res.render('index', ...)
5. views/index.jade
```

2. app.js: `express()` λ‘ μμ±λλ `app` κ°μ²΄λ₯Ό νμΈν  μ μλ€. `Express.js` μ κΈ°λ₯μ λ΄μ κ°μ²΄
3. λΌμ°ν: `appλΌμ°ν`, `express λΌμ°ν`
4. `path parameter`: μ£Όμμ μΌλΆλ₯Ό λ³μμ²λΌ μ¬μ©ν  μ μλ€.

```js
1. /users/:id - /users/123, /users/456 λ±μΌλ‘ μ μνμ λ λΌμ°ν μ μ©
2. /messges/:from-:to /message/123-456/ λ±μΌλ‘ μ μνμ λ λΌμ°ν μ μ©
```

5. `request handler - request`: λΌμ°νμ μ μ©λλ ν¨μ, `HTTP` μμ²­κ³Ό μλ΅μ λ€λ£° μ μλ ν¨μλ‘, μ€μ λ λΌμ°ν κ²½λ‘μ ν΄λΉνλ μμ²­μ΄ λ€μ΄μ€λ©΄ `Request handler` ν¨μκ° μ€νλ¨

![](https://images.velog.io/images/abcd8637/post/c0917c7f-e341-426f-9d3d-47833c4ec7e5/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-01%2015.02.32.png)

```javascript
// μ€μ λ λΌμ°ν κ²½λ‘μ ν΄λΉνλ μμ²­μ΄ λ€μ΄μ€λ©΄ `request handler` ν¨μλ₯Ό μ€ννλ€.
router.get("/:id", (req, res) => {
    const id = req.params.id;
    res.send(`hello ${id}`);
});
```

6. `resquest-handler - response`: HTTP μλ΅μ μ²λ¦¬νλ κ°μ²΄, HTTP μλ΅μ λ°μ΄ν°λ₯Ό μ μ‘νκ±°λ, μλ΅ μν λ° ν€λλ₯Ό μ€μ ν  μ μμ

![](https://images.velog.io/images/abcd8637/post/491ccb9e-2905-4a01-97df-f766b09f0b0f/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-01%2015.03.04.png)

```javascript
// path parameter
const express = require("express");

const app = express();

app.get("/", (req, res) => {
    res.send("hi");
});

// path parameter μ¬μ©νκΈ°
app.get("/say/:greeting", (req, res) => {
    const { greeting } = req.params;
    res.send(greeting);
});

app.listen(8080);

// router μ°κ²°
const express = require("express");
const userRouter = require("./routes/users");

const app = express();

app.get("/", (req, res) => {
    res.send("OK");
});

/* λΌμ°ν°λ₯Ό '/users' κ²½λ‘μ μ°κ²° */
app.use("/users", userRouter);

app.listen(8080);
```

---

## π 28μΌμ°¨ 12.2.λͺ©(μ€μκ° κ°μ)

λ°μκ² μ΄λ©΄ μκ°μ΄ λΉ¨λ¦¬ κ°λκ²μ²λΌ λκ»΄μ§λ νΉμ§μ΄ μλλ°, μ§κΈμ λ΄κ° κ·Έλ λ€. μμ²­ λ§μ΄ νκ²κ°μ§λ μμλ° λ²μ¨ λͺ©μμΌμ΄λ€. μΌλ₯Έ μλ£νκ³  μ·¨μμ μ μ λ°μ΄λ€κ³  μΆλ€. μ€λμ `npm`, `API`, `RESTAPI`, `express.js`, `middleware`μ κ΄ν λ΄μ©μ λ°°μ λ€.

### β npm

1. `npm init`: `package.json` νμΌ μμ±
2. `package.json`: λͺ¨λμ κ΄λ¦¬νλ νμΌ
3. `package.json - dependencies`: λ΄κ° μ€μΉν λΌμ΄λΈλ¬λ¦¬λ₯Ό λ³΄μ¬μ€λ€. λ²μ  μμ `^`λ λ²μ μ λλ΅μ μΌλ‘ λ³΄μ¬μ€λ€. μλ°μ΄νΈ λΆλΆμμ μμΈνκ² λ€λ£¬λ€.
4. `npm cache clean -f`: μΊμ¬ κ°μ λ‘ λΉμ°κΈ°
5. `node_modules`: λ΄κ° μ€μΉν λͺ¨λμ μμΈν μ λ³΄(λ΄ μ»΄ν¨ν° - programfilesλΌκ³  μκ°νλ©΄ νΈνλ€.)
6. λ€λ₯Έ κ°λ°μλ€κ³Ό νμν λλ `package.json`μ μλ λͺ¨λμ λ²μ λ§κ³  `package-lock.json` νμΌμ μλ λͺ¨λμ λ²μ μ μλ €μ€μΌ μλ¬λ₯Ό λ°©μ§ν  μ μλ€. `package.json`μ λ²μ μ΄ λλ΅μ μΌλ‘λ§ λμμλ€.
7. `npm install [package-name] --save-dev`: κ°λ°μ©μΌλ‘ λͺ¨λμ μ€μΉνλ€.
8. `npm install \ yarn install`: `node_modules`κ° μμ λ `package.json` νμΌμ μ°Έκ³ νμ¬ `node_modules`λ₯Ό μ€μΉν΄μ€λ€. (git clone νκ³ λμ μ¬μ©νλ©΄ λλ€.)
9. `npm install --production`: κ°λ°μ© μμ‘΄μ±(`devDependencies`) λͺ¨λμ μ μΈνκ³ , `dependencies`μλ§ μ€μΉνλ€.
10. `sementic versioning`: 0.0.0(μμμλΆν° `major`, `minor`, `patch` μμλ‘ λΆλ₯Έλ€.)
11. `npm update [package-name]`: λ²μ  μμ `^`κ° λΆμ΄μμΌλ©΄ λλ²μ§Έ μλ¦¬μΈ `minor`ν μ΅μ  λ²μ μ μλ°μ΄νΈνλ€. λ²μ  μμ `~`κ° λΆμ΄μμΌλ©΄ μΈλ²μ§Έ μλ¦¬μΈ `patch` λ₯Ό μ΅μ  λ²μ μΌλ‘ μλ°μ΄νΈ νλ€.
12. `npm install -g [package-name]`: κΈλ‘λ²λ‘ λͺ¨λμ μ€μΉνλ€.
13. `yarn add [package-name]`: λͺ¨λ μ€μΉ
14. `yarn add -D [package-name]`: κ°λ°μ© λͺ¨λ μ€μΉ
15. `yarn remove [package-name]`: λͺ¨λ μ κ±°
16. `scripts`: `CLI` λͺλ Ήμ΄ μ€μ 

### β API

1. λ΄μ₯ λΌμ΄λΈλ¬λ¦¬λ‘ μ¬μ©νλ€ μΈλΆμ λ°μ΄ν°λ₯Ό μ μ₯ν΄μ μλ²μ ν΅μ κΈ°κΈ°κ°μ μ λ³΄λ₯Ό μ£Όκ³ λ°λ κ°μ λ§νλ€.
2. `soap`, `rest`: μ λ³΄ κ΅νμ νμ€μ± κ°λ°μ μλ―Ένλλ°, `soap`λ `xml` κΈ°λ°μΌλ‘ `html`μ²λΌ μ½λκ° λ³΅μ‘ν΄μ μ΄λ₯Ό λ³΄μνκΈ° μν΄ λμ¨ κ²μ΄ `rest`λ€. `rest`λ `json` κΈ°λ°μΌλ‘ μ½λκ° κ°κ²°νλ€.
3. `--print=hHbB`: ν€λλ₯Ό ν΅ν΄ λ³΄λΈκ°κ³Ό λ°μ κ°μ λ³΄μ¬μ£Όλ λͺλ Ήμ΄
4. `npm install --save-dev nodemon`: `node.js`μ μ½λκ° λ°λ λλ§λ€ μλμΌλ‘ μλ‘κ³ μΉ¨ν΄μ£Όλ λΌμ΄λΈλ¬λ¦¬, κ°λ°μ©μΌλ‘λ§ μ¬μ©νκ³  λ°°ν¬ν λλ μ¬μ©νμ§ μλ κ²μ κΆμ₯νλ€.
5. `?`: λ§€κ°λ³μ(μΏΌλ¦¬λΌλ¦¬λ `&`λ‘ κ΅¬λΆνλ€.)

```json
http://localhost:9999/routes/is_odd_2?number=13&number3=1
```

6. `RESTAPI`: `API`μ§λ§, μΉμ ν΅ν΄ μνλ μμ²­μ λ³΄λ΄κ³ , κ·Έ μμ²­μ λ°λ κ². `URL`λ‘ μμ²­μ λ³΄λ΄λ©΄ `HTTP` μν μ½λμ ν¨κ» κ²°κ³Όκ°μ λ³΄λΈλ€. μμ²­μ λͺμΈμ λ§μΆμ΄ λ³΄λ΄μΌ `FE`, `BE`κ°μ μνν ν΅μ μ΄ κ°λ₯νλ€. (`swagger`: RESTAPI λͺμΈ μμ± μ¬μ΄νΈ)

```javascript
// GET
1. λ°μ΄ν°λ₯Ό μ½κ±°λ κ²μν λ μ¬μ©νλ λ©μλ (μ±κ³΅μ 200 return)
2. GET μμ²­μ μ½μ λλ§ μ¬μ©, μμ λ  λλ μ¬μ©μ§ μμμΌ νλ€.

// POST
1. μ£Όλ‘ μλ‘μ΄ λ¦¬μμ€λ₯Ό μμ±ν  λ μ¬μ© λ¨(μΌλ°μ μΌλ‘ μ±κ³΅ μ 201return)
2. POSTλ HTMl bodyλ JSONμΌλ‘ μ λ¬ ν¨
```

7. `.dotenv`: ν¨λΆλ‘ λΈμΆν  μ μλ κ°(APIKEY, password λ±)μ `env` ν΄λμ μ μ₯ν΄μ μ¬μ©νλ€. (`gitignore`λ₯Ό κΌ­ μ μ©νμ.)

### β MiddleWare

1. `μλ²`μ `ν΄λΌμ΄μΈνΈ`μ¬μ΄μ μ‘΄μ¬, κ°κΈ° λΆλ¦¬λ 2κ° μ΄μμ νλ‘κ·Έλ¨ μ¬μ΄μμ, λ§€κ°μ­ν μ νκ±°λ μ°ν©μμΌμ£Όλ νλ‘κ·Έλ¨. `next()`λ₯Ό μμ±νμ§ μμΌλ©΄ ν΄λΉ λ―Έλ€μ¨μ΄μμλ§ μ€ννκ³  λ€μ λ―Έλ€μ¨μ΄λ‘ λμ΄κ°μ§ μλλ€.
2. `Express.js`μμ λ―Έλ€μ¨μ΄λ μμ°¨μ μΌλ‘ μ½λλ₯Ό μ€ννλ€.
3. μΈμ¦ννΈμμ `middleware`λ₯Ό μ¬μ©νκ³  μΈμ¦μ΄ λμμΌλ©΄, λ΄ μ£Όλ¬Έ, μ λ¬Όν¨, κ²°μ λ΄μ­ λ±μ λ³΄λλ° μ¬μ© λ  μ μλ€.
4. `html form methods="POST"`λ‘ μ€μ νλ©΄ `URI` λ€μ `?`ννλ‘ μΏΌλ¦¬κ°μ΄ λμ΄μ¨λ€

```javascript
// middle wareμ μ μ°¨μ μΈ νλ‘μΈμ€1
app.use('/', (req, res, next) => {
	console.log('middelware 1');
	next();  // nextκ° μμΌλ©΄ λμ΄κ°μ§ μλλ€.
}

app.use('/', (req, res, next) => {
	console.log('middelware 2');
}

// middle wareμ μ μ°¨μ μΈ νλ‘μΈμ€2: middleware2, hello, express
app.use('/', (req, res, next) => {
	console.log('middelware 2');
	res.send("hello, express!');
}

app.use('/', (req, res, next) => {
	console.log('middelware 1');  // μ appμμ nextκ° μκΈ°λλ¬Έμ μ€νλμ§ μλλ€.
}

// middlewareμμ κ°μ λκ²¨μ£ΌκΈ°
app.use('/', (req, res, next) => {
	console.log('middelware 1');
	const requestdAt = new Date();
	req.requestdAt = requestdAt;
	next();
}

app.use('/', (req, res, next) => {
	console.log(req.resquestedAt);  // Date
}

// promise μ¬μ©νκΈ°
app.use('/', (req, res, next) => {
	console.log('middelware 1');
	const fileContent = await fs.promises.readFile(".gitignore");
	req.fileContent = fileContent;
	next();
}

// κ²½λ‘ μ€μ 
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

// ?: μμ κ°μ΄ μμ΄λ λκ³  μμ΄λ λλ€.(option)
app.get('/ab?cd',(req, res) => {
	res.send("Root - GET")
})

// +: μμ κ°μ΄ μ¬λ¬κ°κ° μλ λλ€.
app.get('/ab+cd',(req, res) => {
	res.send("Root - GET")
})

// *: *μλ¦¬μ μλ¬΄λ¬Έμλ μλ λλ€.
app.get('/ab*cd',(req, res) => {
	res.send("Root - GET")
})

// ()?: ()μμ κ°μ λ¬Άμ΄μ μ¬μ©νλ€.
app.get('/a(bc)?cd',(req, res) => {
	res.send("Root - GET")
})

// $: $μμ κ°μ ν¬ν¨ν΄μΌ νλ€
app.get('/abcd$/',(req, res) => {
	res.send("Root - GET")
})

// []: λ°°μ΄ μμ κ°μ΄ λ§€μΉ­λ λ
app.get(['/abc', '/xyz'],(req, res) => {
	res.send("Root - GET")
})

// λΆκΈ°μ²λ¦¬ μ 
app.get('/users',(req, res) => {
	res.send("Root - GET")
})

app.get('/users/:id',(req, res) => {
	res.send("Root - GET")
})

// λΆκΈ° μ²λ¦¬ ν
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

5. μλ¬νΈλ€λ§

```javascript
const user = USERS[value];

if (!user) {
    const err = new Error("User not found");
    err.statusCode = 404;
    throw err;
}

req.user = user;
next();

// expressμμ 4κ°μ μΈμλ₯Ό μ€λ€. error νΈλ€λ§ λ―Έλ€μ¨μ΄λ‘ μΈμ
app.use((err, req, res, next) => {
    res.statusCode = err.statusCode || 500;
    res.send(err.message);
});
```

---

## π 29μΌμ°¨ 12.3.κΈ(μ¨λΌμΈ κ°μ)

μ΄μ μ μ΄μ΄μ `express.js` μ¬μ©λ² κ·Έλ¦¬κ³  `middleware`, `postman`μ μ΄μ©ν `RESTAPI`μ€μ΅μ λ°°μ λ€. μ€μ΅μ νλ©΄μ λλκ±΄ <a href='https://velog.io/@abcd8637/%EC%B5%9C%EC%A2%85%EB%A9%B4%EC%A0%91-SW-%EC%A0%95%EA%B8%80%EC%82%AC%EA%B4%80%ED%95%99%EA%B5%90-%ED%9B%84%EA%B8%B0'>μμ </a>μ μ κΈμ¬κ΄νκ΅ λ©΄μ λ³΄κΈ° μ  κ³Όμ  μνμμ κ²μν `CRUD` κ΅¬ννλ κ³Όμ κ° μμλλ°, `R, U` κΈ°λ₯μ ν΄κ²°νμ§ λͺ»νμλ€. μ΄μ μ κΈ°μ΅μ νΈλΌμ°λ§λ‘ κ°κ³ μμ΄ `CRUD`λ₯Ό μ‘°κΈ ννΌ(?)νκ² λμμ§λ§, μ΄λ²μ μμ ν μ λ³΅νκ² λ€λ μμ§λ‘ κ³΅λΆνλ€. λμ€μ λ°±μλ μμ§λμ΄μ νμν  λ μλ²μ κ΄ν΄ λνλ₯Ό ν  λ λ§μ΄ μ ν΅ν μ λλ‘ μ±μ₯νκ³  μΆλ€.

### β middleWare

1. λ―Έλ€μ¨μ΄λ `Express.js`λμμ ν΅μ¬μ΄λ€. `HTTP` μμ²­κ³Ό μλ΅ μ¬μ΄μμ λ¨κ³λ³ λμμ μνν΄μ£Όλ ν¨μλ₯Ό λ»νλ€.
2. `HTTP` μμ²­μ΄ λ€μ΄μ¨ μκ°λΆν° `express.js` κ° μ€νλλ€. λ―Έλ€μ¨μ΄λ `HTTP` μμ²­κ³Ό μλ΅ κ°μ²΄λ₯Ό μ²λ¦¬νκ±°λ, λ€μ λ―Έλ€μ¨μ΄λ₯Ό μ€ν ν  μ μλ€.(μμ°¨μ μΌλ‘ μ²λ¦¬νλ€.) `HTTP` μλ΅μ΄ λ§λ¬΄λ¦¬ λ λκΉμ§ λ―Έλ€μ¨μ΄ λμ μ¬μ΄ν΄μ΄ μ€νλλ€.
3. `req`, `res`, `next` λ₯Ό κ°μ§ ν¨μλ₯Ό μμ±νλ©΄ ν΄λΉ ν¨μλ λ―Έλ€μ¨μ΄λ₯Ό λμν  μ μλ€.

```javascript
1. req: HTTP μμ²­μ μ²λ¦¬νλ κ°μ²΄
2. res: HTTP μλ΅μ μ²λ¦¬νλ κ°μ²΄
3. next: λ€μ λ―Έλ€μ¨μ΄λ₯Ό μ€ννλ ν¨μ
```

4. `RouteHandler`: λ―Έλ€μ¨μ΄μ ν μ’λ₯, λΌμ°ν ν¨μ(get, post, put, delete λ±)μ μ μ©λ λ―Έλ€μ¨μ΄, μΌλ°μ μΈ λ―Έλ€μ¨μ΄μλ λ€λ₯΄κ² path parameterλ₯Ό μ¬μ©ν  μ μλ€. next ν¨μκ° νΈμΆλμ§ μμΌλ©΄ λ―Έλ€μ¨μ΄ μ¬μ΄ν΄μ΄ λ©μΆκΈ° λλ¬Έμ μ£Όμν κ²

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

5. `middleware`λ μ μ©λλ μμΉμ λ°λΌ μ΄νλ¦¬μΌμ΄μ λ―Έλ€μ¨μ΄, λΌμ°ν° λ―Έλ€μ¨μ΄, μ€λ₯μ²λ¦¬ λ―Έλ€μ¨μ΄λ‘ λΆλ₯κ°λ₯νλ€. νμν λμ λ°©μμ λ°λΌ λ―Έλ€μ¨μ΄λ₯Ό μ μ©ν  μμΉλ₯Ό κ²°μ νλ€.

```javascript
// μ νλ¦¬μΌμ΄μ λ―Έλ€μ¨μ΄
// useλ http method ν¨μλ₯Ό μ¬μ©νμ¬ λ―Έλ€μ¨μ΄λ₯Ό μ°κ²° ν  μ μλ€.
app.use((req, res, next) => {
	console.log(`Request ${req.path}`);
	next();
)

app.use(auth);

app.get('/', (req, res, next) => {
	res.send('Hello express!')
})

// λΌμ°ν° λ―Έλ€μ¨μ΄
// νΉμ κ²½λ‘μ λΌμ°νμλ§ λ―Έλ€μ¨μ΄λ₯Ό μ μ©νκΈ° μν λ°©λ²
router.use(auth);

router.get('/', (req, res, next) => {
	res.send('Hello Router!')
})

app.use((req, res, next) => {
	console.log(`Request ${req.path}`);
	next();
)

app.use('/admin', router)

// λ―Έλ€μ¨μ΄ μλΈμ€ν
// μ¬λ¬κ°μ λ―Έλ€μ¨μ΄λ₯Ό λμμ μ μ©ν  μ μμ. μ£Όλ‘ νκ°μ κ²½λ‘μ νΉμ ν΄μ λ―Έλ€μ¨μ΄λ₯Ό μ μ©νκΈ° μν΄ μ¬μ©
app.use(middleware1, middleware2...);

app.use('/admin', auth, adminRouter);

app.get('/', logger, (req, res, next) => {
	res.send('Hello Router!')
})
```

6. μ€λ₯μ²λ¦¬ λ―Έλ€μ¨μ΄: μΌλ°μ μΌλ‘ κ°μ₯ λ§μ§λ§μ μμΉνλ λ―Έλ€μ¨μ΄, λ€λ₯Έ λ―Έλ€μ¨μ΄μ λ¬λ¦¬ err, req, res, next λ€κ°μ§ μΈμλ₯Ό κ°μ§λ©°, μμ  λ―Έλ€μ¨μ΄μμ next ν¨μμ μΈμκ° μ λ¬λλ©΄ μ€νλ¨

```javascript
// nextμ μΈμλ‘ λκΈ°λ©΄ μ€κ°μ κ±΄λλ°κ³  λ§μ§λ§ μ€λ₯μ²λ¦¬ λ―Έλ€μ¨μ΄κ° μ€νλλ€.
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

7. ν¨μν λ―Έλ€μ¨μ΄: νλμ λ―Έλ€μ¨μ΄λ₯Ό μμ±νκ³ , μλλͺ¨λλ₯Ό μ νν΄μ μ¬μ©νκ³  μΆμ κ²½μ°, λ―Έλ€μ¨μ΄λ₯Ό ν¨μνμΌλ‘ μμ±νμ¬ μ¬μ©νλ€. (μ, API λ³λ‘ μ¬μ©μμ κΆνμ λ€λ₯΄κ² μ ννκ³  μΆμ κ²½μ°)

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

8. μμ½: λ―Έλ€μ¨μ΄λ HTTP μμ²­κ³Ό μλ΅ μ¬μ΄μμ μλνλ ν¨μ, req, res, next λ₯Ό μΈμλ‘ κ°μ§ μ μλ€. app νΉμ router κ°μ²΄μ μ°κ²°ν΄μ μ¬μ©κ°λ₯νλ€. next μ μΈμλ‘ λκΈ°λ©΄ μ€λ₯μ²λ¦¬ λ―Έλ€μ¨μ΄κ° μ€νλλ€. λ―Έλ€μ¨μ΄μ κ°μ μ€μ νκ³  μΆλ€λ©΄ ν¨μν λ―Έλ€μ¨μ΄λ‘ μ€μ νλΌ.

### β REST API

1. `REST` μν€νμ³λ₯Ό μ€μνλ μΉ `API`, `RESTFul` μ΄λΌκ³ λ λΆλ₯Έλ€.
2. `API` : μλΉμ€λ νλ‘κ·Έλ¨κ°μ λ―Έλ¦¬ μ ν΄μ§ κΈ°λ₯μ μ€νν  μ μλλ‘ νλ κ·μ½
3. `REST`: μΉμμ μλ£λ₯Ό μ μ‘νκΈ° μν νν λ°©λ²μ μν€νμ³, κΈ°λ³Έμ μΈ REST κ°μ΄λλ₯Ό λ°λ₯΄λ©΄ μ‘°κΈ λ μ’μ κ΅¬μ‘°μ APIλ₯Ό κ΅¬μ±ν  μ μμ
4. APIμ λμμ `HTTP method + λͺμ¬ν URL` μΌλ‘ ννν¨. `/posts` `url` μ κ²μκΈ μμμ κ°λ¦¬ν¨λ€κ³  ν  λ http method(get, post, put, delete)μ κ²°ν©νμ¬ api λμμ μ μνλ€.
5. `url` ννλ²: μμμ λ³΅μνμΌλ‘ νννκ³  νλμ μμμ μ κ·Όμ λ³΅μν + μμ΄λλ₯Ό ν΅ν΄ νΉμ  μμμ μ κ·Όνλ€. μλ₯Ό λ€μ΄ `/posts` κ° κ²μκΈ μ μ²΄λΌκ³  νλ€λ©΄, `/posts`μ 1λ² κ²μκΈμ΄λΌλ μμμ ννν¨
6. `rest api` λ `url` μ ν΅ν΄ μμμ κ³μΈ΅μ μΌλ‘ νννλ€. `/users/1/posts` λΌλ `URL` μ 1λ² μ μ μ κ²μκΈ μ μ²΄λΌλ μμμ λνλΈλ€
7. restapiλ rest μν€νμ³λ₯Ό μ€μνλ μΉ apiλ₯Ό μλ―Ένλ©°, rest μν€νμ³λ₯Ό μ€μνλ κ°λ¨ν λ°©λ²μΌλ‘ urlμ ν΅ν μμμ νν λ°©λ²κ³Ό http methodλ₯Ό ν΅ν api λμμ μ μ μ λλ§ μ¬μ©ν΄λ νλ₯­ν rest apiλ₯Ό κ΅¬νν  μ μλ€.

### β JSON

1. JSμμ κ°μ²΄λ₯Ό νννλ ννμμΌλ‘ μμνλ€. λ°μ΄ν°λ₯Ό νννλ λ°©λ²μ΄ λ¨μνκ³  μ΄ν΄νκΈ° μ¬μμ λ°μ΄ν°λ₯Ό μ μ‘ν  λ λ§μ΄ μ¬μ©νλ€.
2. μΉ apiλ λ°μ΄ν°λ₯Ό λ¬Έμμ΄λ‘ μ μ‘νλ€. μ΄λ€ κ°μ²΄λ₯Ό μΉ apiλ₯Ό ν΅ν΄ λ¬Έμμ΄λ‘ μ λ¬νκΈ° μν΄ jsonμ μ¬μ©νλ€.
3. `value` μλ μ΄λ€ κ°μ΄λΌλ μ¬μ© λ  μ μλ€.

### β Express.jsλ‘ REST API κ΅¬ννκΈ°

1. κ°λ¨ν λ©λͺ¨μ μμ±, μ­μ , νμΈκΈ°λ₯ api κ΅¬ν
2. express-generatorλ₯Ό μ¬μ©νμ§μκ³  MVCν¨ν΄ κ΅¬ν

### β MVC ν¨ν΄

1. νλ‘μ νΈμ κΈ°λ₯λ€μ μ΄λ»κ² λΆλ¦¬ν μ§μ λν νλμ κ΅¬μ± λ°©λ²
2. model: λ°μ΄ν°μ μ κ·Όνλ κΈ°λ₯, λ°μ΄ν° κ·Έ μμ²΄, λ°μ΄ν°μ μ½κΈ° μ°κΈ°λ `model` μ ν΅ν΄μλ§ νν
3. view: λ°μ΄ν°λ₯Ό νννλκΈ°λ₯, controllerμ μν΄ λ°μ΄ν°λ₯Ό μ λ¬λ°κ³  νλ©΄μ νμνλ κΈ°λ₯
4. controller: modelμ ν΅ν΄ λ°μ΄ν°μ μ κ·Όνμ¬ μ²λ¦¬ κ²°κ³Όλ₯Ό viewμ μ λ¬νλ κΈ°λ₯, λΌμ°ν ν¨μκ° controllerκΈ°λ₯μ μννλ€.
5. `express.js` λ κΈ°λ³Έμ μΌλ‘ `HTTP body` μ μ λ¬λλ `JSON` λ°μ΄ν°λ₯Ό μ²λ¦¬νμ§ λͺ»ν¨. `express` μμ κΈ°λ³Έμ μΌλ‘ μ κ³΅ν΄μ£Όλ `express.json()` λ―Έλ€μ¨μ΄λ₯Ό μ¬μ©ν΄μΌ `JSON` λ°μ΄ν°λ₯Ό μ¬μ©ν  μ μ `a pp.use(express.json())`
6. κ°μ₯ λ§μ§λ§ λ―Έλ€μ¨μ΄λ‘ μ€λ₯ μ²λ¦¬ λ―Έλ€μ¨μ΄λ₯Ό μ μ©νλ©΄ λͺ¨λ  λΌμ°νμ κ³΅ν΅μ μΈ μ€λ₯μ²λ¦¬ λ‘μ§μ μ μ©ν  μ μμ

```javascript
// μ΄μ μ next()μ μΈμλ‘ λκ²¨μ€
app.use((err, req, res, next) => {
    res.status(500);

    res.json({
        result: "fail",
        error: err.message,
    });
});
```

7. λͺ¨λ  λΌμ°νμ΄ μ μ© λ μ΄ν μ¬μ©λλ λ―Έλ€μ¨μ΄λ μ€μ λ κ²½λ‘κ° μλ μμ²­μ μ²λ¦¬νλ Route Handler λ‘ λμνλ€. Express.js λ κΈ°λ³Έμ μΌλ‘ 404 νμ΄μ§λ₯Ό κ°μ§κ³  μμ§λ§, μ§μ  μ²λ¦¬κ° νμν  λ Route Handler λ₯Ό μΆκ°νλ€.

```javascript
app.use((req, use, next) => {
    res.status(404);
    res.send({
        result: "fail",
        error: `Page not found ${req.path}`,
    });
});
```

### β postman

1. API νμ€νΈ λκ΅¬λ‘ HTTP μμ²­μ μμ½κ² μμ±νμ¬ νμ€νΈν΄λ³Ό μ μκ² λμμ μ€λ€.

### β λ―Έλ€μ¨μ΄ μμ±κ³Ό μ¬μ©

μ΄ν μ€μ΅ μ½λ μλ΅

---

## π 30μΌμ°¨ 12.4.ν (μ¨λΌμΈ κ°μ)

μ€λμ `mongoDB`μ `express.js`λ₯Ό μ°λνμ¬ `CRUD`νλ λ²μ λ°°μ λ€. μμ μ `mongoDB`λ₯Ό μ΄μ©νμ¬ μ΅μ  κΈ°μ¬λ₯Ό νλμ λ³΄μ¬μ£Όλ <a href='https://blog.naver.com/abcd8637/222152180429'>μ§κΈ λ΄μ€!</a> νλ‘μ νΈλ₯Ό μ§ννμΌλ, `AWS` λ¬΄λ£ ν°μ΄κΈ°κ°μ΄ λλμ μ·¨μνλ λ°λμ μλ²λ₯Ό λ«μλ€. κ·Έλλ `Robo 3T` νλ‘κ·Έλ¨μΌλ‘ `mongoDB`λ₯Ό μ‘°μνλλ° μ΄λ²μλ <a href='https://www.mongodb.com/ko-kr'>mongoDB</a> ννμ΄μ§μ `cloud` κΈ°λ₯κ³Ό μ°λνλ λ²μ λ°°μ λ€. mongoDB ννμ΄μ§μμ λ€λ£¨λκΉ ν¨μ¬ `UX`κ° μ’μλ€.

### β MongoDB

1. λνμ μΈ `NoSQL`, `Document DB` mongoλ Humongousμμ λ°μ¨ λ§λ‘, μμ²­λκ² ν° DB, λμ©λ λ°μ΄ν°λ₯Ό μ²λ¦¬νκΈ° μ’κ² λ§λ€μ΄μ§
2. `NoSQL` (Not Only SQL): κ΅¬μ‘°νλ μ§μμ΄λ₯Ό μ¬μ©νμ§ μλ λ°μ΄ν°λ² μ΄μ€, μλ£κ°μ κ΄κ³μ μ΄μ μ λμ§ μμ. λ°μ΄ν°λ₯Ό κ΅¬μ‘°ννμ§ μκ³  μ μ°νκ² μ μ₯ν¨
3. `RDB` (Relational Database): κ΄κ³ν λ°μ΄ν° λ² μ΄μ€, μλ£λ€μ κ΄κ³λ₯Ό μ£Όμνκ² λ€λ£Έ, SQL μ§μμ΄λ₯Ό μ¬μ©νκΈ° μν΄ λ°μ΄ν°λ₯Ό κ΅¬μ‘°ν ν΄μΌν¨
4. μ `NoSQL`μ μ¬μ©νλκ°? `SQL`μ μ¬μ©νκΈ° μν΄μλ λ°μ΄ν°λ₯Ό κ΅¬μ‘°ννλ κ²μ΄ νμμ΄λ€.(`DDL`) μ€ν€λ§μ μ μλ λ°μ΄ν°κ° μλλ©΄ μ μ₯ν  μ μλ μ μ½μ΄ λ°λ₯΄λλ°, `NoSQL` μ μ¬μ©νλ©΄ μ¬μ μμ μμ΄ DB λ₯Ό μ¬μ©ν  μ μλ€.(DBν¬κΈ°μ κ΄μ¬νμ§ μκ³  νλ‘μ νΈλ₯Ό λΉ λ₯΄κ² μ§νν  μ μμ)

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

5. NoSQLμ λ€μν μ’λ₯κ° μμ§λ§, λνμ μΌλ‘ μλ£λ₯Ό λ¬Έμλ‘ μ μ₯νλ `DocumentDB` κ° μΌλ°μ , μ΄ μΈμ, `key-value`, `Graph`, `large collection` λ±μ `NoSQL DB` κ° μ‘΄μ¬νλ€.
6. `mongoDB` λ₯Ό μ§μ  μ€μΉνκ±°λ `Cloud` μλΉμ€λ₯Ό μ¬μ©ν  μ μμ. μ§μ  μ€μΉνλ©΄ κ·μ°?κ³  μ΄λ ΅μ§λ§, μνλ λ§νΌ μΌλ§λ μ§ λ°μ΄ν°λ₯Ό μ¬μ©ν  μ μμ. `Cloud` λ₯Ό μ¬μ©νλ©΄ μ½κ³  λΉ λ₯΄κ² μμ κ°λ₯νμ§λ§, μ¬μ©λμ λ°λΌ μκΈμ΄ λΆκ³Όλλ€.
7. μ§μ  μ€μΉνκΈ°: μ§μ  λͺ¨λ  DB κ΄λ ¨ μ€μ μ ν΄μΌνλ€. sharding μ΄λ replication λ±μ μμμ΄ νμν  λ μ΄μμ§μκ³Ό λΈνμ°κ° μκ΅¬λλ€. λ¬΄λ£λ‘ μ κ³΅νλ community version μ μ κ³΅ν¨
8. `mongoDB cloud`: λͺ¨λ  DB κΈ°λ₯μ μΉμμ κ΄λ¦¬ κ°λ₯νλ€. νΉλ³ν λΈνμ°μμ΄ DB μ΄μ© κ°λ₯νκ³  `512MB`κΉμ§λ νμ λ¬΄λ£λ‘ μ¬μ©κ°λ₯
9. `mongoDB compass`: mongoDBμ μ μνμ¬ Database, collection, document λ±μ μκ°ννμ¬ κ΄λ¦¬ν  μ μκ² λμμ£Όλ λκ΅¬, MySQL workbench μ μ μ¬

### β MongoDBμ κΈ°λ³Έ κ°λ

1. `Database`: νλ μ΄μμ `collection` μ κ°μ§ μ μλ μ μ₯μ, `SQL`μμμ `database` μ μ μ¬
2. `Collection`: νλ μ΄μμ `Document`κ° μ μ₯λλ κ³΅κ°. SQL μμμ table κ³Ό μ μ¬νλ€. νμ§λ§, collection μ΄ document μ κ΅¬μ‘°λ₯Ό μ μνμ§ μμ
3. `Document`: `mongoDB` μ μ μ₯λλ μλ£, SQL μμ row μ μ μ¬νμ§λ§, κ΅¬μ‘°μ μ½ μμ΄ μ μ°νκ² μ μ₯ κ°λ₯, JSON κ³Ό μ μ¬ν BSON μ μ¬μ©νμ¬ λ€μν μλ£νμ μ§μνλ€.
4. `document - objectID` : κ° document μ μ μΌν ν€ κ°, SQL μ primary key μ μ μ¬νλ€. νλμ© μ¦κ°νλ κ°μ΄ μλ document λ₯Ό μμ±ν  λ μλμΌλ‘ μμ±λλ κ°(timestamp + random value + auto increament)

### β Mongoose ODM

1. `ODM(Object Data Modeling)`: MongoDBμ collectionμ μ§μ€νμ¬ κ΄λ¦¬νλλ‘ λμμ£Όλ ν¨ν€μ§ Collection μ λͺ¨λΈννμ¬, κ΄λ ¨ κΈ°λ₯λ€μ μ½κ² μ¬μ©ν  μ μλλ‘ λμμ€
2. `MongoDB` λ κΈ°λ³Έ `Node.js` λλΌμ΄λ²λ μ°κ²°μνλ₯Ό κ΄λ¦¬νκΈ° μ΄λ €μ μ΄λ, `Mongoose` λ₯Ό μ¬μ©νλ©΄ κ°λ¨νκ² λ°μ΄ν°λ² μ΄μ€μμ μ°κ²°μνλ₯Ό κ΄λ¦¬ν΄μ€.
3. μ€ν€λ§ κ΄λ¦¬: μ€ν€λ§λ₯Ό μ μνμ§ μκ³  λ°μ΄ν°λ₯Ό μ¬μ©νλ κ²μ NoSQL μ μ₯μ μ΄μ§λ§, λ°μ΄ν° νμμ λ―Έλ¦¬ μ μ ν΄μΌ μ½λ μμ±κ³Ό νλ‘μ νΈ κ΄λ¦¬μ μ μ©ν¨. `Mongoose` λ `Code-level` μμ μ€ν€λ§λ₯Ό μ μνκ³  κ΄λ¦¬ν  μ μκ² ν΄μ€, μ€κ°λ¨κ³μμ μ²΄ν¬ν΄μ£Όκ³  κ΄λ¦¬ν¨
4. `populate`: `mongoDB`λ `join` μ μ κ³΅νμ§ μμ. `join` κ³Ό μ μ¬ν κΈ°λ₯μ μ¬μ©νκΈ° μν΄μ `aggregate` λΌλ λ³΅μ‘ν μΏΌλ¦¬λ₯Ό μ¬μ©νμ§λ§ `Mongoose` μμ `populate` λ₯Ό μ¬μ©νμ¬ κ°λ¨νκ² κ΅¬νν  μ μμ

### β Mongoose ODM μ¬μ©μμ

1. μ€ν€λ§ μ μ β λͺ¨λΈ λ§λ€κΈ° β λ°μ΄ν°λ² μ΄μ€ μ°κ²° β λͺ¨λΈ μ¬μ©
2. μ€ν€λ§ μ μ: `Collection` μ μ μ₯λ  `Document` μ μ€ν€λ§λ₯Ό `Code-level` μμ κ΄λ¦¬ν  μ μλλ‘ `schema` λ₯Ό μμ±ν  μ μμ. λ€μν νμμ λ―Έλ¦¬ μ§μ νμ¬ μμ±, μμ  μμ μ λ°μ΄ν° νμμ μ²΄ν¬ν΄μ£Όλ κΈ°λ₯μ μ κ³΅ν¨. `timestamps` μ΅μμ μ¬μ©νλ©΄ μμ±, μμ  μκ°μ μλμΌλ‘ κΈ°λ‘ν΄ μ€

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

3. λͺ¨λΈ λ§λ€κΈ°: μμ±λ μ€ν€λ§λ₯Ό `mongoose` μμ μ¬μ©ν  μ μλ λͺ¨λΈλ‘ λ§λ€μ΄μΌ ν¨. λͺ¨λΈμ μ΄λ¦μ μ§μ νμ¬ `populate` λ±μμ ν΄λΉ μ΄λ¦μΌλ‘ λͺ¨λΈμ νΈμΆ ν  μ μμ

```javascript
const mongoose = require("mongoose");
const PostSchema = require("./schemas/board");
exports.Post = mongoose.model("Post", PostSchema);
```

4. λ°μ΄ν°λ² μ΄μ€ μ°κ²°νκΈ°: `connect` ν¨μλ₯Ό μ΄μ©νμ¬ κ°λ¨νκ² DB μ μ°κ²°ν  μ μμ. `mongoose` λ μλμΌλ‘ μ°κ²°μ κ΄λ¦¬ν΄μ£ΌκΈ° λλ¬Έμ μ§μ  μ°κ²° μνλ₯Ό μ²΄ν¬νμ§ μμλ λͺ¨λΈ μ¬μ© μ μ°κ²° μνλ₯Ό νμΈνμ¬ μ¬μ©μ΄ κ°λ₯ν  λ μμμ μ€ν ν¨

```javascript
const mongoose = require("mongoose");
const { Post } = require("./models");
mongoose.connect("mongodb://localhose:27017/myapp");
```

### β λͺ¨λΈ μ¬μ©νκΈ° - κ°λ¨ν CRUD

![](https://images.velog.io/images/abcd8637/post/5f2948d4-a672-49e9-bcd5-92c2d5ba714d/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-04%2012.09.12.png)

1. `CREATE`: create ν¨μλ₯Ό μ¬μ©νμ¬ Documentμμ±, create ν¨μμλ Document Object λ (λ¨μΌ Document) Document Object μ Array μ λ¬ κ°λ₯(λ³΅μDocument), create λ μμ±λ Document λ₯Ό λ°νν΄μ€

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

2. `FIND(READ)`: find κ΄λ ¨ ν¨μλ₯Ό μ¬μ©νμ¬ document λ₯Ό κ²μ, query λ₯Ό μ¬μ©νμ¬ κ²μνκ±°λ findById λ₯Ό μ¬μ©νλ©΄ objectID λ‘ document λ₯Ό κ²μν  μ μμ

```javascript
const { Post } = require("./models");
async function main() {
    const listPost = await Post.find(query);
    const onePost = await Post.findOne(query);
    const postById = await Post.findById(id);
}
```

3. `query` : MongoDB μλ SQL where μ μ μ¬ν μ‘°κ±΄μ  μ¬μ© κ°λ₯. MongoDB μ query λ BSON νμμΌλ‘ κΈ°λ³Έ λ¬Έλ² κ·Έλλ‘ mongoose μμλ μ¬μ© κ°λ₯, {key: value}λ‘ `exact match`

```javascript
Person.find({
    name: "AYW",
    age: {
        $lt: 20, // less then: λ―Έλ§(and)
        $gte: 10, // grater then equal: μ΄μ(and)
    },
    languages: {
        $in: ["ko", "en"], // in: μ‘΄μ¬νλ©΄(and)
    },
    $or: [
        // or: aciveμ΄κ±°λ trueμΈ κ° μ€ νλ
        { status: "ACTIVE" },
        { isFresh: true },
    ],
});
```

4. `mongoose` λ μΏΌλ¦¬ κ°μΌλ‘ λ°°μ΄λ‘ μ λ¬νλ©΄ μλμΌλ‘ `$in` μΏΌλ¦¬λ₯Ό μμ±ν΄μ€λ€.

```javascript
Person.find({ name: ["elice", "ted"] }); // { name: { $in: ['elice', 'ted' ]}}
```

5. `UPDATE`: update κ΄λ ¨ ν¨μλ₯Ό μ¬μ©νμ¬ document λ₯Ό μμ , find~ ν¨μλ€μ κ²μλ documentλ₯Ό μλ°μ΄νΈλ₯Ό λ°μνμ¬ λ°νν΄μ€λ€. λ°λ©΄, update λ κΈ°λ³Έμ μΌλ‘ $set operator λ₯Ό μ¬μ©νμ¬ document λ₯Ό ν΅μ§Έλ‘ λ³κ²½νμ§ μλλ€.

```javascript
async function main() {
    const updateResult = await Post.updateOne(query, {});
    const updateResults = await Post.updateMany(query, {});
    const postById = await Post.updateOne(query, {});
    const onePost = await Post.findOneAndUpdate(query, {});
}
```

6. `DELETE` : delete κ΄λ ¨ ν¨μλ€μ μ¬μ©νμ¬ document μ­μ κ²°κ³Όλ₯Ό λ¦¬ν΄νλ€. find~ ν¨μλ€μ κ²μλ document λ₯Ό λ°νν΄μ€λ€.

```javascript
async function main() {
    const deleteResult = await Post.deleteOne(query, {});
    const deleteResults = await Post.deleteMany(query, {});
    const onePost = await Post.findOneAndDelete(query, {});
    const postById = await Post.findByIdAndDelete(query, {});
}
```

7. `populate`: document μμ document λ₯Ό λ΄μ§ μκ³  objectID λ₯Ό κ°μ§κ³  reference νμ¬ μ¬μ©ν  μ μλ λ°©λ², document μλ reference λλ ObjectID λ₯Ό λ΄κ³ , μ¬μ©ν  λ populate νμ¬ νμ Document μ²λΌ μ¬μ©ν  μ μκ² ν΄μ€

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

### β Express.js + Mongoose ODM

1. `Express.js` λ νλ‘μ νΈ κ΅¬μ‘°λ₯Ό μμ λ‘­κ² κ΅¬μ±ν  μ μκΈ° λλ¬Έμ μ΄λ λΆλΆμ `Mongoose ODM` μ μμΉμν€λ©΄ μ’μμ§ μ μ ν μμΉλ₯Ό κ²°μ νλ κ²μ΄ μ€μ
2. μΌλ°μ μΌλ‘ `models` λλ ν°λ¦¬μ `Schema` μ `Model` μ κ°μ΄ μμΉμν¨λ€. `app` κ°μ²΄λ μ΄νλ¦¬μΌμ΄μ μμμ μλ―Ένλ λΆλΆμΌλ‘ ν΄λΉ λΆλΆμ λ°μ΄ν°λ² μ΄μ€ μ°κ²°μ λͺμνλ `mongoose.connect` λ₯Ό μμΉνλ€. νΉλ³ν μ μ½μ΄ μλκ²μ μλλ€.

![](https://images.velog.io/images/abcd8637/post/015977e8-b060-4a36-876b-28414b573f3c/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-04%2016.34.38.png)

3. `Express.js` μ΄νλ¦¬μΌμ΄μμ μ’λ£λμ§ μκ³  λμνκΈ° λλ¬Έμ, κ³μν΄μ DB κ° μ μμ μΌλ‘ λμνλμ§ νμνκΈ° μν΄ λμ μ€μ λ°μνλ DB μ°κ²° κ΄λ ¨ μ΄λ²€νΈμ λν μ²λ¦¬λ₯Ό νλ κ²μ΄ μ’μ

```javascript
// connection events
mongoose.connect("----");
mongoose.connection.on("connected", () => {}); // μ°κ²°μλ£
mongoose.connection.on("disconnected", () => {}); // μ°κ²°λκΉ
mongoose.connection.on("reconnected", () => {}); // μ¬μ°κ²° μλ£
mongoose.connection.on("reconnectFailed", () => {}); // μ¬μ°κ²° μλ νμ μ΄κ³Ό
```

### β Sequelize ORM

1. `ORM`(Object-Relational Mapping): `MySQL`, `PostgreSQL` λ±μ `RDBMS` λ₯Ό μ΄μ©νλ κ°λ¨ν λ°©λ² `ODM` μ΄ λ¨μν λͺ¨λΈμ μ§μ€νμ¬ κ΄λ¦¬νλ κ²μ λ°ν΄, `ORM` μ νμ΄λΈ κ΄κ³μ μΏΌλ¦¬ λ±μ κΈ°λ₯μ λμ± λ¨μννλ μ©λλ‘ μ£Όλ‘ μ¬μ©
2. `sequelize` λ μ°κ²°μ κ΄λ¦¬νλ κ°λ¨ν λ°©λ²μ μ κ³΅, `mongoose` κ° `mongoDB` λ§ μ°κ²°μ΄ κ°λ₯νλ°μ λ°ν΄, `sequelize` λ `MySQL`, `PostgreSQL` , `SQLite` λ± λ€μν `RDBMS` μ μ°κ²°κ°λ₯νλ€.
3. λμ€μ `node.js`λ‘ κ΄κ³ν λ°μ΄ν°λ² μ΄μ€λ₯Ό κ΅¬ννκ³  μΆμΌλ©΄ `Sequelize`λ₯Ό κ³΅λΆνμ.

```javascript
// connect db
const sequelize = new Sequelize("database", "usename", "password", {
    host: "localhost",
    dialect: "mysql",
});
```

4. μ€ν€λ§ μμ±: `define` μ ν΅ν΄ `Schema` μμ±, `sequelize` λ `Schema`κ° `DDLλ` μμ±ν΄μ€λ€.

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

5. κ΄κ³ μ μ: νμ΄λΈ κ°μ κ΄κ³λ₯Ό `Code-level` λ‘ κ΄λ¦¬ ν  μ μλ€. μ΄λ₯Ό μ΄μ©νλ©΄ μΈλν€ μ€μ κ³Ό μ μ½μ‘°κ±΄κΉμ§ `DDL` λ‘ μμ±νλ€. λν λ€λλ€ κ΄κ³ μ€μ μ ν΅ν΄ `relation table` λ μλμΌλ‘ μμ±νλ€.

```SQL
User.hasMany(Post);
Post.belongsTo(User);
Foo.belongsToMany(Bar);
Bar.belongsToMany(Foo);
```

6. μΏΌλ¦¬: Operator λ₯Ό μ΄μ©ν΄ SQL μΏΌλ¦¬λ₯Ό μ½λλ‘ μμ± κ°λ₯, μ€ν€λ§μ κ΄κ³ μ€μ μ ν κ²½μ° include λ₯Ό μ¬μ©νμ¬ μλμΌλ‘ join μΏΌλ¦¬ μμ± κ°λ₯

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

7. `Synchronization`: `define`λ model λ°μ΄ν°λ₯Ό λ°νμΌλ‘ DDL μ μλμΌλ‘ μ€νν΄μ€. μ§μ  λ°μ΄ν°λ² μ΄μ€μ μ μνμ¬ νμ΄λΈ μμ± λ° κ΄λ¦¬λ₯Ό ν  νμκ° μμ. μλμΌλ‘ μμ±λ DDL μ λ°λ₯΄μ§ μμΌλ©΄ νμ΄λΈ κ΄λ¦¬κ° μ΄λ €μ μ§

```javascript
sequelize.sync();
```

8. `Sequelize ORM` λ₯Ό μ¬μ©νλ©΄ λ°μ΄ν°λ² μ΄μ€μ μ§μ  DDL μ μ¬μ©νμ§ μκ³ , JS μ½λλ‘ νμ΄λΈ λ° κ΄κ³λ₯Ό κ΄λ¦¬ν  μ μλ€. λν RDB μ μ΄λ €μ΄ μ  μ€ νλμΈ join μ includes μ΅μμ ν΅ν΄ κ°λ¨νκ² μ¬μ©ν  μ μλ€.

---

## π 31μΌμ°¨ 12.7.ν λ°μ΄ν° λ² μ΄μ€ μ°λ(μ€μκ° κ°μ)

μ΄λ²μ£Όλ `node.js`λ₯Ό λ°νμΌλ‘ `mongoDB`λ₯Ό μ΄μ©νμ¬ λ°μ΄ν°λ² μ΄μ€λ₯Ό μ°λνμ¬ νμκ°μκ³Ό λ‘κ·ΈμΈ κΈ°λ₯μ κ΅¬ννλ€. νλ‘ νΈμλλ₯Ό μ€λΉνκ³  μμ΄ `DB`λ₯Ό λ§μ΄ κ³΅λΆνμ§ μμμ§λ§ μ΄λ² κΈ°νλ₯Ό κ³κΈ°λ‘ `DB`μ μΉν΄μ Έλ³΄κ³  κ²μν `CRUD`μ νμ΄μ§λ€μ΄μμ κ΅¬νν΄λ³΄κ³  μΆλ€.

### β DataBase

1. μ¬λ¬ μ¬λμ΄ κ³΅μ νμ¬ μ¬μ© ν  λͺ©μ μΌλ‘ μ²΄κ³ννμ¬ κ΄λ¦¬λλ λ°μ΄ν°μ μ§ν©(`DBMS`μ μν΄ μ μ΄ λ¨)
2. λ°μ΄ν° κ³΅μ : μ¬λ¬λͺμ΄ λμμ κ³΅μ νλλΌλ μμ μ±, μ νμ±μ κ°μΆ€
3. λ°μ΄ν° μ€λ³΅ μ΅μν: νλμ λ°μ΄ν°λ² μ΄μ€μ μ¬λ¬ νμ΄λΈμ λλμ΄ λ°μ΄ν° μ€λ³΅ μ΅μν
4. μ§μμ±: λ°μ΄ν°κ° μ¬λ¬ κ΅°λ°μ μ°μ¬ν΄ μμΌλ©΄ λμμ κ΄λ¦¬νκΈ° μ΄λ ΅κ³ , λ¬΄κ²°μ± μ μ§λ μ΄λ €μ, λ°μ΄ν°λ² μ΄μ€λ `DBMS`μ μν΄ μ€μμ§μ€μ μΌλ‘ κ΄λ¦¬λμ΄ λ¬΄κ²°μ± μ μ§κ° μ©μ΄
5. λ³΄μμ±: μ€μμ§μ€μ μΌλ‘ κ΄λ¦¬λκΈ°μ ν κ΅°λ°λ§ λ³΄μμ μ μ§νλ©΄ λ¨
6. `ACID`: μμμ±(Atomicity) - νΈλμ­μ κ΄λ ¨ μμμ΄ λͺ¨λ μνλλμ§ νμΈ, μΌκ΄μ±(Consistency) - λ°μ΄ν°κ° μΈμ λ μΌκ΄μ± μλ μνμΈμ§ νμΈ, κ³ λ¦½μ±(Isolation) - ν μμ μνμ λ€λ₯Έ μμμ΄ λΌμ΄λ€μ§ λͺ»νκ² λ³΄μ₯, μ§μμ±(Durability) - μ±κ³΅μ μΌλ‘ μνλ μμμ μμν λ°μ μ¦ `ACID`λ λ°μ΄ν°λ² μ΄μ€ νΈλμ μμ΄ μμ νκ² μνλλ€λ κ²μ λ³΄μ₯νκΈ° μν μ±μ§μ΄λ€.
7. `SQL`μ `ACID`κ° μλ λμ  νλ‘κ·Έλ¨μ΄ λ¬΄κ²μ§λ§ μμ νλ€. λ°λλ‘ `NoSQL`μ `ACID`κ° μλ λμ μ νλ‘κ·Έλ¨μ΄ `SQL`λ³΄λ€ κ°λ³κ³  λΉ λ₯΄λ€. λμ  μ΄νλ¦¬μΌμ΄μλ¨μμ λ³΄μμ κ°νμμΌμΌ νλ€.
8. μμ§νμ₯: `SQL`μμ ν μΈμ€ν΄μ€λ₯Ό ν€μ λ ν° λ‘λλ₯Ό κ°λΉνλ€. μ΄λ νκ³κ° μλ€.
9. μννμ₯: `NoSQL`μμ λ λ§μ μΈμ€ν΄μ€λ₯Ό λ§λ€μ΄ λ ν° λ‘λλ₯Ό κ°λΉνλ€. `NoSQL`μ λ°μ΄ν° κ΅¬μ‘°κ° μ ν΄μ Έ μμ§ μμ μΈμ€ν΄μ€λ₯Ό λ¬΄μ ν λλ¦΄ μ μλ€.(μ΄μλΉμ©μ΄ λ°μ³μ€λ€λ©΄..)

### β DBMS

1. Oracle: κ°μ₯ λ¨Όμ  μμμ©μΌλ‘ λ°νλ κ΄κ³ν λ°μ΄ν°λ² μ΄μ€, DBμμ₯ μ μ μ¨ 1μμ§λ§, λΉμ©μ΄ λ§μ΄λ€κ³ , λκΈ°μμμ μ£Όλ‘ μ¬μ©νλ€.
2. MySQL: `MySQL`μ¬μμ λ§λ  μ€νμμ€ λ°μ΄ν°λ² μ΄μ€, `Oracle`μ λΉν΄ λμ©λ λ°μ΄ν° μ²λ¦¬λ μ΄λ €μ
3. PostgreSQL: κ°μ²΄ κ΄κ³ν λ°μ΄ν°λ² μ΄μ€ μμ€ν, μ€νμμ€, λ€μν λ°μ΄ν°λ² μ΄μ€ κ°μ²΄λ₯Ό μ¬μ©μκ° μμ μμ±κ°λ₯
4. MariaDB λ±λ±..
5. μ΄ = νλ = μμ±
6. ν = νν = λ μ½λ

### β NoSQL

1. `key-value`: `Redis`, `AWS DynamoDB`, `value`λ μ΄λ€ κ°μ΄λ  κ°λ₯, κ°μ₯ λ¨μν νν
2. `doucment`: `DynamoDB`, `CouchDB`, κ° λ μ½λκ° νλμ λ¬Έμκ° λ¨, λ¬Έμλ λ°μ΄ν°λ² μ΄μ€μ λ°λΌ `XML`, `YAML`, `JSON`, `BSON` λ±μ μ¬μ©νλ€.
3. `graph-based`: `Neo4j`, `AWS Neptune`, κ·Έλν μ΄λ‘ μ λ°νμΌλ‘ λ°μ΄ν°λ² μ΄μ€λ₯Ό κ·Έλνλ‘ νννλ€. κ΄κ³κΈ°λ°λ¬Έμ μ μ λ¦¬ν¨

### β mongoDB CRUD

```javascript
// create
const users = client.db('fc21').collection('users')
    // delete, users collectionμ ν­μ λΉμμ§
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

### β κ΄κ³ν λ°μ΄ν°λ² μ΄μ€(RDB)

1. κ°μ₯ κ³ μ μ μ΄κ³  λλ¦¬ μλ €μ§ λ°μ΄ν°λ² μ΄μ€ λͺ¨λΈ
2. λ°μ΄ν°μ κ·κ²©μΈ μ€ν€λ§(νμ΄λΈ)μ κ°μ’ μ μ½ μ‘°κ±΄μ μ νκ³ , κ·Έμ λ§κ² λ°μ΄ν° μ μ₯
3. λλΆλΆμ κ²½μ° `SQL`λ‘ μνΈμμ©νλ€.

```SQL
SELECT id, name FROM cities
INSERT INTO users (name, 'cityId') VALUES ('Bobo', 1)
UPDATE users SET name = 'Coco' WHERE name = 'bobo'
DELETE FROM users WHERE name = 'Coco'
```

4. `ORM(Object-relation-mapping)`: κ°μ²΄μ κ΄κ³ν λ°μ΄ν°λ² μ΄μ€μ λ°μ΄ν°λ₯Ό μλμΌλ‘ λ§€νν΄μ£Όλ κ²(JPA, Hibernate λ±)
5. `SQL injection`: μμμ μΈ μ¬μ©μκ° λ³΄μμμ μ·¨μ½μ μ μ΄μ©νμ¬, μμλ‘ `SQL`λ¬Έμ μ£Όμνκ³  μ€ννμ¬ `DB`κ° λΉμ μμ μΈ λμμ νλλ‘ μ‘°μνλ νμ

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
 // SQL injectionμ΄ κ°λ₯ν μ§μ 
 const inserted = `' OR '' = '`

 // λͺ¨λ  row μ­μ 
 const query = `DELETE FROM users WHERE name = '${inserted}'`
 console.log(query)

 // await client.query(query)
 await client.end()

 // prevent SQL injection
 await client.query(`DELETE FROM users WHERE name = $1::text`, [
 userName.userName])
```

6. `Sequelize`: κ°μ²΄μ λ©μλλ₯Ό νμ©νλ κ²μ²λΌ μΏΌλ¦¬ λ‘μ§μ μμ±κ°λ₯, Node.js μ λνμ μΈ ORM, Promise κΈ°λ°μΌλ‘ κ΅¬νλμκΈ° λλ¬Έμ λΉλκΈ° λ‘μ§μ νΈλ¦¬νκ² μμ±ν  μ μλ€.

### β CRUD μ¬μ©μ μΆκ°νκΈ°

1. μΉμ μ±λ₯μ ν¬κΈ°ν΄λ μ¬μ©μκ° νΈλ¦¬νκ² λ λ§λ€μ.
2. λ°μ΄ν°λ₯Ό λ£κ³  μ§μ°λκ²λ³΄λ€ μ μ²΄λ₯Ό μλ‘ κ·Έλ €λ΄λκ²½μ°κ° λΉ λ₯Ό λκ° μλ€.
3. `app.use(express.json())`: req.bodyμ κ°μ λ£μ΄μ€λ€. ()
4. `app.use(express.urlencoded({extended: false}))`: js λ΄λΆ λͺ¨λ μ€ `query-string` λͺ¨λμ΄ μλλ° μ°λ¦¬κ° μ¬μ©νκΈ° νΈνκ² λΆμν΄μ `req.body` μ λ£μ΄μ£Όκ³ . `extended: true` λ₯Ό μ¬μ©νλ©΄ `qs` λͺ¨λμ μ΄μ©ν΄μ `req.body` μ λ£μ΄μ€λ€. (`query-string` μ λΉν΄ λ³΄μμ±μμ λ°μ΄λλ€?μ λμ μ°¨μ΄, λ¨μ μ λ²μ κ΄λ¦¬)
5. POSTλ‘ νκΈ(μ λμ½λ)μ λκΈΈλ λͺλͺ νλ‘μμμ νκΈμ΄ κΉ¨μ§λ κ²½μ°κ° μλ€. (λλΆλΆμ μ§μν¨)
6. κ°λ°μ κ·μ°?λλΌλ λ²μ©μ±μκ² μμ±ν΄μΌνλ€. (μλλ λΈλΌμ°μ λ₯Ό μν΄μ)

---

## π 32μΌμ°¨ 12.8.μ. μ¨λΌμΈ κ°μ

μ€λμ `CRUDλ₯Ό μ΄μ©νμ¬ κ²μν λ§λ€κΈ°`,` Template Engine`, `Pug`, `PM2`μ λ°°μ λ€. `node.js`μ κΈ°λ³ΈμΈμ΄λ `JS`μΈλ°, νκ°μ§μ μΈμ΄λ‘ νλ‘ νΈμ λ°±μ λ€λ£¬λ€κ³  μκ°νλκΉ κ°μ΄μ΄ μμ₯ν΄μ‘λ€. (μμ§μ μ΄μνμ§λ§..) μμ£Ό μ΄ν΄λ³΄λ©° λμ μ΅νλ κ²μ΄ μλ¬΄λλ μ’κ² μ§??

### β κ²μν λ§λ€κΈ°

1. μΉ μλΉμ€ κ°λ°μ κΈ°λ³Έμ νμ΅νκΈ° μ’λ€. κ²μνμ ν΅ν΄ κΈ°λ³ΈκΈ°λ₯Ό μ λ€μ§λ©΄ λ¬΄μμ΄λ  μμ© κ°λ₯
2. κ²μν λͺ©λ‘, λ³΄κΈ°, μμ , μμ±, μ­μ 
3. νμκ°μ, λ‘κ·ΈμΈ, λΉλ°λ²νΈ μ°ΎκΈ°, pagination, κ΅¬κΈ λ‘κ·ΈμΈ, μ μ  μμ±κΈ λͺ¨μλ³΄κΈ°

### β Template Engine

1. μλ²μμ ν΄λΌμ΄μΈνΈλ‘ λ³΄λΌ `HTML` ννλ₯Ό λ―Έλ¦¬ ννλ¦ΏμΌλ‘ μμ±νκ³  λμμμ λ―Έλ¦¬ μμ±λ ννλ¦Ώμ λ°μ΄ν°λ₯Ό λ£μ΄ μμ±λ `HTML`μ μμ±νλ€.
2. ννλ¦Ώ μμ§μ ννλ¦Ώ μμ± λ¬Έλ²κ³Ό ννλ¦Ώμ `HTML` ννλ‘ λ³ννλ κΈ°λ₯μ μ κ³΅νλ€.

![](https://images.velog.io/images/abcd8637/post/87224629-659a-4550-ac3d-4e76a6144652/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-08%2009.10.41.png)

3. `Express.js`μ ννλ¦Ώμμ§: `EJS`(htmlκ³Ό μ μ¬ν λ¬Έλ²), `Mustache`(κ°λ¨ν λ°μ΄ν° μΉνμ λλ§ μ κ³΅νλ κ²½λν λ ννλ¦Ώ μμ§), `Pug`(λ€μ¬μ°κΈ° ννμμ μ¬μ©ν κ°λ΅ν νκΈ°μ λ μ΄μμ λ± κ°λ ₯ν κΈ°λ₯μ μ κ³΅)

### β Pug

1. λ€μ¬μ°κΈ° ννμμ μ΄μ©ν΄ κ°λμ±μ΄ μ’κ³  κ°λ° μμ°μ±μ λμΈλ€.
2. `HTML`μ μ λͺ°λΌλ λ¬Έλ²μ μΈ μ€μλ₯Ό μ€μΌ μ μλ€.
3. `layout`, `include`, `mixin` λ± κ°λ ₯ν κΈ°λ₯μ μ κ³΅νλ€.
4. `HTML` λ«κΈ° νκ·Έ μμ΄ λ€μ¬μ°κΈ°λ‘ λΈλ­μ κ΅¬λΆνλ€.
5. `=` μ μ΄μ©ν΄ μ λ¬λ°μ λ³μλ₯Ό μ¬μ©ν  μ μλ€.
6. `id` λ `class` λ νκ·Έ λ€μ μ΄μ΄μ λ°λ‘ μ¬μ©νκ³ , `()` λ₯Ό μ΄μ©ν΄μ `attribute` λ₯Ό μ¬μ©νλ€.
7. `each-in`: `for` κ³Ό λΉμ·ν νκ·Έ
8. `if, else if, else` : μ‘°κ±΄λ¬Έ

```pug
// index.pug
html
	head
		title= title   // title λ³μ μ¬μ©
	body
		h1#greeting μλνμΈμ
		a.link(href="/") νμΌλ‘

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

// main.pug, λ°λ³΅λλ μΉμ¬μ΄νΈμ νμ μμ±νκ³  extendsνλ©° κ°λ°νλ©΄ λ§€μ° νΈλ¦¬νλ€.
extends layout  // layoutμ extendsνλ©΄ block λΆλΆμ μμ±ν HTML νκ·Έκ° ν¬ν¨λ¨
block content  // blockμ ν¬ν¨ν ννλ¦Ώμ layoutμΌλ‘ μ¬μ©κ°λ₯
	h1 Main Page

// include, layoutμ λ°κΉ₯μ μ μΈνκ³  κ°μ Έλ€ μ°κ³ , includeλ μ‘°κ°μ λ§λ€μ΄μ κ°μ Έλ€ μ΄λ€.
// μμ£Ό λ°λ³΅λλ κ΅¬λ¬Έμ λ―Έλ¦¬ μμ±νκ³  includeνμ¬ μ¬μ©νλ€.
// μΌλ°μ μΈ νμ€νΈνμΌλ includeνμ¬ ννλ¦Ώμ ν¬ν¨ κ°λ₯νλ€.

// title.pug
h1= title

// main.pug
extend layout
block content
	include titie
	div.content
		μλνμΈμ
	pre
		include article.txt

// mixin, ννλ¦Ώμ ν¨μμ²λΌ μ¬μ©ν  μ μλ€.
// includeλ κ°μ μ§μ ν  μ μμ§λ§, mixinμ νλΌλ―Έν°λ₯Ό μ§μ νμ¬ κ°μ λκ²¨λ°μ ννλ¦Ώμ μ¬μ©ν  μ μλ€.

// listItem.pug
mixin listItem(title, name)
	tr
		td title
		td name

// main.pug
include listItem
table
	body
		listItem('μ λͺ©', 'μ΄λ¦')
```

### β Express.jsμ pugμ μ°λ

1. `app.set` μ μ΄μ©ν΄ ννλ¦Ώμ΄ μ μ₯λλ λλ ν λ¦¬λ₯Ό μ§μ νκ³ , μ΄λ€ ννλ¦Ώ μμ§μ μ¬μ©ν μ§ μ§μ ν  μ μλ€.
2. `res.render` ν¨μλ `app.set` μ μ§μ λ κ°μ μ΄μ©ν΄ νλ©΄μ κ·Έλ¦¬λ κΈ°λ₯μ μννλ€. `render` ν¨μμ μ²« λ²μ¬ μΈμλ ννλ¦Ώμ μ΄λ¦, λλ²μ§ΈμΈμλ ννλ¦Ώμ μ λ¬λλ κ°

```javascript
// app.js
app.set("views", path.join(__dirname, "views"));
app.set("view engine", "pug");

// request handler
res.render("main", {
    title: "Hello Express",
});
```

3. `app.locals` : `render` ν¨μμ μ λ¬λμ§ μμ κ°μ΄λ ν¨μλ₯Ό μ¬μ©ν  μ μλ€. ννλ¦Ώμ μ μ­μΌλ‘ μ¬μ©λ  κ°μ μ§μ νλ μ­ν 

```javascript
// app.js
app.locals.appName = "Express"

// main.pug
h1= appName
<h1>Express</h1>
```

### β Express-generator μ¬μ© μ ννλ¦Ώ μμ§ μ§μ νκΈ°

1. `express-generator` λ κΈ°λ³Έμ μΌλ‘ `jade` λΌλ ννλ¦Ώ μμ§μ μ¬μ©νλ€.
2. `jade` λ `pug` μ μ΄μ  μ΄λ¦μΌλ‘, μ΅μ  μ§μμ λ°μΌλ €λ©΄ ννλ¦Ώ μμ§μ `pug` λ‘ μ§μ ν΄μΌ νλ€.
3. `--view`: ννλ¦Ώ μμ§μ μ§μ ν  μ μλ€.

```javascript
$ express --view=pug myapp
```

### β κ²μν CRUD λ§λ€κΈ°

1. λ°μ΄ν°λ₯Ό λ€λ£¨λ λ€ κ°μ§ κΈ°λ³Έμ μΈ κΈ°λ₯
2. Create: κ²μκΈ μμ±κΈ°λ₯, μ λͺ©, λ΄μ©, μμ±μ, μμ± μκ° λ±μ μ λ³΄λ₯Ό κΈ°λ‘ν¨, κ²μκΈμ μ λͺ©κ³Ό λ΄μ©μ μ΅μ nκΈμ μ΄μμ΄μ΄μΌ ν¨
3. Read: κ²μκΈμ λͺ©λ‘κ³Ό κ²μκΈμ μμΈλ₯Ό λ³Ό μ μμ΄μΌ ν¨. λͺ©λ‘μ κ°λ΅νλ μ λ³΄λ₯Ό λ³΄μ¬μ€, κ²μκΈ μμΈλ μ λͺ©, μμ±μ, λ΄μ©, μμ± μκ°, μμ  μκ° λ±μ μμΈν μ λ³΄λ₯Ό λ³΄μ¬μ€μΌ νλ€.
4. Update: κ²μκΈμ μμ μ΄ κ°λ₯ν΄μΌνλ€. μ λͺ©, λ΄μ©μ μμ νκ³ , μμ  μκ°μ κΈ°λ‘νλ€. (κ²μκΈ μμ μ μμ±μλ§ κ°λ₯νλ€. + νμκΈ°λ₯)
5. Delete: κ²μκΈ μ­μ νκΈ°, (κ²μκΈ μ­μ λ μμ±μλ§ κ°λ₯νλ€. + νμκΈ°λ₯)
6. λͺ¨λΈμ μΈνκΈ°: `ID` λ urlμ μ¬μ©νκΈ° μ’μ κ°μ΄ μλκΈ° λλ¬Έμ `shortId` λ‘ μμ±νλ€. μ λͺ©, λ΄μ©, μμ±μλ₯Ό `string` νμμΌλ‘ μ€ν€λ§μ μ μΈνλ€.(μμ±μλ νμκ°μ ν μ€μ) `timestamps`μ΅μμΌλ‘ μμ± μκ°, μμ  μκ°μ μλμΌλ‘ κΈ°λ‘ν΄μ€λ€.

```javascript
// shortId νμμ mongoose custom typeμΌλ‘ μ μΈ
// nanoid: μ€λ³΅ μλ λ¬Έμμ΄ μμ±
// defaultλ₯Ό μ΄μ©ν΄ λͺ¨λΈ μμ±μ μλμΌλ‘ μμ΄λ μμ±
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

### β κ²μκΈ μμ± νλ¦

1. `/posts?write=true` λ‘ μμ±νμ΄μ§ μ κ·Ό
2. `<form action="/posts" method="post">` λ₯Ό μ΄μ©ν΄ `post` μμ²­ μ μ‘
3. `[router.post](http://router.post)` λ₯Ό μ΄μ©νμ¬ `post` μμ²­ μ²λ¦¬
4. `res.redirect` λ₯Ό μ΄μ©νμ¬ `post` μλ£ μ²λ¦¬

```javascript
// ./routes/posts.js
const { Router } = require('express');

const router = Router();

router.get('/', (req, res, next) => {
	if (req.query.write){
		res.render('posts/edit');  // write κ°μ΄ μμΌλ©΄ editνμΌλ‘ μ°κ²°νλ€.
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
				th μ λͺ©
				td: input(type='text' name='title')
			tr
				th λ΄μ©
				td: textarea(name='content')
			td
				td(colspan="2")
					input(type="submit" value="λ±λ‘")

// ./routes/posts.js
const { Post } = require('./models);

router.post('/', async (req, res, next) => {
	const { title, content } = req.body;
	try{
		await Post.create({
			title,
			content,
	});
	res.redirect('/');  // κ²μκΈ μμ± ν ν νλ©΄μΌλ‘ μ΄λνκΈ°
	} catch(err){
		next(err);
	}
}
```

### β κ²μκΈ λͺ©λ‘ λ° μμΈ νλ¦

1. `/posts` λ‘ λͺ©λ‘ νμ΄μ§ μ κ·Ό
2. `<a href='/posts/:shortId'>` λ₯Ό μ΄μ©νμ¬ μμΈ URL link
3. `router.get('/:shortId')` path parameterλ₯Ό μ΄μ©νμ¬ μμ²­μ μ²λ¦¬ν¨

```javascript
// ./routes/posts.js
// μ²μ μ μμ λͺ¨λ  λ¦¬μ€νΈλ₯Ό λΆλ¬μ¨λ€.
router.get('/', async(req, res, next) => {
	const posts = await Post.find({});
	res.render('/posts/list', { posts });  // posts/listμ { posts } κ°μ΄ λμ΄κ°λ€.
});

router.get('/:shortId', async(req, rse, next) => {
	const { shortId } = req.params;
	const post = await Post.findOne({ shortId });
	if(!post){
		next(new Error('Post notfound!');
		return;
	}
	res.render('posts/view', { post });  // posts/viewλ‘ κ° λ³΄λ΄κΈ°
});

// ./views/posts/list.pug
...
	table
		tbody
			each post in posts  // eachλ‘ λ°λ³΅λ¬Έ λκΈ°
				tr
					td
						a(href='/posts/${post.shortId}') = post.title
					td= post.author
					td= formatDate(post.createdAt)  // formatDate: custom function
		tfoot
			tr
				td(colsapn='3')
					a(href="/posts?write=true") λ±λ‘νκΈ°

// app.js
// dayjs ν¨ν€μ§ μ¬μ©
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
				td: a(href='/posts/${post.shortId}?edit=true') μμ 
				td button(onclick=`deletePost("${post.shortId}")`) μ­μ 
```

### β κ²μκΈ μμ  νλ¦

1. `/posts/{shortId}?edit=true` λ‘ μμ νμ΄μ§ μ κ·Ό
2. μμ±νμ΄μ§λ₯Ό μμ νμ΄μ§λ‘λ λμνλλ‘ μμ±
3. `<form action="/posts/:shortId" method="post">` λ₯Ό μ΄μ©ν΄ `post` μμ²­ μ μ‘
4. html form μ `PUT method`λ₯Ό μ§μνμ§ μκΈ° λλ¬Έμ `post` μ¬μ©
5. `res.redirect` λ ν­μ GETμμ²­μΌλ‘ λμ΄κ°λ€.

```javascript
// ./routes/posts.js
router.get('/:shortId', async (req, res, next) => {
	if (req.query.edit){
		res.render('posts/edit', { post });
	}
	...
});

// μμ  μμ²­ μ²λ¦¬νκΈ°
router.get('/:shortId', async (req, res, next) => {
	const { shortId } = req.params;
	const { title, content } = req.body;
	const post = await Post.findOneAndUpdate({ shortId }, { title, content })  // shortIdλ₯Ό μ°Ύμ μλ‘μ΄ title, contentλ‘ λ°κΎΈκ² λ€.
	if(!post){  // μμΈ postκ° μμΌλ©΄
		next(new Error('Post notfound');
		return;
	}
	res.redirect(`/posts/${shortId}`);  // redirectλ ν­μ GETμμ²­μΌλ‘ λμ΄κ°λ€.
});

// ./views/posts/edit.pug
...
	- var action = post ? `/posts/${post.shortId}` : "/posts"  // postκ° μλ κ²½μ°μλ μμΈ νμ΄μ§λ‘ μ΄λ, κ·Έλ μ§ μμ κ²½μ°λ μμ±νκΈ° μν URLλ‘ λ³΄λΈλ€.
	form(action=action, method="post")
		table
			tr
				th μ λͺ©
				td: input(type="text" name="title" value=post&post.title) // postκ° μμΌλ©΄ μ λͺ©μ post.titleλ‘ μ±μ°κΈ°
			tr
				th λ΄μ©
				td: textarea(name="content")= post&&post.content  // postκ° μμΌλ©΄ λ΄μ©μ post.contentλ‘ μ±μ°κΈ°
			td
				td(colspan="2")
					- var value = post ? "μμ " : "λ±λ‘"
					input(type="submit" value=value)
```

### β κ²μκΈ μ­μ  νλ¦

1. κ²μκΈ μμΈ νμ΄μ§μ μ­μ  λ²νΌ μΆκ°
2. `html form` μ DELETE λ©μλλ₯Ό μ§μνμ§ μμ
3. `JS` λ₯Ό μ΄μ©ν΄ `fetch` ν¨μλ‘ `HTTP Delete` μμ²­ μ μ‘
4. `router.delete` μ μλ΅μ `fetch` μμ μ²λ¦¬

```javascript
// posts/view.pug
td
	button.delete(onclick='deletePost("${post.shortId}")') μ­μ 

// delete.pug, promiseλ‘ μ€νλλ€.
script(type="text/javascript").
	function deletePost(shortId){
		fetch('/posts/' + shortId, { method: 'delete' })
			.then((res) => {
				if (res.ok) {
					alert('μ­μ κ° μλ£λμμ΅λλ€.');
					window.location.href='/posts';  // μ­μ  μλ£ ν κ²μκΈ λͺ©λ‘μΌλ‘ μ΄λ
				}else{
					alert('μ€λ₯κ° λ°μνμ΅λλ€.');
					console.log(res.statusText);
				}
			})
		.catch((err) => {
			console.log(err);
			alert('μ€λ₯κ° λ°μνμ΅λλ€.');
		});
}

// μ­μ  μμ²­ μ²λ¦¬νκΈ°
// ./routes/posts.js
router.delete('/:shortId', async (req, res, next) => {
	const { shortId } = req.params;
	try{
		await Post.delete({ shortId });  // mongoDB λ΄ ν΄λΉ λ°μ΄ν° μ­μ 
		res.send('OK');
	}catch(e){
		next(e);
	}
});
```

### β Async Request Handler

1. κ³΅μμ μΌλ‘ μ¬μ©λλ `express` κΈ°μ μ μλκ³  ν¨ν΄ μ€ νλμ.
2. `async` ν¨μλ₯Ό μ‘°κΈ λ μ½κ² μ¬μ©ν  μ μκ³ , λΉλκΈ° μ€ν μ€ μ€λ₯ μ²λ¦¬λ₯Ό λ κ°λ¨νκ² ν  μ μλ μ₯μ μ΄ μλ€.
3. `request handler` μμ μ€λ₯λ₯Ό μ²λ¦¬νκΈ° μν λ°©λ² (`promise().catch(next)`, `async function, try - catch, next`)
4. `async` μ λΉλκΈ° μ²λ¦¬λ λ§€μ° νΈλ¦¬νμ§λ§, λ§€λ² `try-catch` κ΅¬λ¬Έμ μμ±νλ κ²μ κ·μ°?κ³  μ€μνκΈ° μ¬μ λ°λΌμ `request handler` λ₯Ό `async function` μΌλ‘ μμ±νλ©΄μ `try-catch next` λ₯Ό μλμΌλ‘ ν  μ μλλ‘ κ΅¬μ±ν μμ΄λμ΄
5. `asyncHandler` λ `requestHandler` λ₯Ό λ§€κ°λ³μλ‘ κ°λ ν¨μν λ―Έλ€μ¨μ΄, μ λ¬λ `requestHandler` λ `try-catch` λ‘ κ°μΈμ Έ `asyncHandler` λ΄μμ μ€νλκ³ , `throw` λλ μλ¬λ μλμΌλ‘ μ€λ₯μ²λ¦¬ λ―Έλ€μ¨μ΄λ‘ μ λ¬λλλ‘ κ΅¬μ±λ¨.
6. μ€λ₯μ²λ¦¬λ₯Ό μ¬λ°λ₯΄κ² μ¬μ©νμ§ μμΌλ©΄ `express` μ±μ΄ μ’λ£λ  μ μλ€.
7. `next` μΈμλ μ κ±°νκ³  `try-catch` κ΅¬λ¬Έμ μ κ±°ν΄λ λμΌνκ² μ€λ₯ μ²λ¦¬κ° κ°λ₯νλ€.

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

// μ€μ  μ μ© μ½λ(next μΈμλ λΉΌμ€μΌνλ€.)
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
      throw new Error('μ λͺ©κ³Ό λ΄μ©μ μλ ₯ν΄ μ£ΌμΈμ');
  }

  const post = await Post.create({ title, content });
  res.redirect(`/posts/${post.shortId}`);
}));

router.post('/:shortId', asyncHandler(async (req, res) => {
  const { shortId } = req.params;
  const { title, content } = req.body;
  if (!title || !content) {
      throw new Error('μ λͺ©κ³Ό λ΄μ©μ μλ ₯ν΄ μ£ΌμΈμ');
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

### β Pagination

1. λ°μ΄ν°κ° λ§μμ§λ©΄ ν νμ΄μ§μ λͺ©λ‘μ λͺ¨λ  λ°μ΄ν°λ₯Ό νννκΈ° μ΄λ €μ. λ°λΌμ λ°μ΄ν°λ₯Ό κ· μΌν μλ‘ λλμ΄ νμ΄μ§λ‘ λΆλ¦¬νλ κ²(ex, 10κ°μ© λλμ΄ 1νμ΄μ§λ 10~20, 2νμ΄μ§λ 11~20λ²κΉμ§ λ³΄μ¬μ£ΌκΈ°)
2. `page`: νμ¬ νμ΄μ§, `perPage`: νμ΄μ§ λΉ κ²μκΈ μ
3. `/posts?page=1&perPage=10` μ²λΌ `url query` λ₯Ό μ¬μ©ν΄ μ λ¬, `url query` λ λ¬Έμμ΄λ‘ λμ΄κ°κΈ° λλ¬Έμ μ¬μ©μ `number` λ‘ ν λ³νμ ν΄μ€μΌ νλ€.

```javascript
router.get( => {
	const page =
			Number(req.query.page || 1)  // `page`κ° μμΌλ©΄ default 1
	const perPage =
			Number(req.query.perPage || 10)  // `perPage`κ° μμΌλ©΄ default 10
})
```

4. `mongoDB` μ `limit`, `skip` μ μ¬μ©νμ¬ κ΅¬νλ κ°λ₯νλ€. (`limit`: κ²μ κ²°κ³Ό μ μ ν, skip: κ²μ μ ν¬ν¨νμ§ μμ λ°μ΄ν° μ)

```javascript
// λ°μ΄ν°μ μμκ° μ μ§ λ  μ μλλ‘ sortλ₯Ό μ¬μ©νλ€.
// μ΅μ μμΌλ‘ μ λ ¬νκ³  μ²μλΆν° λͺκ°μ κ²μλ¬Όμ μ μΈμν€κ³  λλ¨Έμ§ κ²μλ¬Όμ λͺκ°μ© κ°μ Έμ€λμ§
router.get(... => {
	const total = await Post.countDocument({});
	const posts = await Post.find({})
		.sort({ createdAt: -1 })  // μ΅μ μμ λ ¬
		.skip(perPage * (page - 1))
		.limit(perPage);
	const totalPage = Math.ceil(total / perPage);  // κ²μκΈ μ / νμ΄μ§ λΉ κ²μκΈ μ = μ΄ νμ΄μ§ μ
})

// pug
// patinationμ΄ νμν νμ΄μ§μμ ν΄λΉ ννλ¦Ώμ includeν ν, + paginationμΌλ‘ mixinμ μ¬μ© ν¨.
// νμ¬ νμ΄μ§λ b νκ·Έλ‘ κ΅΅κ² νμ
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

### β PM2 (Process Manager)

1. `Node.js` μ μμμ κ΄λ¦¬ν΄μ£Όλ `Process Manager`
2. `node` λͺλ Ήμ΄λ‘ μ€ν μ μ€λ₯ λ°μμ΄λ μ€ν μν κ΄λ¦¬λ₯Ό ν  μ μμ
3. `pm2` λ μμ κ΄λ¦¬λ₯Ό μν λ€μν μ μ©ν κΈ°λ₯μ μ κ³΅ν΄ μ€
4. μμ μ μΈ νλ‘μΈμ€ μ€ν: μ€λ₯λ°μ μ μλ μ¬μ€ν
5. λΉ λ₯Έ κ°λ°νκ²½: μμ€ μ½λ λ³κ²½ μ μλ μ¬μ€ν
6. λ°°ν¬ μ νΈλ¦¬ν κ΄λ¦¬: pm2μ λͺ¨λ  νλ‘μΈμ€λ₯Ό ν λ²μ κ΄λ¦¬
7. `pm2 init simple`, `pm2 init` μ΄ν `pm2 start` λͺλ Ήμ΄ μ€ν κ°λ° μ `watch` μ΅μ μ¬μ©νμ¬ νμΌ λ³κ²½ μ μλ² μλ μ¬μ€ν κ΅¬μ±

```javascript
// ecosystem.config.js
module.exports = {
	apps: [{
		name: 'simple-board',
		script: './bin/www',
		watch: '.',  // λͺ¨λ  κ²½λ‘λ₯Ό λ°λΌλ³Έλ€.
		ignore_watch: 'views',
	}],
}

$ pm2 start
```

---

## π 33μΌμ°¨ 12.9.λͺ©. μ€μκ° κ°μ

μ€λμ `graphQL`, `μΈμ¦`μ λν΄μ λ°°μ λ€. μ€μ΅μκ° λ§μ§λ§μλ `HTTP / HTTPS(SSL)`μ μ°¨μ΄, `cookie-session, JWT` λ°©μμ μ°¨μ΄μ λν΄μ μλ €μ£Όμ¨λλ° λλ¬΄ μ μ΅νλ€. `restAPI`μ `graphQL`μ μ°¨μ΄λ λ΄κ² μ€μΉκ³Όλ κ°μΌμ  <a href='https://blog.toycrane.xyz/rest-api%EA%B0%80-%EA%B0%80%EA%B3%A0-graphql%EC%9D%B4-%EC%99%94%EB%8B%A4-a9e400b77902'>νν°λ</a> λ―Έλμμ μ°Έκ³ νλ©΄ λμμ΄ λ§μ΄ λλ€.

### β REST API vs gql API

1. `gql` μ νλμ `Endpoint` λ§ μ‘΄μ¬
2. `REST API` λ `End point` λ§λ€ λ°μ΄ν°λ² μ΄μ€ `SQL` μΏΌλ¦¬κ° λ¬λΌμ§
3. `gql API` λ `gql` μ€ν€λ§μ νμλ§λ€ λ°μ΄ν°λ² μ΄μ€ `SQL` μΏΌλ¦¬κ° λ¬λΌμ§

### β GraphQL

1. FACEBOOKμμ 2015λμ λ°νν μλ‘μ΄ api κ·κ²©
2. `type system` μ κΈ°λ³Έμ μΌλ‘ κ°μΆκ³  μμ΄μ `REST` λ³΄λ€ ν¨μ¬ μμ μ 
3. `Apollo`, `Prisma` λ± λ°©λνκ³  κ°λ ₯ν μ€ν μμ€ ν΄λ€λ‘ μμ§μ κ°λ°μ κ²½ν κ°μ μ κΈ°λνλ€.
4. `SDL(Schema Definition Language)` : μλ²μ λ¬΄μμ μ§μνμ¬ κ°μ λλ €λ°κΈ°λ₯Ό μν  λ `SDL`λ‘ κΈ°μ (λͺνν νμμ μ μνμ¬ κΈ°μ )
5. `CLI` λ‘ `post` μμ²­μ μ λ°μ΄νλ₯Ό λΉΌλ λ³΄λ΄μ§λ€.

### β OAuth

1. μ κ·ΌκΆν μμμ μν κ³΅κ° νμ€
2. μ μ  μ§μμ₯λ²½μ΄ λ§€μ° λ?μμ§(μν΄λ¦­μΌλ‘ λ‘κ·ΈμΈ κ°λ₯)
3. μ μ κ° λΉλ°λ²νΈλ₯Ό κΈ°μ΅ν  νμκ° μμ΄μ§
4. μ μ  νμ© μ¬λΆμ λ°λΌ μ΄λ©μΌ, νλ‘ν μ¬μ§, λλ€μ λ±μ κΈ°λ³Έ μ λ³΄λ₯Ό μ»μ μ μλ€.

### β κΈ°ν λ΄μ©λ€

1. νλ‘μ νΈλ₯Ό ν  λ `F/E` λ₯Ό λλκΈ°λ³΄λ€λ κΈ°λ₯λ³λ‘ λ΄λΉνμ(ex, `login + front + back` / `pay + front + back`)κ³Ό κ°μ΄ μνμ μΌλ‘ μ μ)
2. νλ‘ νΈμ λ°±μ λλ μ κ°λ°νλ©΄ μλμμ μ°¨μ΄κ° λλ€. (μ²μμ λ°±μλκ° λλ¦¬λ€. DB, λ³΄μ, μΈνλΌ λ±λ±... λμ€μ λ°μνλλ¬Έμ νλ‘ νΈ κ°λ° μλκ° λ¦μ΄μ§λ€. μλ‘ μκ²¬μΆ©λμ΄ λλ€. μ¦, μ μ²΄μ μΈ νλ‘μ νΈκ° λ¦μ΄μ§κΈ° λλ¬Έμ μΉνμΉκ΅¬λ μλ ¨λ λΆλ€κ³Ό νλ©΄ κΈ°λ₯λ³λ‘ μͺΌκ°μ κ°λ°νλκ²μ κΆμ₯νλ€.)
3. ννλ¦Ώ μμ§: `html` μ½λμΈλ°, κ·Έ μμμ λ°λ³΅, μ‘°κ±΄μ λ‘ `view` λ₯Ό λ§λ€μ΄μ€ λ μ¬μ©νλ€.(μΌμΌμ΄ λ°λ‘ λ§λ€λ©΄ μ€λ³΅λλ μ½λκ° λ§κΈ° λλ¬Έμ λ‘μ§μ λΆμ¬μ μλμΌλ‘ `html` μ½λλ₯Ό λ§λ€μ΄μ€ λ) `EJS`, `JADE -> PUG` , `nunjunks` μ¬μ©λΉλ: `nunjunks` β `EJS`

```javascript
1. nunjunks: EJSμ μμνΈν(htmlμ λ?μ), junja2μ μν₯μ λ°μ(flaskμμ λμ¨?)
2. EJS: htmlμ λ?μ
3. pug: λ¬Έλ²μ΄ νΉμ΄ν΄μ λ°λ‘ κ³΅λΆν΄μΌν¨
```

4. `passport` : λ‘κ·ΈμΈ κ΅¬νμ νΈλ¦¬νκ² λμμ£Όλ μΉκ΅¬, μ΄κ² μμΌλ©΄ `header`, `session` κ΄λ¦¬λ₯Ό μ§μ  ν΄μ€μΌ νλ€. μ¨λνν° λ‘κ·ΈμΈλ μ§μνλ€.
5. λ‘κ·ΈμΈ νΉμ λ§μ΄νμ΄μ§λ₯Ό λ³΄μ¬μ£Όλ κΈ°λ₯ λ±μ μλ²λ‘λΆν° μΈμ¦μ λ°μμΌνλ μν©μΌ λ μ νμ§λ ν¬κ² 3κ°μ§ `cookie`, `cookie - session` , `JWT` λ°©μμ΄ μλ€. μλ²λ μ λ νκ°λ‘ μ΄μνμ§ μκ³ , 2κ° μ΄μμΌλ‘ μ΄μλλλ° μμ²­μ ν κ³³μμ λ€μ΄μ¨λ€. μ΄λ μμ²­μ μ¬λ¬κ°μ μλ² μ€ νκ³³μΌλ‘ λΆλ°°ν΄μ£Όλ μ₯μΉκ° νμνλ°, μ΄κ²μ΄ `LB(load balancer` λ€. `AWS` μμλ `ELB(elastic load balancer)` λΌκ³  λΆλ₯Έλ€.( `elastic: νλ ₯μ μΈ, κ³ λ¬΄μ`), `cookie-session` λ `DB` κ° νμνκ³ , `JWT` λ `DB` κ° νμνμ§ μλ€.
6. `cookie` λ°©μμ ν΄λΌμ΄μΈνΈμ μ μ₯λλ `key - value` λ‘ μ΄λ£¨μ΄μ§ λ°μ΄ν°λ€. μΈμ¦ μ ν¨μκ°μ μ€μ ν  μ μκ³ , μ ν¨μκ°μ΄ μ ν΄μ§λ€λ©΄ ν΄λΌμ΄μΈνΈκ° μ’λ£λμ΄λ μΏ ν€κ° μ μ§λλ€. κ·Έλ¬λ, μ€μμ λ³΄λ₯Ό μΏ ν€μ λ΄κ³ μμΌλ―λ‘ ν΄μ»€μκ² νμ·¨λΉνλ©΄ μ¬μ©μμ μ λ³΄λ₯Ό λͺ¨λ λΉΌμκΈΈ μ μλ€. κ·Έλμ μΏ ν€μμ²΄λ‘λ λ³΄μκ³Όλ μκ΄μλ κ°μΈ μ₯λ°κ΅¬λ, μλλ‘κ·ΈμΈ μ€μ  λ±μ μ¬μ©νλ€.
7. `cookie-session` λ°©μμ `client` μμ μμ²­μ λ³΄λ΄λ©΄ `server` μμ `cookie` μ κ°μ κ°μ§κ³  μλ€κ° `cookie` μ μΌμΉνλ `session` μ ν΄λΉ μλ²μμ μ°Ύκ³  `cookie` λ₯Ό μ¬μ©μμκ² λ³΄λ΄μ€λ€. κ·Έλ°λ°, μ¬λ¬κ°μ μλ²κ° μ°κ²°λμ΄μλ€κ³  κ°μ ν΄λ³΄μ. `server 1`μ νμ¬ `cookie`λ₯Ό κ°μ§κ³  μλ€κ° μ°κ²°μ΄ λκ²¨ λ€μ `LB` λ₯Ό κ±°μ³κ°μ 2λ²μ§Έ `server` λ‘ μ°κ²°μ΄ λλ©΄, `cookie` κ° μκΈ° λλ¬Έμ μ§κΈ μμ²­ν μ¬μ©μκ° μΈκ°λ μ¬μ©μμΈμ§ λͺ¨λ₯Έλ€. μ΄λ΄ λλ μλ²μ `session` λ°μ΄ν°λ₯Ό μ μ₯νμ§μκ³ , `DB`(redis) λ₯Ό μ΄μ©ν΄ ν΄λΉ `session` λ°μ΄ν°λ₯Ό `DB` μ μ μ₯νλ€. `DB` μμ μΏ ν€μ λ§λ μΈμλ°μ΄ν°λ₯Ό μ°Ύκ³  ν΄λΉνλ λ°μ΄ν°κ° μμΌλ©΄ λ¦¬νμ€νΈλ₯Ό λλ €μ€λ€. `DB` λ¨μ΄ λΆμκΈ° λλ¬Έμ μμ²­λμ΄ λ§μμ§λ©΄ μκ°μ΄ μ€λ κ±Έλ¦΄ μ μλ€.
8. `JWT` λ°©μμ `cookie-session` λ°©μκ³Ό λ€λ₯΄κ² `DB` λ¨μ΄ νμμλ€. `JWT` λ μΌμ’μ μ λΆμ¦μ΄λΌκ³  μκ°νλ©΄ νΈνλ€. `JWT` λ `JSON web Token` λ₯Ό λ»νλλ°, ν ν°μ νΉμ±μ μμ‘°κ° μλΉν μ΄λ ΅λ€. κ·Έλ¬λ νλ² νμ·¨λλ©΄ λ³΄μμ κ΅μ₯ν μ·¨μ½ν΄μ§λ€. μ΄λ₯Ό λ°©μ§νκ³ μ λ§λ£μκ°μ΄ μκ²Όλ€. μ΄λ λ§λ£μκ°μ λ³΄ν΅ 5-30λΆ κΈΈλ©΄ 1μ£ΌμΌμ λλ‘ μΈννλ€. μμ²­μ΄ μ€λ©΄ `JWT` λ₯Ό λ°κΈν΄μ€λ€. `mypage` λ‘ μμ²­μ΄ λ λΌμ€λ©΄ μμ²­κ³Ό ν¨κ» μ¨ `JWT` κ° μμ‘°λμλμ§ νμΈνλ€. μλ²μ μ μ₯λμ΄μλ `JWT` μ μΌμΉνλ©΄ `mypage` μμ²­μ κ°μ΄ λ³΄λ΄μ€λ€. `cookie-session` λ°©μμ²λΌ `DB` λ¨μμ μΈμ λ°μ΄ν°λ₯Ό νμΈν  μΌμ΄ μ¬λΌμ§λ€.
9. `http` (80), `https` (443): λ³΄μ μ λ¬΄, `get` μ `URL` μ `post` λ `http.body` μ μμ²­μ΄ λμ΄κ°λ€. κ·Έλμ `http.body` λ `postman` κ°μ νλ‘κ·Έλ¨μΌλ‘ μ΄μ΄λ³Ό μ μλ€. λ°λΌμ `http` μμ `get`, `post` μ λ³΄μμ μμ νμ§ μλ€.(`id`, `pw`, `cookie` κ° νλ¬ΈμΌλ‘ λ μκ°λ€.) νΉν, `cookie` λ₯Ό λμ²­νκ² λλ©΄ λ€λ₯Έ μ¬μ΄νΈμμ μ¬μ¬μ©ν  μ μλ°. (`cookie` λ λ‘κ·ΈμΈμ μ±κ³΅ν μ¬λμκ² λκ²¨μ£ΌκΈ°λλ¬Έμ λΈμΆλλ©΄ μννλ€.) `https` λ μ΄λ° `id`, `pw`, `cookie` κ° μνΈνκ° λμ΄ μλ²λ‘ λ μκ°λ€. κ·Έλμ μ€κ°μ ν΄μ»€κ° νμ·¨νκΈ° νλ€λ€. `curl` λͺλ Ήμ΄
10. `http -> https`: `DNS` κ° λ΄λΉνλ€. `http` λ‘ μμ²­μ΄ λ λΌμ€λ©΄ `DNS` μμ λ€μ ν΄λΌμ΄μΈνΈλ‘ λ°μ‘μ²λ¦¬ μν€κ³  ν΄λΌμ΄μΈνΈμμ `DNS` νν `https` λ‘ μμ²­νκ² λλ€. `server` μμ `client` λ‘ κ° λ `https` λ‘ λ³ννλ€.(ν­μ κ·Έλ°κ²μ μλκ³  λλΆλΆ μΊμ±μ΄ λμ΄μμ΄μ μ€κ°μ λ€μ μ΄)
11. `SSL` μΈμ¦μ: μ΄ μ¬μ΄νΈκ° μμ νμ§ νμΈνλ μΈμ¦μ(λνμ μΌλ‘ `AWS` certificate managerμμ λ°κΈν΄μ€λ€. μΈμ¦κΈ°κ΄μ λΉμ©μ μ§λΆνλ©΄ `DNS` μ λΆμ¬μ€λ€. λ§μ½, `SSL` μΈμ¦μκ° μμΌλ©΄ λ€μ λΈλΌμ°μ λ‘ λ¦¬ν΄νκ±°λ μλ¬λ₯Ό λ°μμν¨λ€.)
12. `node template engine` μ μλ²μμ νμΌμ λ³΄λ΄μ€μ λΈλΌμ°μ λ¨μμ λμ°κΈ°λ§ νλ€. μ΄λ° λ°©μμ `SSR`, λ°λλ‘ `CSR` μ λ¦¬μ‘νΈμμ νμΌμ λ§λ€κ³  λ°μ΄ν°λ§ μλ²μ μμ²­ν΄μ λλ€ ν©μΉλ©΄ `CSR` μ΄ λλ€.
13. `SSR` μ κ²μμμ§μ΄ λ°μ΄ν°λ₯Ό λͺ¨λ μ½μ μ μλ€. `CSR` μ νμΌμ νλ² κ±°μ³μ νμν΄μΌνκΈ° λλ¬Έμ λ°λ‘ λΈμΆμ΄ λμ§ μλλ€(feat. CORS)
14. λ¦¬μ‘νΈλ λΈλμλ²μ μ§μ  μμ²­ν΄μ λ°μμ€λκ²μ μλλ€. κ·Έλ₯ λΈλΌμ°μ λ‘ λ°μ΄ν°λ₯Ό λ³΄λ΄μ£Όκ³  λ°μ΄ν°λ λΈλΌμ°μ μμ μλ²λ‘ μμ²­νμ¬ λΈλΌμ°μ μμ μ·¨ν©νλ€.
15. λ‘κ·ΈμΈμ²λΌ `DB` μ¬μ©νλκ±΄ `node.js` μ¬μ©νκ³ , λ³΄μ¬μ£ΌκΈ°λ§ ν κ±°λ©΄ `CSR`
16. μ€ μλΉμ€ν λλ λ΄λΆ μΉμλ²λ³΄λ€ `nginx`λ₯Ό μ§μ  λΆμ΄λ νΈμ΄ λ μ’λ€. `node.js` λ λ΄λΆ μΉμλ²λ λ°°ν¬νκΈ° μΆ©λΆνλ€.
17. `AWS - route 53` μμ `DNS` μ `SSL` μ μ§μ  λΆμΈλ€. `ELB` μλ `SSL` μ λΆμ¬μΌνλ€. μ΄ν λ·λ¨μ μλ `EC2` μλ²λ‘ λμ΄κ°λ€.
18. `ELB` λ₯Ό μ°λ μ΄μ λ `autoScaling` μ μ°κΈ° μν¨μ΄λ€.
19. μΈμ€ν΄μ€λ₯Ό λλ¦΄ λλ μ¬μ©λ₯ μ΄ 51%λ₯Ό λμ΄μ°μ λ μ΄λ μλ²κ° ν°μ Έλ²λ¦¬λ©΄ λ€μμλ²λ `@ + 51%` κ° λλλ° λ€μ μλ²κ° 50μ΄λ©΄ μλ²κ° ν°μ Έλ²λ¦°λ€.

---

## π 34μΌμ°¨ 12.10.κΈ. μ¨λΌμΈ κ°μ

μ€λμ `νμκ°μ`, `passport.js`, `session-store`, `λκΈ κΈ°λ₯`μ λ°°μ λ€.

### β νμκ°μ

1. μ΄λ©μΌ, μ΄λ¦, ν¨μ€μλμ κ°λ¨ν μ λ³΄λ§ μ¬μ©(μ΄λ©μΌ νμμ΄ μ¬λ°λ₯Έμ§ νμΈ, λΉλ°λ²νΈ μ΅μ κΈΈμ΄ μ€μ , ν¨μ€μλμ ν¨μ€μλ νμΈ λ¬Έμκ° μΌμΉνλμ§ νμΈ)
2. νμμ λΉλ°λ²νΈλ₯Ό `DB`μ κ·Έλλ‘ μ μ₯νλ©΄, κ΄λ¦¬μκ° λͺ¨λ  νμμ λΉλ°λ²νΈλ₯Ό μ μ μκ³ , `DB`κ° ν΄νΉλλ©΄ λ³΄μ μ·¨μ½μ μ΄ λ°κ²¬νκ² λλ―λ‘ `hash`κ°μΌλ‘ λΉλ°λ²νΈλ₯Ό μ μ₯νλ€.(`hash`λ λ¬Έμμ΄μ λλλ¦΄ μ μλ λ°©μ), λΉλ°λ²νΈμ `hash`κ°μ `DB`μ μ μ₯νκ³ , λ‘κ·ΈμΈ μ μ λ¬λ λΉλ°λ²νΈλ₯Ό `hash`νμ¬ μ μ₯λ κ°κ³Ό λΉκ΅ν΄ λ‘κ·ΈμΈμ μ²λ¦¬νλ€.
3. `node.js`μ κΈ°λ³Έμ κ³΅ λͺ¨λμΈ `crypto` λͺ¨λμ μ¬μ©νμ¬ `hash` κ°μ μ»μ μ μλ€. κ°λ¨νκ² `sha1` μκ³ λ¦¬μ¦μ μ¬μ©νκ±°λ, λ³΄λ€ κ°λ ₯ν `sha224`, `sha256` λ±μ μκ³ λ¦¬μ¦λ μ¬μ©ν  μ μλ€.

```javascript
const hash = crypto.createHash("sha1");
hash.update(password);
hash.digest("hex");
```

4. νμκ°μ νμ΄μ§ κ΅¬ν -> `script`λ₯Ό μ΄μ©ν΄ μ΄λ©μΌ νμ, λΉλ°λ²νΈ νμΈ λ¬Έμ -> `form`μ μ΄μ©ν΄ `post` μμ²­ μ μ‘ -> νμκ°μ μ²λ¦¬ λ° `redirect`

```javascript
// λΉλ°λ²νΈ hash κ° μ μ₯
// μ΄λ―Έ μ‘΄μ¬νλ νμμΈμ§ μ²΄ν¬
// κ°μ ν λ©μΈνλ©΄μΌλ‘ redirect

router.post(... => {
	const { email, name, password } = req.body;
	const pwHash = getHash(password);
	const exists = await User.findOne({ email })

	if (exists){
		throw new Error("μ΄λ―Έ κ°μλ λ©μΌμλλ€.");  // try - catch λ¬Έμ΄ μλλ―λ‘ async request handlerλ₯Ό μ¬μ©νλ€.
	}

	await User.create({
		email,
		name,
		password: pwHash,
	})

	res.redirect('/');  // λ©μΈνλ©΄μΌλ‘ λ³΄λ΄κΈ°
})
```

### β passportλ?

1. `express.js` μ΄νλ¦¬μν€μμ κ°λ¨νκ² μ¬μ©μ μΈμ¦ κΈ°λ₯μ κ΅¬ννκ² λμμ£Όλ ν¨ν€μ§, μ μ§ μΈμ κ΄λ¦¬ λ° λ€μν λ‘κ·ΈμΈ λ°©μ μΆκ° κΈ°λ₯ μ κ³΅
2. `passport-local`: λ€μν λ‘κ·ΈμΈ λ°©μμ κ΅¬ννκΈ° μν΄ `strategy`λΌλ μΈν°νμ΄μ€λ₯Ό μ κ³΅νλ€. `strategy`λ μΈν°νμ΄μ€μ λ§κ² μ€κ³λ λ€μν κ΅¬νμ²΄(facebook, google, ...)λ€μ΄ μλ€. `passport-local` μ `username`, `password`λ₯Ό μ¬μ©νλ λ‘κ·ΈμΈ κ΅¬νμ²΄λ₯Ό μλ―Ένλ€.

```javascript
1. λ‘κ·ΈμΈ νλ©΄ κ΅¬μ±
2. passport-local strategyλ‘ λ‘κ·ΈμΈ κ΅¬ννκΈ°
3. passport.js μ€μ νκΈ°
4. passportλ‘ μμ²­ μ²λ¦¬νκΈ°

// passport-local stratgy
// config μ λ³΄ μ λ¬ -> authenticate μ€ν(configλ₯Ό μΈμλ‘ μ λ¬λ°μ μ΄λ©μΌ, ν¨μ€μλ, μλ£μ²λ¦¬ μ½λ°±ν¨μ(done)) -> λ°μ΄ν° μ°ΎκΈ°

const config = {
	usernameField: 'email',
	passwordField: 'password',
}

const local = new LocalStrategy(config, )

..., async(email, password, done) => {
	try{
		const user = await User.findOne({ email });
		if(!user){
			throw new Error("νμμ μ°Ύμ μ μμλλ€.");
		}

		if(user.password !== getHash(password)){
			throw new Error("λΉλ°λ²νΈκ° μΌμΉνμ§ μμλλ€.");
		}

	// μΈμμ μ μ₯λλ μ μ  μ λ³΄μ μ΅μν
    // μ²« λ²μ§Έ μΈμ: error, λλ²μ§ΈμΈμ: data
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
// μμ±ν strategyλ₯Ό passport.userλ₯Ό μ΄μ©ν΄ μ¬μ©νλλ‘ μ μΈν΄μΌ ν¨
// passport.useλ₯Ό μ΄μ©ν΄ strategyλ₯Ό μ¬μ©νλλ‘ μ μΈν ν passport.authenticateλ₯Ό μ¬μ©ν΄ ν΄λΉ strategyλ₯Ό μ΄μ©ν΄ μμ²­μ μ²λ¦¬ν  μ μμ
const local = require('./strategies/local');
passport.use(local);

// routes/auth.js
router.post('/',
	passport.authenticate('local');
...

// app.js
// passport.authenticate ν¨μλ₯Ό http λΌμ°νμ μ°κ²°νλ©΄ passportκ° μλμΌλ‘ ν΄λΉνλ strategyλ₯Ό μ¬μ©νλ request handlerλ₯Ό μλ μμ±
// express-sessionκ³Ό passport.session()μ μ¬μ©νλ©΄ passportκ° λ‘κ·ΈμΈ μ μ μ  μ λ³΄λ₯Ό μΈμμ μ μ₯νκ³  κ°μ Έμ€λ λμμ μλμΌλ‘ μνν΄ μ€
const session = require('express-session');
app.use(session({
	secret: 'secret',
	resave: false,
	saveUninitialized: true,
}));

app.use(passport.initialize());
app.use(passport.session());
app.use('/auth', authRouter);

// session μ μ  νμ©νκΈ°
// sessionμ μ΄μ©ν΄ userλ₯Ό μ¬μ©ν  λλ serializeUserμ deserializeUserλ₯Ό μ€μ νλ€.
// μ΄λ μΈμμ userμ λ³΄λ₯Ό λ³ννμ¬ μ μ₯νκ³  κ°μ Έμ€λ κΈ°λ₯μ μ κ³΅νλ€.(νμ idλ§ μΈμμ μ μ₯νκ³  μ¬μ© μ νμμ λ³΄λ₯Ό λλΉμμ μ°Ύμμ μ¬μ©)
// μΈμ μ¬μ© μ μ λ ν¨μλ₯Ό μμ±νμ§ μμΌλ©΄ passport λ‘κ·ΈμΈμ΄ λμνμ§ μμ
passport.serializeUser((user, callback) => {
	callback(null, user)
})

passport.deserializeUser((obj, callback) => {
	callback(null, obj)
})

// logout
// passportλ req.logout ν¨μλ₯Ό ν΅ν΄ μΈμμ λ‘κ·ΈμΈ μ λ³΄λ₯Ό μ­μ νμ¬, λ‘κ·Έμμ κΈ°λ₯μ κ΅¬νν  μ μλ€.
router.get('/logout', ... {
	req.logout();
	res.redirect('/');
})

// login νμΈ λ―Έλ€μ¨μ΄
// λ‘κ·ΈμΈμ νμλ‘ μ€μ νκ³  μΆμ κ²½μ°, λ―Έλ€μ¨μ΄λ₯Ό μ¬μ©νμ¬ μ²΄ν¬ν  μ μμ
function loginRequired(req, res, next){
	if(!req.user){
		res.redirect('/');
		return;
	}
	next();
}

app.use('/posts', loginRequired, postsRouter)  // λ‘κ·ΈμΈμ΄ νμΈλλ©΄ postsRouterλ‘ λμ΄κ°λ€.
```

### β Session

1. μΉ μλ²κ° ν΄λΌμ΄μΈνΈμ μ λ³΄λ₯Ό ν΄λΌμ΄μΈνΈλ³λ‘ κ΅¬λΆνμ¬ μλ²μ μ μ₯νκ³ , ν΄λΌμ΄μΈνΈ μμ²­μ `session ID`λ₯Ό μ¬μ©νμ¬ ν΄λΌμ΄μΈνΈμ μ λ³΄λ₯Ό λ€μ νμΈνλ κΈ°μ (ν΄λΌμ΄μΈνΈκ° μ λ³΄λ₯Ό μ μ₯νκ³  μμ²­μ μ λ³΄λ₯Ό λ³΄λΈ `Cookie`μ λμ‘° λ¨)
2. μλ²λ μΈμμ μμ±νμ¬ μΈμμ κ΅¬λΆμμΈ `session ID`λ₯Ό ν΄λΌμ΄μΈνΈμ μ λ¬ν¨. ν΄λΌμ΄μΈνΈ μμ²­μ `session ID`λ₯Ό ν¨κ» λ΄μμ μ μ‘, μλ²λ μ λ¬λ°μ `session ID`λ‘ ν΄λΉνλ μΈμμ μ°Ύμ ν΄λΌμ΄μΈνΈ μ λ³΄λ₯Ό νμΈν¨
3. `express-session` ν¨ν€μ§λ₯Ό μ¬μ©νμ¬ κ°λ¨νκ² `session` λμμ κ΅¬νν  μ μλ€. νΉλ³ν μ€μ  μμ΄ μλμΌλ‘ `session`λμμ κ΅¬νν΄μ€, γλμΌλ‘ `session ID`λ₯Ό ν΄λΌμ΄μΈνΈμκ² μ λ¬, `session ID`λ‘ ν΄λΌμ΄μΈνΈ μ λ³΄ νμΈ

### β Session Storeλ₯Ό μ¬μ©νλ μ΄μ 

1. `express-session` ν¨ν€μ§λ `session` μ κΈ°λ³Έμ μΌλ‘ λ©λͺ¨λ¦¬μ μ μ₯ν¨. λ°λΌμ νμ¬ κ΅¬νλ μ΄νλ¦¬μΌμ΄μμ μ’λ£ ν λ€μ μ€ννλ©΄ λͺ¨λ  μ μ μ λ‘κ·ΈμΈ ν΄μ λ¨, νΉμ μλ²κ° μ¬λ¬ λ μμ κ²½μ°, μλ² κ° μΈμμ λ³΄λ₯Ό κ³΅μ ν  μ μμ

### β MongoDB - Session Store

1. `connect-mongo` ν¨ν€μ§λ₯Ό μ΄μ©ν΄ `MongoDB` λ₯Ό `session store` λ‘ μ¬μ©ν  μ μλ€.
2. `connect-mongo` ν¨ν€μ§λ `express-session` ν¨ν€μ§μ μ΅μμΌλ‘ μ λ¬ κ°λ₯νλ€. μλμΌλ‘ `session` κ°μ΄ λ³κ²½λ  λ `update` λκ³  `session` μ΄ νΈμΆλ  λ `find` ν¨
3. μ¬λΆνλμ΄λ `data` κ° μ­μ λμ§ μκΈ° λλ¬Έμ `session-data` λ₯Ό μ μ§ ν  μ μλ€.
4. μΈμλ°μ΄ν°λ₯Ό λͺ½κ³ λλΉμ μ μ₯νκ³  κ΄λ¦¬νλ κΈ°λ₯μ μλμΌλ‘ μνν΄ μ€

```javascript
// connect-mongo ν¨ν€μ§λ₯Ό μ΄μ©ν΄ express-session μ€μ μ store μ΅μμ μ λ¬ λ° mongoUrl μ€μ 
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

### β νμκ³Ό κ²μκΈμ μ°λ

1. κ²μκΈ μμ±μ λ‘κ·ΈμΈλ νμ μ λ³΄λ₯Ό μμ±μλ‘ μΆκ°

```javascript
// PostSchemaμ author μΆκ°
// populateλ₯Ό μ¬μ©νκΈ° μν΄ ObjectID μ¬μ©
// refλ₯Ό μ μ  λͺ¨λΈμ μ΄λ¦μ 'User'λ‘ μ μΈ
author: {
	type: Schema.Types.ObjectId,
	ref: 'User',
	required: true,
}

// κ²μκΈμ μμ±μ μΆκ°
// req.userμλ straegyμλ μ΅μνμ μ λ³΄μΈ shortId, email, usernameλ§ κ°μ§κ³  μλ€.
// Post μμ± μ userμ ObjectIDλ₯Ό μ λ¬ν΄μΌνλλ°, Userμμ shortIdλ‘ νμμ κ²μνμ¬ ν λ² λ κ²μ¦
// κ°μ²΄κ° μ£Όμ΄μ§λ©΄ μλμΌλ‘ ObjectID μ¬μ©
const author = await User.find({
	shortId: req.user.shortId,
})

if(!author){
	throw new Error('No User')
}

await Post.create({
	title,
	content,
	author,  // authorλ§ λ€μ΄κ°μλκ² μλκ³  userκ°μ²΄ dataμ μ²΄κ° λ€μ΄κ°λλ°, mongoDBκ° μ¬κΈ°μ _idλ§ κΊΌλ΄μ μ μ₯ν΄μ€λ€.
})
```

2. κ²μκΈ - μμ±μλ populate νμ¬ μ¬μ©νλλ‘ κ΅¬ν

```javascript
// populate
// μλμΌλ‘ user collectionμμ authorλ₯Ό μ°Ύμμ λ£μ΄μ€λ€.
const posts = await Post.find({}).populate("author");

res.render("posts/list", { posts }); // postsλ₯Ό λ°λ³΅λ¬ΈμΌλ‘ κΊΌλ΄ μΈ μ μλ€.
```

3. κ²μκΈ μμ , μ­μ  μ λ‘κ·ΈμΈλ μ μ μ μμ±μκ° μΌμΉνλμ§ νμΈ

```javascript
// μμ , μ­μ  μ μ μ  νμΈ
const post = await Post.find({ shortId }).populate("author");

if (post.author.shortId !== req.user.shortId) {
    throw new Error("Not Authorized");
}
```

4. μμ±μμ κ²μκΈ λͺ¨μ λ³΄κΈ° κΈ°λ₯ κ΅¬ν: κΈ°λ³Έμ μΌλ‘ `MongoDB` λ `Document` κ²μ μ μ μ²΄ λ¬Έμλ₯Ό νλμ© νμΈνκΈ° λλ¬Έμ λ§€μ° λΉν¨μ¨μ μΈ κ²μμ μννλ€. λ°μ΄ν°κ° λ§μμ§ κ²½μ° μλ μ νμ ν° μμΈμ΄ λλ€. κ²μμ μν΄ `Document` λ₯Ό μ λ ¬νλ κΈ°λ₯μ μ κ³΅ν¨. index λ₯Ό μ€μ νλ©΄ μ£Όμ΄μ§ μΏΌλ¦¬λ₯Ό ν¨μ¨μ μΌλ‘ μννμ¬ μ±λ₯μ ν₯μμν¬ μ μλ€.

```javascript
// index: true μ΅μμ μ¬μ©νλ©΄ mongooseκ° μλμΌλ‘ MongoDBμ μΈλ±μ€λ₯Ό μμ±ν΄μ€
// μ΄λ―Έ λ°μ΄ν°κ° λ§μ λ index μΆκ°μ μμμκ°μ΄ κΈΈμ΄μ Έ MongoDBκ° μλ΅νμ§ μμ μ μλ€. μμλλ μΈλ±μ€λ₯Ό λ―Έλ¦¬ μΆκ°νλ κ²μ΄ μ’μ(μ²μλΆν° μ€μ ))
author: {
	type: Schema.Types.ObjectId,
	ref: 'User',
	required: true,
	index: true,
}
```

5. νμ κ²μκΈ λΌμ°ν μΆκ°νκΈ°: RESTful ν κ΅¬μ±μ μν΄ /users/{userId}/posts λ‘ κ΅¬μ±, κ²μκΈ λͺ©λ‘ view λ κΈ°μ‘΄μ μμ±ν posts/list.pug λ₯Ό μ¬νμ©

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

h2= user ? `${user.name}μ κ²μκΈ` : `μ μ²΄ κ²μκΈ`
td: a(href=`/users/${post.author.shortId}/posts`)
	= post.author.name
```

### β CSRλ‘ λκΈ κΈ°λ₯ κ΅¬ννκΈ°

1. νμ΄μ§ λ‘λ μ νμν λ¦¬μμ€λ₯Ό ν΄λΌμ΄μΈνΈμ μ μΈ(HTML Template, λΈλΌμ°μ μ νμλμ§ μλ HTML elementλ₯Ό μμ±ν΄λκ³  JSλ‘ μ΄λ₯Ό νλ©΄μ λ°λ³΅μ μΌλ‘ κ·Έλ¦΄ μ μκ² νλ κΈ°μ )
2. ν΄λΌμ΄μΈνΈμμ νμν λ°μ΄ν°λ₯Ό λΉλκΈ° νΈμΆ
3. ν΄λΌμ΄μΈνΈκ° μ λ¬λ°μ λ°μ΄ν°λ₯Ό κ°κ³΅, λ¦¬μμ€λ₯Ό μ¬μ©νμ¬ νλ©΄μ νμ
4. `HTML template` μ¬μ©νμ¬ ν κ°μ λκΈμ΄ νμλ  λͺ¨μμ μ μΈ(JSλ‘ μ‘°μνκΈ° μν΄ `id`, `class` λ₯Ό μ μΈνλ κ²μ΄ μ μ©νλ€)
5. `CSR` μ κ΅¬ννκΈ° μν΄μλ `HTML` μ΄ μλ λ°μ΄ν°λ§ μ£Όκ³ λ°μ μ μλ `API` λ₯Ό κ΅¬μ±ν΄μΌνλ€.(JSON μ¬μ©), λκΈ μμ± μ λκΈλͺ©λ‘μ λ€μ λΆλ¬μ κ·Έλ¦¬λ νμμΌλ‘ κ΅¬ν
6. `sub-schema` λ₯Ό μ΄μ©νμ¬ `Post` μ€ν€λ§μ `Comment` λ₯Ό λ°°μ΄λ‘ μΆκ°

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

7. λκΈ μμ±: `api/posts/{postId}/comments` κ²½λ‘λ‘ λκΈ μμ± κΈ°λ₯ κ΅¬ν, κ²μκΈ μλ°μ΄νΈμ `${push}` λ₯Ό μ¬μ©νμ¬ `comments` λ°°μ΄μ μλ‘ μμ±λ λκΈ μΆκ°(λμμ λ€μ΄μ€λ μμ²­μ μ ννκ² μ²λ¦¬), `api` λ `render` λμ  `json` μΌλ‘ μλ΅

```javascript
// λκΈ μλ°μ΄νΈ
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

// λκΈ λͺ©λ‘
// findμ populateνμ§ μκ³ , User (model)μ populateλ₯Ό μ¬μ©νλ λ°©λ²λ κ°λ₯
await User.populate(posts.comments, {
    path: "author",
});
```

8. λΉλκΈ° HTTP μμ²­μ `fetch` ν¨μλ₯Ό μ΄μ©ν¨.

```js
// λκΈ μμ±νκΈ°
// νΈμΆ κ²°κ³Όμ μ±κ³΅ μ¬λΆλ₯Ό νμΈνμ¬, λκΈ λ€μ λΆλ¬μ€κΈ° μ€ν
fetch('url', {
	method: "post",
	headers: { ~ },
	body: JSON.stringify({ content }),
})
```

### β MongoDB Aggregation

1. MongoDBμμ Documentλ€μ κ°κ³΅, μ°μ°νλ κΈ°λ₯
2. RDMBSμμ SQLλ‘ μνν  μ μλ κΈ°λ₯λ€μ μ μ¬νκ² κ΅¬νν  μ μμ (SQLμ GROUP BY, DISTINCT, COUNT, JOIN λ±)
3. mongoDBμ findλ κ²μ νν°λ§κ³Ό μ λ ¬ μ΄μΈμ κΈ°λ₯μ μ κ³΅νμ§ μμ, λ€λ₯Έ collectionμμ λ°μ΄ν°λ₯Ό κ°μ Έμ€κ±°λ, κ·Έλ£Ήνν λλ Aggregationμ ν΅ν΄ μ΄λ₯Ό μνν  μ μμ

---

## π 35μΌμ°¨ 12.11.ν . μ¨λΌμΈ κ°μ

μ€λμ `JWT` κ·Έλ¦¬κ³  νμ λΉλ°λ²νΈ μ°ΎκΈ°, `SMTP`λ₯Ό μ΄μ©νμ¬ λ©μΌ λ°μ‘κΈ°λ₯, λΉλ°λ²νΈ μ΄κΈ°ν, `OAuth`, μΉ μλ² μννΈμ¨μ΄μΈ `Nginx`μ λν΄μ λ°°μ λ€. λμ€μ λ‘κ·ΈμΈ κ΄λ ¨ κΈ°λ₯μ κ΅¬νν  λ μ¨λ¨ΉμΌλ©΄ λμμ΄ λλ λ΄μ©μ΄λΌμ κΉλ¨Ήμ§ μκ³  κΈ°μ΅ν΄μΌκ² λ€.

### β JWT(Json Web Token)

1. μΈμ¦μ μν μ λ³΄λ₯Ό νΉλ³ν μ μ₯μλ₯Ό μ΄μ©νμ§ μκ³ , μ μ μλͺμ μ΄μ©νμ¬ νμΈνλ λ°©λ²
2. `header`(ν ν°μ νμ(jwt), λ°μ΄ν° μλͺλ°©μ), `payload`(μ λ¬λλ λ°μ΄ν°), `signature` (ν€λμ νμ΄λ‘λμ μ μμλͺ)λ‘ κ΅¬μ±λμ΄ μλ€.
3. `JWT` λ `Web Token`, λ°μ΄ν°λ₯Ό μΉμμ μ¬μ©νκΈ° μν μ€νμ΄λ―λ‘ μΉμμ λ¬Έμ μμ΄ μ¬μ©ν  μ μλ λ¬Έμμ΄λ‘λ§ κ΅¬μ±λ `base64` μΈμ½λ©μ μ¬μ©νλ€.
4. `JWT` μ `payload` λ λ¨μν μ λ³΄λ₯Ό `base64 encode` β `decode` μ μ λ³΄κ° λΈμΆλλ€ β λ―Όκ°ν μ λ³΄λ μ μΈνκ³  ν ν°μ μμ±νλ€.
5. μλ²λ `JWT` λ₯Ό μμ±ν  λ, λΉκ³΅κ°ν€λ₯Ό μ΄μ©νμ¬ μλͺμ ν¨. `payload` λ₯Ό μ‘°μν  κ²½μ° μλͺ(signature)μ΄ μΌμΉνμ§ μκΈ° λλ¬Έμ μΈμ¦ μ€ν¨
6. μ¬μ©μ λ‘κ·ΈμΈ β μλ²λ λ‘κ·ΈμΈλ μ μ  μ λ³΄λ₯Ό JWT λ‘ μμ±νμ¬ ν΄λΌμ΄μΈνΈμ μ λ¬ β ν΄λΌμ΄μΈνΈλ μ λ¬λ°λ JWT λ₯Ό μ΄μ©νμ¬ μΈμ¦μ΄ νμν μμ²­μ μ¬μ©

![](https://images.velog.io/images/abcd8637/post/080642e9-3012-4b15-8761-b2bc72473699/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-11%2009.31.32.png)

### β JWT μ¬μ© μ΄μ 

1. `session` μ κΈ°λ³Έμ μΌλ‘ μΉ λΈλΌμ°μ λ₯Ό μν ν΅μ  μ€ν
2. λͺ¨λ°μΌ μ± λ±, μΉ λΈλΌμ°μ κ° μλ μ΄νλ¦¬μΌμ΄μμ κ²½μ° `session` μ νμ©νκΈ° λΆμ ν©ν¨, `JWT` λ₯Ό μ¬μ©νλ©΄ μ΄λ ν΄λΌμ΄μΈνΈμμλ λμΌν λ°©μμ μ¬μ©μ μΈμ¦μ κ΅¬ν κ°λ₯

### β JWT + Cookie

1. `cookie`: μΉ μλΉμ€μμ μ¬μ©νλ μ λ³΄λ₯Ό ν΄λΌμ΄μΈνΈ(λΈλΌμ°μ )μ μ μ₯νκ³ , `HTTP` μμ²­μ μ΄λ₯Ό ν¨κ» μ μ‘νμ¬ ν΄λΌμ΄μΈνΈ μ λ³΄λ₯Ό μλ²μ μ λ¬νλ κΈ°μ 
2. `session`: ν΄λΌμ΄μΈνΈ μ λ³΄λ₯Ό μλ² μΈ‘ μ μ₯μμ μ μ₯νκ³  μ¬μ©(`session id` λ‘ `session store` μμ νμΈν΄μ ν΄λΌμ΄μΈνΈ μ λ³΄λ₯Ό νμΈν¨),
3. `session` μ μ¬μ©ν μ μ  λ‘κ·ΈμΈ: `cookieμ session ID` μ μ₯ β `session store` μμ μ μ  μ λ³΄ κ°μ Έμ€κΈ°
4. `JWT` λ₯Ό μΏ ν€μ²λΌ μ¬μ©νλ κ²½μ°: `JWT` λ‘ μμ²­ β μλͺ νμΈ ν μ μ  μ λ³΄ μ¬μ©(DB μ κ·Όμ΄ νλ¨κ³ μ€μ΄μ ν¨μ¨μ μΈ μΈμ¦ κ΅¬ν κ°λ₯)
5. λ‘κ·ΈμΈ λ‘μ§μμ `JWT` μμ± ν μΏ ν€λ‘ μ λ¬ β `passport-jwt` ν¨ν€μ§λ‘ `JWT λ‘κ·ΈμΈ λ―Έλ€μ¨μ΄` μμ± λ° μ¬μ©

```js
// token μμ± λ° λ―Έλ€μ¨μ΄ μ μΈνκΈ°
setUserToken = (res, user) => {
	const token = jwt.sign(user, secret);
	res.cookie('token', token);  // res.cookie ν¨μλ₯Ό μ¬μ©νμ¬ tokenμ ν΄λΌμ΄μΈνΈ μΏ ν€λ‘ μ λ¬
}

---
router.post('/', passport.authenticate('local'),
	(req, res, next) => {
		setUserToken(res, req.user);  // μΏ ν€λ₯Ό λΈλΌμ°μ μ μ μ₯ν¨

	res.redirect('/');
});

// passport-jwt μ¬μ©νκΈ°
// μμ²­λ JWTν ν°μ μλͺμ νμΈνκ³  μΈμ¦νλ κΈ°λ₯μ κ΅¬ν
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

6. `JWT` ν ν°μ κΈ°λ³Έμ μΌλ‘ λͺ¨λ  μμ²­μ ν¬ν¨νλ€. μμ²­μ ν ν°μ΄ μλ κ²½μ° λ‘κ·ΈμΈλ μνλ‘ μ²λ¦¬νκΈ° μν΄ λͺ¨λ  μμ²­μ κ³΅ν΅μ μΌλ‘ μ μ©ν  μ μλ λ―Έλ€μ¨μ΄λ‘ `JWT` λ‘κ·ΈμΈμ μΆκ°
7. λ‘κ·Έμμμ κ°λ¨νκ² ν΄λΌμ΄μΈνΈ μΏΌλ¦¬λ₯Ό μ­μ νμ¬ μ²λ¦¬ κ°λ₯, `token` κ°μ `null` λ‘ μ λ¬νκ³  `cookie` μ λ§λ£μκ°μ 0μΌλ‘ μ€μ νμ¬ ν΄λΌμ΄μΈνΈκ° μΏ ν€λ₯Ό λ°λ‘ λ§λ£μν€λλ‘ μ λ¬

```js
// jwt middleware
app.use((req, res, next) => {
    if (!req.cookies.token) {
        next();
        return;
    }

    return passport.authenticate("jwt")(req, res, next); // req.userμ μ μ₯
});

// jwt logout
res.cookie("token", null, {
    maxAge: 0, // μΏ ν€ λ§λ£ μν€κΈ°
});
```

### β νμ λΉλ°λ²νΈ μ°ΎκΈ° κ΅¬ν

1. μμμ λ¬Έμμ΄λ‘ λΉλ°λ²νΈ μ΄κΈ°ν
2. μ΄κΈ°νλ λ¬Έμμ΄μ λ©μΌλ‘ μ λ¬ β λ©μΌ λ°μ‘κΈ°λ₯ κ°λ° νμ
3. μ΄κΈ°ν ν μ²« λ‘κ·ΈμΈ μ λΉλ°λ²νΈ λ³κ²½ μμ²­

### β λ©μΌ λ°μ‘κΈ°λ₯ κ΅¬ν λ°©λ²

1. `SMTP` μλ² μ΄μ©: λ€μ΄λ² κ΅¬κΈ λ±μ λ©μΌμλ²λ₯Ό μ΄μ©νμ¬ λ¬΄λ£λ‘ λ°μ‘ κ°λ₯, λ©μΌ λ°μ‘ λ° κ΄λ¦¬ κΈ°λ₯ μ§μ  κ°λ° νμ
2. λ©μΌ λ°μ‘ μλΉμ€ μ΄μ©(Mailgun, Sendgrid): λ©μΌ λ°μ‘ api μ κ³΅ λ° κ΄λ¦¬μ© μΉνμ΄μ§ μ κ³΅, μ¬μ©λμ λ°λΌ μ λ£ κ³ΌκΈ

### π‘Β SMTPλ?

1. `Simple Mail Transfer Protocol`: λ©μΌ μ μ‘μ μν νμ€ κ·μ½, `SMTP` μλ²λ νμ€ κ·μ½μ ν΅ν΄ λ©μΌ μ μ‘νλ κΈ°λ₯μ κ΅¬νν μλ²
2. `Node.js` μμ λ©μΌ λ°μ‘νκΈ°: `Nodemailer` ν¨ν€μ§λ₯Ό μ¬μ©νμ¬ `SMTP` μλ²(gmail, naver...)λ₯Ό ν΅ν΄ λ©μΌ λ°μ‘νκΈ°, μ§μ  λ§λλ κ²μ λΉν¨μ¨μ μ΄λ€.
3. `Nodemailer` μμ `gmail` μ μ¬μ©νκΈ° μν΄μλ μ± λΉλ°λ²νΈ μ€μ  νμ, νλ² μ€μ νλ©΄ μ¬ νμΈ λΆκ°

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

### β λΉλ°λ²νΈ μ΄κΈ°ν κΈ°λ₯

```js
// μμμ λ¬Έμμ΄μ λ§λ€μ΄μ£Όλ ν¨μ
function generateRandomPassword(){
	return Math.floor(
		Math.random() * (10 ** 8)
		).toString().padStart('0', 8);
}
---

// emailμ λ°μμ generateRandomPasswordλ‘ μ¬μ©μμ λΉλ°λ²νΈ μ΄κΈ°ν ν λ©μΌλ‘ λ°μ‘
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

### β λΉλ°λ²νΈ μ΄κΈ°ν ν λ‘κ·ΈμΈ μ λΉλ°λ²νΈ λ³κ²½ μμ²­

```js
// λΉλ°λ²νΈ λ³κ²½
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

// λΉλ°λ²νΈ λ³κ²½ μμ²­
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

### β OAuthμ μ΄ν΄

1. `open authorization`: μλΉμ€ μ κ³΅μκ° λ€λ₯Έ μλΉμ€μκ² λ°μ΄ν°λ₯Ό μ κ³΅νκΈ° μν΄ μλΉμ€ μ¬μ©μμκ² μ κ³΅νλ μ¬μ©μ μΈμ¦λ°©μμ νμ€
2. μλΉμ€ μ κ³΅μμκ² μΈμ¦ μμ²­ β μΈμ¦ μλ£ ν μ¬μ©μ μ λ³΄λ₯Ό μμ²­ν μλΉμ€λ‘ μ λ¬ β μΈμ¦ μ λ³΄λ₯Ό μ΄μ©ν΄ μλΉμ€ μ κ³΅μμ λ°μ΄ν° μ¬μ©
3. κ΅¬κΈ `OAuth` μΈμ¦ μμ²­ β μΈμ¦λ `OAuth Token` μ κΈ°λ‘ β `OAuth Token` μ μ¬μ©νμ¬ κ΅¬κΈ μΊλ¦°λ `API` μ¬μ©
4. μΉ μλΉμ€ μ κ³΅μλ ID, PW λ‘κ·ΈμΈμ κ΅¬νν  νμκ° μμ
5. μΉ μλΉμ€ μ¬μ©μλ ID, PW λ₯Ό μλ ₯ν  νμκ° μμ

### β κ΅¬κΈ λ‘κ·ΈμΈ κ΅¬ννκΈ°

1. κ΅¬κΈ ν΄λΌμ°λ νλ«νΌ νλ‘μ νΈ μμ±
2. API λ° μλΉμ€ β OAuth λμνλ©΄ μ€μ 
3. μ¬μ©μ μΈμ¦μ λ³΄ β OAuth ν΄λΌμ΄μΈνΈ ID λ§λ€κΈ°
4. passport-google-oauth20 μ°λ
5. `passport-google-oauth20` : passport-strategy μΈν°νμ΄μ€μ κ΅¬κΈ λ‘κ·ΈμΈ μ§ν©μ²΄(OAuth μΈμ¦μ κ΅¬ννκΈ° μν΄μλ μΈμ¦ μμ²­, λ°μ΄ν° μμ  λ±μ λ³΅μ‘ν μμ νμ), `passport-google-oauth2.0` μ μμ½κ² κ΅¬κΈ `OAuth 2.0` μ κ΅¬νν΄μ£Όλ ν¨ν€μ§

### β Nginx

1. μ΅κ·Ό μ κ· νλ‘μ νΈμμ κ°μ₯ λ§μ΄ μ±νλκ³  μλ μΉ μλ² μννΈμ¨μ΄(μΉ μλ² μννΈμ¨μ΄: `HTTP` μμ²­μ λ°μ νμΌμ΄λ νλ‘κ·Έλ¨ μ€ν κ²°κ³Όλ₯Ό `HTTP` μλ΅μΌλ‘ λ³΄λ΄μ£Όλ μννΈμ¨μ΄)
2. `Java - Tomcat`, `PHP - fastcgi` λ± λ€λ₯Έ μΈμ΄κ° `HTTP` μμ²­μ μ²λ¦¬λ₯Ό μν μμ‘΄μ±μ΄ μλ κ²μ λ°ν΄, `Node.js` λ κΈ°λ³Έμ μΌλ‘ `HTTP` μμ²­μ μμ νκ³ , μλ΅νλ κΈ°λ₯μ΄ μ΄λ―Έ μλ€. λ°λΌμ μΉ μλ² μννΈμ¨μ΄ μμ΄λ μ€μ€λ‘ λμν  μ μλ€. νμ§λ§, `node.js` λ¨λμΌλ‘ μ¬μ©νκ² λλ©΄ `HTTPS`, `λλ©μΈ μ°κ²°`, `static file caching` λ±μ κΈ°λ₯μ `production-level` μλΉμ€λ₯Ό κ΅¬μΆν  μλ μλ€. λ°λΌμ `node.js` μ λ¨μ μΉ μλ² μννΈμ¨μ΄λ₯Ό λΆμ¬μ μ¬μ©νλ€. `HTTP` μμ²­κ³Ό μλ΅μ node.jsμμ μμ²΄μ μΌλ‘ μ¬μ©μ΄ κ°λ₯νλ€.
3. `Nginx` μ `reverse-proxy` κΈ°λ₯μ μ¬μ©ν΄, `Node.js` μ `Nginix` λ₯Ό μ°κ²°ν  μ μλ€. `reverse-proxy` λ `HTTP` μμ²­μ λ€λ₯Έ μλ²μ μ λ¬νλ κΈ°λ₯μΈλ°, `Nginx` κ° μμ²­μ λ°μ, μ€μ λ λ΄μ©μ ν΄λΉνλ μμ²­λ§ `node.js` μ μ λ¬νλ€.

![](https://images.velog.io/images/abcd8637/post/9d61eb15-28cf-47e0-9c8e-5b6cdb9ea673/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-12-11%2016.38.13.png)

```js
// μΈλΆμμ μ¨ λͺ¨λ  μμ²­μ localhost:3000μΌλ‘ μ λ¬νλ μ€μ  νμΌ
// HTTPS, file cachingλ€μ μμμ Nginxμ μ€μ λ°©λ²μ μ°Έκ³ νκΈ°
server {
	listen 80;
	server_name www.example.com;

	location / {
		proxy_pass http://localhost:3000;
		proxy_http_version 1.1;
	}
}
```