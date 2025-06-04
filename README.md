# JS_Operator  

## Operator(연산자)  
```
console.log(1 + 2)
console.log(5 - 7)
console.log(3 * 4)
console.log(10 / 2)
console.log(7 % 5)
```
데이터 : 피연산자  
기호  : 연산자  

부정연산자
```
console.log(!true)   // fasle
console.log(!false)  // true
```

비교연산자  
```
const a = 1
const b = 3
console.log (a > b) // false
console.log (a < b) // true
```

논리연산자  
```
const a = true
const b = false
if (a && b) {
    console.log('모두가 참')
}
if (a || b) {
    console.log('하나 이상이 참참')
}
```
```
console.log(true && false) //false
console.log(true || false) //true
console.log(null ?? true) //true
```
&& (And연산)은 왼쪽값이 flase면 왼쪽값 반환 true면 오른값 반환  
|| (Or연산)은 왼쪽값이 true면 왼쪽값 반환 false면 오른값 반환  
?? (Nullish연산)은 왼쪽값이 Null, undefined 일때만 오른값 반환  


삼항 연산자  
```
// 삼항
const a = 1

if (a < 2) {
    console.log('참')
} else {
    console.log('거짓')
}

// 삼항 연산자
console.log(a < 2 ? '참' : '거짓')
```
전개 연산자  
```
const a = [1, 2, 3]

console.log(a) // [1, 2, 3]
console.log(...a) // 1, 2, 3
```
  
## Assignment(할당)  
```
const a = 3
a = a + 2 // a += 2
console.log(a)
// (X)
```
const는 재할당이 불가능한 변수이다.  
재할당을 하기위해선 let을 써야한다. const -> let  
  
```
let a= 3
console.log(++a) //4
console.log(a)   //4
```
```
let a= 3
console.log(a++) //3
console.log(a)   //4
```

구조분해할당  
객체나 배열의 값을 변수로 쉽게 꺼내는 문법.  
```
const arr = [1, 2, 3];
const [a, b, c] = arr;

console.log(a); // 1
console.log(b); // 2
console.log(c); // 3
```
```
const arr = [1,2,3]
const [a, ...rest] = arr

console.log(a, rest) // 1, [2, 3]
```
