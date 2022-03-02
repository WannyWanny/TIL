# 변수 선언 방식
ES6이전에는 `var` 선언을 하였으나 큰 단점이 있다.
```
var name = 'wanny'
console.log(name)       //wanny

var name = 'kim'
console.log(name)       //kim
```
변수를 한번 더 선언했음에도 불구하고 에러가 나오지도 않고 각기 다른 값을 출력한다.
이를 보완하기 위해선 ES6에선 `let`과 `const`를 사용한다.

위와 같은 방식으로 `const`를 할 경우, //Uncaught SyntaxError: Identifier 'name' has already been declared를 출력한다.

`let`과 `const`의 차이점은 `immutable`여부이다. 즉, `let`은 변수에 재할당이 가능하지만 `const`는 재선언, 재할당이 불가능하다.

호이스팅이란 개념도 등장한다. 스코프내에서 선언을 해야 변수를 참조할수 있다는 말이다. 대단히 당연한 행위이다.

## 결론
어떤 상황에서 무엇을 써야할까? 답은 간단하다.<p>
변수 선언은 기본적으로 `const`를 사용하고 재할당이 필요한 경우에 한정해 `let`를 사용하면 된다.
