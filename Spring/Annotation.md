# 각종 Annotation 정리
> Spring Framework를 사용하며 만날 수많은 Annotation들을 기록하기 위한 글입니다.
----------------------------------------------

# @RequestBody, @ResponseBody 
<br> HTTP 비동기 통신을 하기위해 필요합니다. 클라이언트와 서버는 데이터를 끊임없이 주고 받는데, 요청(request)과 응답(response) 메세지를 처리하기 위하여 사용합니다. 대표적으로는 JSON방식으로
많이 사용하여 클라이언트와 서버가 끊임없이 데이터를 주고받습니다. <br>즉 , @RequestBody를 사용하여 HTTP 요청 본문에 담긴 값들을 자바 객체로 변환시켜 객체에 저장하고, @ResponseBody를 사용하여 자바 
객체를 HTTP 응답 본문의 객체로 변환하여 클라이언트로 전송하는 역할을 합니다.
