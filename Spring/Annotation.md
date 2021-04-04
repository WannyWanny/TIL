# 각종 Annotation 정리
> Spring Framework를 사용하며 만날 수많은 Annotation들을 기록하기 위한 글입니다.
----------------------------------------------

# @RequestBody, @ResponseBody 
<br> HTTP 비동기 통신을 하기위해 필요합니다. 클라이언트와 서버는 데이터를 끊임없이 주고 받는데, 요청(request)과 응답(response) 메세지를 처리하기 위하여 사용합니다. 대표적으로는 JSON방식으로
많이 사용하여 클라이언트와 서버가 끊임없이 데이터를 주고받습니다. <br>즉 , @RequestBody를 사용하여 HTTP 요청 본문에 담긴 값들을 자바 객체로 변환시켜 객체에 저장하고, @ResponseBody를 사용하여 자바 
객체를 HTTP 응답 본문의 객체로 변환하여 클라이언트로 전송하는 역할을 합니다.

# @Test

<br> 말그대로 test하기 위해 붙인다. main메소드처럼 개별적으로 실행할 수 있다.
- @Disabled: 특정 메소드가 @Deprecated되었거나 테스트에 확실히 Passed가 되는 경우가 아닐때 실행되지 않도록 처리하는 부분.
- @BeforeAll, @AfterAll: 클래스에 존재하는 모든 메소드를 실행한다고 할때, 메소드가 시작하기전과 끝난후에 실행되는 단위들
- @BeforeEach, @AfterEach: 각각의 메소드가 실행 전, 실행 후에 호출되어 처리 되는것들. 
