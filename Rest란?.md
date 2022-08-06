> https://gmlwjd9405.github.io/2018/09/21/rest-and-restful.html 참조

## ```Rest```란?
> * ```Representational State Transfer```의 약자
> * ```상태(정보) 전달```
>   * 데이터가 요청되어지는 시점에서 자원의 상태(정보)를 전달한다.
>   * JSON 혹은 XML를 통해 데이터를 주고 받는 것이 일반적이다.
> * REST는 ```웹의 기존기술```과 ```HTTP 프로토콜```을 그대로 활용하기 때문에 웹의 장점을 최대한 활용 가능한 아키텍처 스타일이다.

## 구체적 개념
> * ```HTTP URI(Uniform Resource Identifier)```를 통해 ```자원(Resource)```을 명시하고, ```HTTP Method(POST, GET, PUT, DELETE)```를 통해 해당 자원에 대한 ```CRUD Operation```을 적용하는 것을 의미한다.
> * ```HTTP 요청 Method```
>   * 주어진 리소스에 수행하길 원하는 행동을 의미, ```HTTP 동사```라고도 불림
> * ```CRUD Operation```
>   * Create: 생성(```POST```)
>   * Read : 조회(```GET```)
>   * Update : 수정(```PUT```)
>   * Delete : 삭제(```DELETE```)
>   * HEAD : header정보 조회(```HEAD```)

## REST 특징
> * ```Server-Client 구조```(server-자원보유, client-자원요청)
>   * REST Sever: API제공, 비즈니스 로직처리 및 저장
>   * Client: 사용자 인증, context(세션, 로그인정보) 등을 직접 관리
> * ```Stateless(무상태)```
>   * HTTP 프로토콜이 Stateless Protocol이므로.
>   * Client의 context를 Server에 저장하지않는다.-> 구현 단순해짐
>   * Server는 각각의 요청을 완전히 별개의 것으로 인식하고 처리
>     * 각 API 서버는 Client의 요청만을 단순처리.
>     * 즉, 이전 요청이 다음 요청의 처리에 연관되어서는 안됨.
>     * SErver의 처리방식에 일관성을 부여, 부담 줄어듬, 서비스 자유도 높아짐
> * ```Cacheable(캐시 처리 가능)```
> * 등등..

## ```RESTful```이란?
> * ```RESTful```은 일반적으로 REST라는 아키텍처를 구현하는 웹서비스를 나타내기 위해 사용되는 용어.
>   * ```REST API'``를 제공하는 웹서비스를 'RESTful' 하다고 할 수 있다.
>   * ```REST 원리를 따르는 시스템```은 RESTful 이란 용어로 지칭

## RESTful 의 목적
> * 이해하기 쉽고 사용하기 쉬운 REST API 만드는 것.

### RESTful 하지 못한 경우
> * CRUD 기능을 모두 POST로만 처리하는 API
> * route에 resource, id 외의 정보가 들어가는 경우
