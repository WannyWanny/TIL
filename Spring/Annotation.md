# 각종 Annotation 정리
> Spring Framework를 사용하며 만날 수많은 Annotation들을 기록하기 위한 글입니다.
----------------------------------------------

### @RequestBody, @ResponseBody 
HTTP 비동기 통신을 하기위해 필요합니다. 클라이언트와 서버는 데이터를 끊임없이 주고 받는데, 요청(request)과 응답(response) 메세지를 처리하기 위하여 사용합니다. 대표적으로는 JSON방식으로
많이 사용하여 클라이언트와 서버가 끊임없이 데이터를 주고받습니다. <br>즉 , @RequestBody를 사용하여 HTTP 요청 본문에 담긴 값들을 자바 객체로 변환시켜 객체에 저장하고, @ResponseBody를 사용하여 자바 
객체를 HTTP 응답 본문의 객체로 변환하여 클라이언트로 전송하는 역할을 합니다.

### @Test
말그대로 test하기 위해 붙인다. main메소드처럼 개별적으로 실행할 수 있다.
- @Disabled: 특정 메소드가 @Deprecated되었거나 테스트에 확실히 Passed가 되는 경우가 아닐때 실행되지 않도록 처리하는 부분.
- @BeforeAll, @AfterAll: 클래스에 존재하는 모든 메소드를 실행한다고 할때, 메소드가 시작하기전과 끝난후에 실행되는 단위들
- @BeforeEach, @AfterEach: 각각의 메소드가 실행 전, 실행 후에 호출되어 처리 되는것들. 

### @AutoWired
스프링 컨테이너 안에 존재하는 Bean을 자동으로 주입해준다.

### @PathVariabl
주소뒤에 변수명을 매핑하기 위함. ex) /put/{userId}로 받을 경우 parameter에 userId변수가 있을 텐데 앞에 해당 어노테이션을 붙인다.<br>
@PathVariable(name = )으로도 사용이 가능함. 

### @Configuration
스프링 IoC Container에게 해당 클래스를 Bean구성 Class임을 선언한다. <br>

### @Component, @Bean
둘다 IoC Container에게 Bean을 등록하도록 메타데이터를 기입하는 어노테이션. 하지만 둘의 용도는 다르다.
@Bean의 경우 개발자가 직접 제어가 불가능한 외부 라이브러리등을 Bean으로 만들려고 할 때 사용.<br>
@Componenet는 개발자가 직접 작성한 Class를 Bean으로 등록하기 위해 사용.
