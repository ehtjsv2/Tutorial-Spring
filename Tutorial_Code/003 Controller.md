## 배운점
1. 매핑된 메소드에서 return 한 값을 페이지에 띄어준다.

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
}

```
