# OSI 7Layers

|계층|이름|설명|
|--|-------------|----------------|
|7|Application Layer|Human-computer interaction layer, where applications can access the network service|
|6|Presentation Layer|Ensure that data is in a usable format and is where adta encryption occurs|
|5|Session Layer|Maintains connections and is responstible for controlling ports and sessions|
|4|Transoport Layer|Transmits data using transmission protocols incliding TCP and UDP|
|3|Network Layer|Decides which physical path the data will take|
|2|Data Link Layer|Defines the format of data on the network|
|1|Physical Layer|Transmits raw bit stream over the physical medium|

응용 계층(7, 6, 5), 전송계층(4), 네트워크 계층(3), 물리 계층(2, 1)

## 물리 계층
컴퓨터와 네트워크 장비를 연결하고 컴퓨터와 네트워크 장비 간의 전송되는 데이터를 전기 신호로 변환하는 계층. 랜 카드를 이용하여 0과 1을 전기 신호로 변환한다.

## 데이터 링크 계층
네트워크 장비 간에 신호를 주고받는 규칙을 정하는 계층, 일반적으로 가장 많이 사용되는 규칙이 이더넷.
이더넷 헤더 = 목적지 MAC 주소(6바이트) + 출발지 MAC 주소(6바이트) + 유형(2바이트)
데이터를 감싸는 캡슐화를 통해 정보를 파악하고 보낼때는 다시 역 캡슐화를 한다.

## 네트워크 계층
네트워크 간의 통신을 가능하게 하는 것이 네트워크 계층의 역할. 이 계층을 이용하려면 라우터라는 네트워크 장비 필요.
IPv4로 43억개의 IP를 제공해왔으나 부족해서 340간개의 IP를 제공하는 IPv6이 생겼다.

A클래스 = 네트워크ID(8비트) + 호스트ID(24비트)<br>
B클래스 = 네트워크ID(16비트) + 호스트ID(16비트)<br>
C클래스 = 네트워크ID(24비트) + 호스트ID(8비트)

클래스의 대규모 네트워크를 작은 네트워크로 분할하여 브로드캐스트로 전송되는 패킷의 범위를 좁힐 수 있으므로 효과적인 IP사용이 가능하다. <br>이처럼 네트워크를 분할하는 것을 서브넷팅이라 하고 분할된 네트워크를 서브넷이라 한다.
서브넷 마스크는 네트워크 주소와 호스트 주소를 식별하는 값.

## 전송 계층
목적지에 신뢰할 수 있는 데이터를 전달하기 위해 필요. 전송된 데이터의 목적지가 어떤 애플리케이션인지 식별하는 기능. 
연결형 통신 프로토콜에는 TCP가, 비연결형 통신에는 UDP가 사용된다.

## 응용 계층
클라이언트에서 사용하는 애플리케이션과 서버에서 사용하는 서버 프로그램 간의 통신은 응용 계층의 프로토콜을 사용
