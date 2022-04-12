## RestTemplate
REST API 호출 이후 응답을 받을 때 까지 기다리는 동기 방식. <br>
스프링에서 제공하는 http 통신에 유용하게 쓸 수 있는 템플릿. <br>
HTTP 서버와의 통신을 단순화 하고 RESTful하다.

### 동작 원리
1. 어플리케이션이 RestTemplate를 생성하고 URI, HTTP 메소드 등의 헤더를 담아 요청
2. RestTemplate는 HttpMessageConverter를 사용하여 RequestEntity를 요청 메세지로 변환
3. RestTemplate는 ClientHttpRequestFactory로 부터 ClientHttpRequest를 가져와서 요청을 보냄
4. ClientHttpRequest는 요청메세지를 만들어 HTTP 프로토콜을 통해 서버와 통신
5. RestTemplate는 ResponseErrorHandler로 오류를 확인하고 있다면 처리로직을 태움
6. ResponseErrorHandler는 오류가 있다면 ClientHttpResponse에서 응답데이터를 가져와서 처리
7. RestTemplate는 HttpMessageConverter를 이용해서 응답메세지를 java object로 변환
8. 
