## Validation
올바르지 않은 데이터를 걸러내고 보안을 유지하기 위해 데이터 검증은 여러 계층에 걸쳐서 적용. Client의 데이터는 조작이 쉬울 뿐더러 모든 데이터가 정상적인 방식으로 들어오는게 아니기 때문에,
Client Side 뿐만 아니라 Server Side에서도 데이터 유효성 검사를 해야한다.<br>
예를 들어 회원가입 서비스를 구현한다 치자. Email형식의 아이디를 받아야 하는데 일일히 코딩으로 구현하기는 쉽지 않다. 이런 경우엔 @Email을 사용하면 손쉽게 데이터 검증이 가능하다.

Spring boot의 Validation 종류에는 다음과 같이 있다.
@Null, @Notnull, @Positive, @Negative, @Future, @Past.... 다 적기에는 너무 많으니 필요할 때 마다 찾아보도록 하자.

Validation을 생성하여 Client와 Server에서 이중으로 안전하게 검증하는 방법을 적극 활용하자.
