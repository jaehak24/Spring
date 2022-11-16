# MVC 워크플로우


![image](https://user-images.githubusercontent.com/65396939/202103665-7d9e3903-30f4-48be-8211-48b16e82d8e9.png)


## 1.요청 전송
    클라이언트로부터 DispatchServlet으로 요청 데이터가 전송
    
## 2. Controller 검색
    DispatchServelet이 HandlerMapping에게 해당 요청에 상응하는 인터페이스를 요청
    
## 3.Controller 정보 리턴
    해당 요청에 상응하는 컨트롤러 정보 리턴
    
## 4. HandlerAdapter 호출 위임
    DispatchServlet이 handlerMapping으로부터 받은 정보를 토대로 해당 Controller의 Handler 메서드를 호출.
    이 때, DispatchServlet이 이를 직접 호출하지 않고, Handler Adpater에게 Handler 메서드 호출을 위임함
    
## 5. HandlerAdapter    
    DispatchServlet에게 받은 정보를 토대로 해당 Handler를 호출
    
## 6. Model 반환 
    HandlerAdapter는 비즈니스 로직을 처리 한 Controller로부터 Model을 받음
    
## 7. Servlet에게 Model 전달
    HandlerAdapter는 Model과 View 정보를 받아 DispatchServlet에게 전달
    
## 8. View 검색 요청
    DispatchServlet은 다시 View Resolver에게 정보와 부합하는 View를 요청
    
## 9.View 정보 반환
    View Resolver는 정보와 상응하는 View를 return
    
## 10. 응답 데이터 생성 요청& Model 데이터 전달
    앞서 받은 Model을 View 객체를 통해 View에게 전달하면서 View로부터 응답 요청을 전송
    
## 11. View 응답
    View는 응답 데이터를 생성해서 DispatchServlet에게 응답 데이터를 전송
    
## 12. 클라이언트에게 전달
    DispathServlet은 View로부터 받은 응답 데이터 전송을 받은 데이터를 클라이언트에게 전달
    
    

