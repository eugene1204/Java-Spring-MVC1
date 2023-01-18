# Java-Spring-MVC1

# 2. 서블릿 
## Hello 서블릿
스프링 부트 환경에서 서블릿 등록하고 사용해보자.
- 참고 : 서블릿은 톰캣 같은 웹 애플리케이션 서버를 직접 설치하고,그 위에 서블릿 코드를 클래스 파일로 빌드해서
  올린 다음, 톰캣 서버를 실행하면 된다. 하지만 이 과정은 매우 번거롭다. 스프링 부트는 톰캣 서버를 내장하고 있으므로, 톰캣 서버 설치 없이 편리하게 서블릿 코드를 실행할 수
있다.

### 스프링 부트 서블릿 환경 구성
```@ServletComponentScan```
스프링 부트는 서블릿을 직접 등록해서 사용할 수 있도록 ```@ServletComponentScan``` 을 지원한다. 다음과 같이 추가하자.

#### hello.servlet.ServletApplication
```
```


### 서블릿 등록하기
처음으로 실제 동작하는 서블릿 코드를 등록해보자. 

#### hello.servlet.basic.HelloServlet
```
```

- @WebServlet 서블릿 애노테이션 
  - name: 서블릿 이름 
  - urlPatterns: URL 매핑

HTTP 요청을 통해 매핑된 URL이 호출되면 서블릿 컨테이너는 다음 메서드를 실행한다.
protected void service(HttpServletRequest request, HttpServletResponse response)

- 웹 브라우저 실행
  - http://localhost:8080/hello?username=world
  - 결과: hello world 

- 콘솔 실행결과
```
```

# Java-Spring-MVC1
