연산자, 문장, Object, Number, Math, String
Template, RegExp, Array, Function, Iterator, Generator, Symbol
Map, WeakMap, Set, WeakSet, Class, Reflect, Proxy
ArrayBuffer, TypedArray, DataView, Promise, Module, Babel & Webpack
ES6와 연관된 Node.js, XMLHttpRequest, Workers, Canvas 부분

연산자,
문장,
Object,
Number,
Math,
String

Template,
RegExp,
Array,
Function,
Iterator,
Generator,
Symbol

Map,
WeakMap,
Set,
WeakSet,
Class,
Reflect,
Proxy

ArrayBuffer,
TypedArray,
DataView,
Promise,
Module,
Babel & Webpack

ES6와 연관된 Node.js,
XMLHttpRequest,
Workers,
Canvas 부분

```
* arrow function

- ...rest // arguments 대체 권장
- function내 scope 유의해야 함
- 자동 return; 1줄이거나 소괄호로 둘러쌓인 JSON객체
- new 연산자로 인스턴스 생성 불가; prototype, constructor가 없음, 생성자가 없는 특별한 형태의 함수;
- this;
- // ES5: setTimeout() 의 경우 this를 window객체 참조
- // ES6: arrow function 의 경우 스코프를 유지할 수 있음. setTimeout() 내에서 this 참조
- 기존 function 키워드 함수와 비교해서 선택 사용

```

```
* Iteration_protocols
- Iteration
- next()
- 
```

## spread
```
- obect는 프로퍼티만 변경 할 수 있음.
```

## array-like
```
- arguments // array-like
- ...rest // array obejct
```

## Destructuring assignment
```
* Array destructuring
* Object destructuring
- The ( .. ) around the assignment statement...
- let {nine, plus: {ten}} = {nine:9, plus: {ten: 10}} // plus: 경로 역할
- Setting a function parameter's default value
```


## Object.defineProperty()
```
configureable
enumerable
value
writable
get
set
```

## Object initializer: shorthand method names
```
vs ES5
* ES5
get: function() {return "book"}
* ES6
get getBook() {return "book"}
```

## Object initializer: computed property names
```
```

## default
```
let {a, b = 5} = {a: 10, b: 20}
let {a, b = a + 1, c = b + 1} = {a: 1}
```

## for...of
```
* 프로퍼티 값이 설정됨
* Difference between for...of and for...in
- 프로토타입에 정의된 프로퍼티는 제외시킴
- Object는 iterable이 아니므로 사용불가 // Ojbect.keys로 활용하여 사용
```

## prototype
```
valueOf
toString

최신동향; 메서드, 함수 prototype에 연결 되지않고 Object에 바로 연결(ES6)
```

## Object.is()
```
* https://dorey.github.io/JavaScript-Equality-Table/
* NaN 도 하나의 값임
- NaN === NaN // false
- Object.is(NaN, NaN) // true

```

## Object.assign()
```
* property 작성 순서 주의
- property, get property vs get property, property
```

## Object.setPrototypeOf()
```
* __proto__ 에 설정하는 목적
* prototype vs __proto__

```

## Object.prototype.__proto__
```
```

## Number
```
* IEEE 754
- double precision floating point format
- 64bit(8byte) 유동 소수점 형태로 수를 표시
- 
- 
```

## Number.MAX_SAFE_INTEGER, Number.MIN_SAFE_INTEGER 
```
```

## Number.EPSILON
```
0.1 + 0.2 === 0.3 // false
Number.EPSILON = true;
0.1 + 0.2 === 0.3 // true

// 기존의 해결방법
소수 -> 정수 변환 and 계산 -> 소수 (정수에서는 문제가 없음)
```

## Number.isNaN()
```
Number.isNaN("ABC");
isNaN("ABC");
```

## Number.isInteger()
```
```

## Number.isSafeInteger()
```
```

## Number.isFinite()
```
```

## Math.log10(), Math.log2(), Math.log1p(), Math.expm1(), Math.cosh(), Math.sinh(), Math.tanh(), Math.acosh(), Math.asinh(), Math.atanh(), Math.hypot(): 제곱근, Math.trunc(): 소수를 제외한 정수 반환, Math.sign(), Math.cbrt(): 세제곱근
```
```

## Math.imul()
```
* 32bit
* Emscripten
```

## Unicode code point escapes
```
\u{XXXXXX}
```

## Surrogate pair
```
* ES5 호환
* http://unicode-table.com/en/
- http://unicode-table.com/en/1F418/
* \{?}\{?}
```

## String.fromCodePoint()
```
* binary 데이터
```

## String.prototype.codePointAt()
```
```

## String.prototype.includes() 
```
* 2번째 파라미터 인덱스 제한 // .incldues('a', 5)
* 정규표현식 사용불가
```

## String.prototype.startsWith(), String.prototype.endsWith()
```
```

## String.prototype.repeat()
```
```

## String.prototype.normalize()
```
* 유니코드 정규화
let ja = "ㄱ".charCodeAt(0); // 초성, 종성 등.. 조합에 따라 유니코드 값이 달라짐
let mo = "ㅏ".charCodeAt(0);
let jamo = '\u3131\u314F';
let result = jamo.normalize('NFC');
```

## String.raw()
```
Template literals
```

## 
```
```

## 
```
```

## 
```
```

## 
```
```

## 
```
```

## 
```
```

## 
```
```

## 
```
```

## 
```
```

