> https://gmlwjd9405.github.io/2018/09/21/rest-and-restful.html 참조

## ```Rest```란?
> * ```Representational State Transfer```의 약자
> * ```상태(정보) 전달```
>   * 데이터가 요청되어지는 시점에서 자원의 상태(정보)를 전달한다.
>   * JSON 혹은 XML를 통해 데이터를 주고 받는 것이 일반적이다.
> * REST는 ```웹의 기존기술```과 ```HTTP 프로토콜```을 그대로 활용하기 때문에 웹의 장점을 최대한 활용 가능한 아키텍처 스타일이다.

## 구체적 개념
> * ```HTTP URI(Uniform Resource Identifier)```를 통해 ```자원(Resource)```을 명시하고, ```HTTP Method(POST, GET, PUT, DELETE)```를 통해 해당 자원에 대한 ```CRUD Operation```을 적용하는 것을 의미한다.
> * HTTP 요청 MEthod
>   * 주어진 리소스에 수행하길 원하는 행동을 의미, ```HTTP 동사```라고도 불림
> * CRUD Operation
>   * Create: 생성(POST)
>   * Read : 조회(GET)
>   * Update : 수정(PUT)
>   * Delete : 삭제(DELETE)
>   * HEAD : header정보 조회(HEAD)

