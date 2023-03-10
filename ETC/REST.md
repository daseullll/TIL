## REST(Representational State Transfer)

<br>

- **REST**이란, 표현 상태를 전달하는 것으로 일종의 HTTP의 디자인패턴이다.
- **HTTP URI**를 통해 자원을 명시하고, HTTP Method(POST, GET, PUT, DELETE)를 통해 해당 자원에 대한 CRUD를 적용하는 것을 의미한다.<br><br>

### REST를 사용하는 이유

- 어플리테이션을 분리 및 통합할 수 있으며, 모든 디바이스 통신이 가능하다.
  <br><br>

### REST의 제약 조건

- 클라이언트-서버
  - 클라이언트와 서버의 기능은 완벽히 분리되어야 한다.
- 무상태(Stateless)
  - REST는 HTTP의 특성을 이용하기 때문에 무상태성을 갖는다. 즉 서버에서 어떤 작업을 하기위해 상태 정보를 기억할 필요가 없고 들어온 요청에 대해 처리만 해주면 되기때문에 구현이 쉽고 단순해진다.
- 캐시 처리 기능
  - 클라이언트는 응답을 캐싱할 수 있어야 한다. -> 클라이언트가 같은 자료를 중복 욫ㅇ하는 것을 막아 서버의 부담을 줄여줄 수 있다.
- 서버와 클라이언트 사이에 캐시 서버나 로드 밸런서 드으이 중간 서버를 둘 수 있다.
  <br><br>

### REST API

- **REST API**는 REST 기반으로 서비스 API를 구현한 것이다.
- 사내 시스템들도 REST 기반으로 시스템을 분산해 확장성과 재사용성을 높여 유지보수 및 운용을 편리하게 할 수 있다.
- REST는 HTTP 표준을 기반으로 구현하므로, HTTP를 지원하는 프로그램 언어로 클라이언트, 서버를 구현할 수 있다.
  <BR>

### HTTP 메소드

- 클라이언트가 요청을 보낼 때 해당 요청의 목적이 뭔지 HTTP 메소드를 통해 명시한다.
- **GET** : 서버의 리소스를 조회하고자 할 때
- **POST** : 서버의 리소스를 생성하고자 할 때
- **DELETE** : 서버의 리소스를 삭제할 때
- **PUT** : 서버의 리소스를 수정하고자 할 때
- **PATCH** : 서버의 리소스의 부분만을 수정할 때

### RESTful 이란

- RESTful은 일반적으로 REST라는 아키텍처를 구현하는 웹 서비스를 나타내기 위해 사용되는 용어이다.
- REST API를 제공하는 웹 서비스를 RESTful하다고 할 수 있다.
- 이해하기 쉽고 사용하기 쉬운 REST API를 만드는 것이다.
- RESTful 하지 못한 경우
  - CRUD 기능을 모두 POST로만 처리하는 API
  - route에 resource, id 외의 정보가 들어가는 경우
