## Root URL이란?
> * ```http://localhost:8080```처럼 도메인명과 포트 뒤에 아무것도 붙이지 않은 URL을 말한다.
```Java
package com.example.demo;

import org.springframework.stereotype.Controller;
import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.ResponseBody;

@Controller
public class MainController {

	
	@RequestMapping("/sbb")
	@ResponseBody
	public String index() {
		return "김도선도 바보";
	}
	
	@RequestMapping("/")
	public String root() {
		return "redirect:/question/list"; // 완전 새로운 해당 URL로요청
//		 return "forward:/question/list"; // 기존 요청 값 유지하고 URL로 전환
	}
	
	
}

```
