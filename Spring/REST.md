## REST(Representational State Transfer : 자원의 상태 전달)

1. Client, Server: 클라이언트와 서버가 독립적으로 분리 되어 있어야 한다.
2. Stateless: 요청에 대해서 클라이언트의 상태를 서버에 저장하지 않는다.
3. Cache: 클라이언트는 서버의 응답을 Cache할 수 있어야 한다.
4. 계층화: 서버와 클라이언트 사이에, 방화벽, 게이트웨이, Proxy등 다양한 계층 형태로 구성이 가능해야 하며, 이를 확장 할 수 있어야 한다.
5. 인터페이스 일관성: 인터페이스의 일관성을 지키고, 아키텍처를 단순화시켜 작은 단위로 분리하여 클라이언트와 서버가 독립적으로 개선 될 수 있어야 한다.
6. Code on Demand(Optional): 특정한 기능을 서버로부터 클라이언트가 전달받아 코드를 실행 할 수 있어야 한다.

<br>

#### 하기 인터페이스 일관성이 잘 지켰는지에 따라, REST가 잘 지켜졌는지 확인할 수 있다.
* 자원의 식별 : 웹 기반의 REST에서는 리소스 접근할 떄 URI를 사용.
* 메세지를 통한 리소스 조작: Web에서는 다양한 방식으로 데이터를 전달. ex)XML, JSON
* 자기서술적 메세지: 요청하는 데이터가 어떻게 처리되어져야 하는지 충분한 데이터를 포함 할 수 있어야 한다.
* Application상태에 대한 엔진으로써 하이퍼미디어
이러한 조건들을 잘 갖춰야 RESTFul하다고 생각한다.
