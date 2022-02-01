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

## Physical Layer
컴퓨터와 네트워크 장비를 연결하고 컴퓨터와 네트워크 장비 간의 전송되는 데이터를 전기 신호로 변환하는 계층. 랜 카드를 이용하여 0과 1을 전기 신호로 변환한다.

## Data Link Layer
네트워크 장비 간에 신호를 주고받는 규칙을 정하는 계층, 일반적으로 가장 많이 사용되는 규칙이 이더넷.
이더넷 헤더 = 목적지 MAC 주소(6바이트) + 출발지 MAC 주소(6바이트) + 유형(2바이트)
데이터를 감싸는 캡슐화를 통해 정보를 파악하고 보낼때는 다시 역 캡슐화를 한다.
