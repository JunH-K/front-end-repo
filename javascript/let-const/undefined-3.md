# 이터레이션

데이터 컬렉션을 순회하기 위한 프로토콜이다. 이터레이션을 준수한 객체는 for..of로 순회할 수 있다. 이터레이션 프로토콜은 이터러블, 이터레이터가 있다.

> 이터러블

이터러블 프로토콜을 준수한 객체를 이터러블이라하고 \[Symbol.iterator\] 메소드를 구현하거나 상속받 객체를 이터러블이라고 한다. 배열은 \[Symbol.iterator\] 메소드를 소유한다. 배열은 이터러블이다. 고로for..of 순회가 가능하다.

```javascript
const arr = [1, 2, 3];
console.log(Symbol.iterator in arr); //true

for (let value of arr) {
  console.log(value);
}

```

