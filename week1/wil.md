# 백엔드 1주차

### 웹이란?

- 인터넷: 전 세계 컴퓨터와 기기를 연결하는 **거대한 글로벌 네트워크**
- 웹: 인터넷 위에서 동작하는 서비스 중 하나, 인터넷에 연결된 전 세계 사용자들이 서로의 정보를 공유할 수 있는 장소.

### 클라이언트와 서버 모델: 컴퓨터와 컴퓨터가 통신하는 구조

- 클라이언트(Client): 요청을 보내고, 서버의 응답 결과를 받아 사용
- 서버(Server): 클라이언트의 요청을 받아 처리하고, 그에 대한 응답을 반환

## URL : **U**niform **R**esource **L**ocator

웹 상에서 특정 자원(웹페이지, 문서, 이미지 등)의 위치를 나타내는 주소

#### http://www.example.com:5883/category/food.html?topic=pizza&size=large

##### Host

- www.example.com 부분: 리소스가 위치한 서버의 IP주소 혹은 도메인

##### Port

- :5883 부분: 서버의 특정 네트워크 포트 번호(일반적으로 생략)

##### Path

- /category/food.html 부분: 서버 내에서 원하는 리소스의 경로

##### Query

- ?topic=pizza&size=large 부분: 서버에 추가적인 정보를 보내는 파라미터로, ? 뒤에 key-value 형식으로 나열

##### Scheme(protocol)

- http 부분: 컴퓨터와 같은 장치들 사이에서 데이터를 주고 받는 방식, 통신하기 위한 규칙

### HTTP : **H**yper**T**ext **T**ransper **P**rotocol

- **무상태성(Stateless)**: 서버는 클라이언트의 이전 요청을 저장하지 않고, 매 요청을 독립적으로 처리
- **비연결성(Connectionless)**: 클라이언트가 요청을 보내고 응답을 받은 후 서버와 연결을 유지하지 않음

### HTTP 주요 메서드

- Get : 리소스를 **조회**
- Post : 리소스를 **추가, 등록**
- Put : 리소스를 **교체**, 없으면 **새로 생성**
- Patch : 리소스의 **일부를 수정**
- Delete : 리소스를 **삭제**

## 프론트엔드와 백엔드

프론트엔드(Frontend): 사용자의 눈에 보이는 부분을 다루는 것

- ui 개발
  백엔드(Backend): 보이지 않는 부분을 다루는 것
- 실제 동작 처리, 데이터 저장. 관리

#### 데이터베이스(DB)

- 데이터를 체계적으로 모아둔 저장소
- 데이터베이스 관리시스템(DBMS)으로 데이터베이스를 관리, 조작

* 데이터 중복 해결, 독립성 확보, 무결성 유지

### API : **A**pplication **P**rogramming **I**nterface

한 프로그램이 다른 프로그램의 기능이나 데이터를 사용할 수 있도록 미리 정해 놓은 약속

## REST : **R**epresentational **S**tate **T**ransfer

### REST 구성요소

1. 자원(resource)- URL: 모든 자원은 고유한 ID를 가짐
2. 행위(verb) - Method: 자원을 조작하기 위해 HTTP Method를 사용
3. 표현(representation) : 서버와 클라이언트가 데이터를 주고 받는 형식으로 JSON 형식이 일반적
