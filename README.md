### 패키지 구조
```
- aop : AOP로 중복 거래 방지 락을 걸때 사용될 어노테이션을 위치 시킴
- config : redis 관련 설정 및 클라이언트 빈 등록, JPA 관련 설정 등록
- controller : API의 endpoint를 등록하고, 요청/응답의 형식을 갖는 클래스 패키지
- domain : jpa entity (테이블)
- dto : DTO(Data Transfer Object)를 위치시키는 곳
    * Controller에서 요청/응답에 사용할 클래스
    * 로직 내부에서 데이터 전송에 사용할 클래스
- exception : 커스텀 Exception, Exception Handler 클래스 패키지
- repository : Repository(DB에 연결할 때 사용하는 인터페이스)가 위치하는 패키지
- service : 비즈니스 로직을 담는 서비스 패키지
- type : 상태타입, 에러코드, 거래종류 등의 다양한 enum class들의 패키지
``` 