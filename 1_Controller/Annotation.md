    @RestController
   1. 클래스 위에 위의 Annotation 추가 시 해당 클래스가 REST API의 리소스를 처리하기 위한 API 엔트포인트로
   한다고 선언
   2. 애플리케이션 로딩 시, Spring Bean으로 등록


    @RequstMapping
   1. 클라이언트의 요청 <-> 핸들러 메서드를 매핑해주는 역할을 합니다.
   
   
    @PostMapping
   1. 클라이언트 요청 데이터를 서버에 생성할 때 사용되는데, 클라이어트에 요청 신호를 전송할 때,
   Http Method 타입을 동일하게 맞춰주어야 합니다.
   
    @RequestParam
   주로 클라이언트 쪽에서 전송하는 Request 데이터를 쿼리 파라미터, 폼 파라미터 형식으로 전송하여
   이를 서버 쪽에서 전달 받을 때 사용하는 어노테이션
   
    @GetMapping
   클라이언트가 서버에 리소스를 조회할 때 사용하는 어노테이션
   
    @PathVariable
   괄호 안에 입력한 문자열 값은 @GetMapping("/{00-id}")처럼 중괄호({}) 안의 문자열과 같아야 함.
    
   
