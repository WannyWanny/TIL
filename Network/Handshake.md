# TCP 3-way(4-way) Handshake란?
TCP/IP 프로토콜을 이용해서 통신을 하는 응용프로그램들이 데이터를 전송하기 전에 정확한 전송을 보장하기 위해 
상대방 컴퓨터와 사전에 세션을 수립하는 과정

## 3-way Handshake(연결성립)
![3-way](https://github.com/WannyWanny/TIL/blob/master/Image/3-way.png)
<ol>
  <li>클라이언트는 서버에 접속을 요청하는 SYN(a)를 보낸다.</li>
  <li>서버는 클라이언트의 요청인 SYN(a)를 받고 클라이언트에게 요청을 수락한다는 ACK(a+1)와 SYN(b)이 설정된 패킷을 발송한다.</li>
  <li>클라이언트는 서버의 수락 응답인 ACK(a+1)와 SYN(b)를 받고 ACK(b+1)을 서버로 보내면 연결이 성립 된다.</li>
</ol>

## 4-way Handshake(연결해제)
![4-way](https://github.com/WannyWanny/TIL/blob/master/Image/4-way.png)
<ol>
  <li>클라이언트가 서버를 종료하겠다는 FIN플래그를 전송한다.</li>
  <li>서버는 클라이언트의 요청(FIN)을 받고 응답하는 확인 메세지로 ACK를 보낸다. 그리고 나서는 데이터를 모두 보낼때 까지 잠시 TIME OUT이 된다.</li>
  <li>데이터를 모두 보내고 통신이 끝났으면 연결이 종료되었다고 클라이언트에게 FIN을 보낸다.</li>
  <li>클라이언트는 FIN 메세지를 확인했다는 ACK메세지를 보낸다.</li>
  <li>클라이언트의 ACK메세지를 받은 서버는 소켓 연결을 close한다.</li>
  <li>클라이언트는 아직 서버로부터 받지 못한 데이터가 있을 것을 대비해 일정 시간 동안 세션을 남겨놓고 잉여 패킷을 기다리는 과정을 거친다.(TIME_WAIT)</li>
</ol>
