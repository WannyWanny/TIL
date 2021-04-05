# Optional
개발할 때 가장 많이 발생하는 예외가 NPE(NullPoineException)이다. NPE를 피하기 위해서는 null을 검사하는 로직을 추가해야 하는데 
변수도 많아지고 로직도 복잡해지는 번거로움이 있다. 그렇기 때문에 Optinal< T >을 사용한다.
null이 올 수 있는 값을 감싸는 Wrapper클래스로, 참조하더라도 NPE가 발생하지 않도록 도와준다.

### Optional의 orElse와 orElseGet의 차이
------------------------------------------------------------------------------------------------------------
optional API의 단말 연산에는 orElse와 orElseGet 함수가 있다. 비슷해 보이는 두 함수에는 아래와 같은 차이다. 있다.
- orElse: null이든 아니든 항상 호출된다.
- orElseGet: null일때만 호출된다.
