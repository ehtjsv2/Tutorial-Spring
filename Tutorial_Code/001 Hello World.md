### 배운점
1. localhost 와 ip 와 포트번호
  * localhost는 본인의 컴퓨터를 가리키는 호스트네임/ 도메인이다.
  * 도메인 형태가 아닌 본인의 컴퓨터 ip는 127.0.0.1 이다. 자신을 가리킨다해서 루프백 주소라고도 불린다.
  * port번호는 본인의 ip는 하나인데 여러가지 요청이 동시에 오면 혼동이 올 수 밖에없다. 그런것을 방지하기위해 각각의 프로세스, 프로그램은 포트번호를 갖게된다. 즉 프로그램을 지정하기위한 번호이다.
2. 애너테이션


```Java
package com.example.demo;

import org.springframework.stereotype.Controller;
import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.ResponseBody;


@Controller // 이 클래스가 컨트롤러라는 것을 알려주는 애너테이션
public class HelloController {
	@RequestMapping("/hello") // hello를 요청받으면 reponsebody를 호출하는 애너테이션
	@ResponseBody // requestMapping의 응답 애너테이션
	public String hello() {
		return "Hello World";
	}
	
}
```
