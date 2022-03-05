# 용어정리
 
### 1. API(Application Programming Interface)
 
- 1-1. Application: 운영체제에서 실행되는 모든 소프트웨어(응용소프트웨어/어플리케이션)
- 1-2. Interface: 접점이 없는 서로 다른 두개의 시스템에서 소통/연결 하는 기술
- 참고사이트
  - [https://www.mulesoft.com/resources/api/what-is-an-api]
  - [https://ko.wikipedia.org/wiki/%EC%9D%91%EC%9A%A9_%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4]
  - [https://ko.wikipedia.org/wiki/%EC%9D%B8%ED%84%B0%ED%8E%98%EC%9D%B4%EC%8A%A4_(%EC%BB%B4%ED%93%A8%ED%8C%85)]
 
### 2. RESTApi (Representational State Transfer)
 
WWW와 같은 분산 하이퍼미디어 시스템을 위한 소프트웨어 아키텍처의 한 형식
웹 상의 자료를 HTTP위에서 SOAP이나 쿠키를 통한 세션 트랙킹같은 별도의 전송 계층 없이 전송하기 위한 아주 간단한 인터페이스로 이런 REST 원리를 따르는 시스템을 RESTful이라고 부르며 그렇게 만들어진 API를 RESTApi/RESTful Api라고 부른다.
 
- 참고사이트
  - [https://restfulapi.net/]
  - [https://ko.wikipedia.org/wiki/API]
  - [https://ko.wikipedia.org/wiki/REST]
 
### 3. HTTP(HypterText Transfter Protocol)
 
www상에서 정보를 주고받을 수 있는 프로토콜로 보통 HTML문서를 주고 받는데 사용되며 TCP 통신을 주로 사용하고 HTTP/3번부터는 UDP를 사용하며 80번을 기본 포트로 가진다.
 
- 참고사이트
  - [https://ko.wikipedia.org/wiki/HTTP]
  - [https://developer.mozilla.org/ko/docs/Web/HTTP/Overview]
 
### 4. WWW(World Wide Web)
 
인터넷에 연결된 컴퓨터를 통해 사람들이 정보를 공유할 수 있는 전 세계적인 정보 공간
 
- 참고사이트
  - [https://ko.wikipedia.org/wiki/%EC%9B%94%EB%93%9C_%EC%99%80%EC%9D%B4%EB%93%9C_%EC%9B%B9]
 
### 5. Protocol(프로토콜)
 
컴퓨터나 원거리 통신 장비 사이에서 메세지를 주고 받는 양식과 규칙의 체계로 신호 체계, 인증, 오류 감지 및 수정 기능 포함 할 수 있다.
프로토콜은 형식, 의미론, 통신의 동기 과정 등을 정의하기는하나 구현되는 방법은 독립적이다. 이 때문에 프로토콜은 하드웨어나 소프트웨어 또는 하드웨어와 소프트웨어 모두를 사용하여 구현되기도 한다.
 
- 참고사이트
  - [https://ko.wikipedia.org/wiki/%ED%86%B5%EC%8B%A0_%ED%94%84%EB%A1%9C%ED%86%A0%EC%BD%9C]
 
### 6. Axios
 
Nodejs와 브라우저를 위한 Promise 기반의 HTTP 클라이언트
 
- 참고사이트
  - [https://axios-http.com/docs/intro]
 
### 7. Promise
 
알려지지 않았을 수도 있는 값을 위한 대리자로 비동기 연산이 종료된 이후에 결과 값과 실패 사유를 처리하기 위한 처리기를 연결할 수 있다. 프로미스를 사용하면 비동기 메서드에서 마치 동기 메서드처럼 값을 반환할 수 있다. 다만 최종 결과를 반환하는 것이 아니고, 미래의 어떤 시점에 결과를 제공하겠다는 '약속(프로미스)'를 반환한다.
 
- 참고사이트
  - [https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Promise]
 
### 8. 비동기 Async(Asynchronous)
 
프로미스나 프로미스로 표시되는 유사한 데이터 구조에서 장기 실행 비동기 작업이 완료되기를 기다리는 동안 프로그램이 다른 코드를 실행할 수 있는 기회를 제공하기 위한 것으로 일부 언어(C#, C++, Python, F#, Hack, Julia, Dart, Kotlin, Rust, Nim, Javascript 등)에서 사용가능하다.
 
프로미스 같은 기능의 단점을 보완하기 위해 만들어졌으며(promise는 콜백지옥 코드가 작성될 수 있다.) 에러처리를 할 수 없기 때문에 try-catch() 문을 활용해야 한다.
 
- 참고사이트
  - [https://ko.wikipedia.org/wiki/Async/await ]
 
### 9. TCP(Transmission Control Protocol)
 
인터넷 프로토콜 스위트(IP)의 핵심 프로토콜 중 하나로 IP와 함께 TCP/IP라는 명칭으로도 널리 불린다. 근거리 통신망이나 인트라넷, 인터넷에 연결된 컴퓨터에서 실행되는 프로그램 간에 일련의 옥텟을 안정적으로, 순서대로, 에러없이 교환할 수 있게 한다.
 
- 참고사이트
  - [https://ko.wikipedia.org/wiki/%EC%A0%84%EC%86%A1_%EC%A0%9C%EC%96%B4_%ED%94%84%EB%A1%9C%ED%86%A0%EC%BD%9C]
 
### 10. 옥텟(octet)
컴퓨팅에서 8개의 비트가 한데 모인 것을 의미한다. 초기 컴퓨터들은 1바이트가 꼭 8비트만을 의미하지 않았으므로 8비트를 명확하게 정의하기 위해 옥텟이라는 용어를 사용하였다. 다만 8비트는 1바이트이기 때문에 요즘은 옥텟이라는 용어는 거의 사용하지 않는다.
 
### 11. 비트(Bit/Binary digit), 바이트(Byte)
11-1. 바이너리(Binary): 두 조각, 두 부분을 의미. 0과 1로 이루어진 이진법  
11-2. 비트(단위): 하나의 값을 가질 수 있는 단위(0이나 1)
11-3. 바이트(단위): 비트가 여러개 모인 것으로 8비트(1옥텟)를 1바이트로 부른다. 4비트는 니블(nibble)이며 두 바이트는 워드(word)를 의미한다. 컴퓨터 메모리의 통상적인 단위이며 거의 표준 값이다(C언어는 다름)
 
* 참고사이트
    * [https://ko.wikipedia.org/wiki/%EC%9D%B4%EC%A7%84_%ED%8C%8C%EC%9D%BC]
 
### 12. 워드(word)
컴퓨터 설계시 정해지는 메모리의 기본 단위