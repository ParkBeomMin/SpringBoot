# SpringBoot 기본 개념

제품 수준의 스프링 기반 애플리케이션을 만들 때 빠르고 쉽게 만들 수 있게 도와주는 것

사용자가 일일히 모든 설정을 직접 하지 않도록, 많이 쓰이는 설정을 제공해준다.(필요시 설정들을 직접 바꿔 줄 수 있다.)

code generation이 없고, XML도 사용하지 않는다.

java 8 이상부터 사용가능하다.

## Controller

- 라우팅 하는 곳
- @RestController 어노테이션을 붙여준다.
- @RequestMapping("/beom/*") 어노테이션으로 상위 경로를 지정해줌
- @GetMapping("/test") 어노테이션으로 endpoint 지정

```java
@RestController
@RequestMapping("/beom/*")
public class BeomController {
    @GetMapping("/test") // localhost:8080/beom/test
    public String doTest() {
        return new BeomService().doBeom();
    }
}
```


## Service

- 비즈니스 로직이 작성되는 곳
- @Service 어노테이션을 붙여준다.

```java
@Service("beomService")
public class BeomService {
    private String result = "test";
    public String doBeom() {
        return new Gson().toJson(this);
    }
}
```

## Security

- 노드의 미들웨어 같은 느낌

## 참고

https://velog.io/@max9106/series/Spring-Boot-%EC%8A%A4%ED%94%84%EB%A7%81-%EB%B6%80%ED%8A%B8-%EA%B8%B0%EC%B4%88