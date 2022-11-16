# Spring MVC

    Spring MVC: Spring의 모듈 중에는 우베 계층을 담당하는 모듈들이 있음
  

## 서블렛(Servlet)

    클라이언트의 요청을 처리하도록 "특정 방식"으로 Java 코드로 작성하는 클래스 파일

## 모델(Model)
    
    Spring MVC가 처리해서 가져온 결과물
    
## View(뷰)

    앞서 언급한 Spring MVC의 모델을 이용해서 화면에 보여지는 데 필요한 리소스를 제공하는 역할
    
## Controller

    Model과 View의 중간점에 위치해 있으며, 클라이언트 측의 정보를 받고 어플리케이션의 비즈니스 로직을 거치고 나온 모델을 
    View로 전달하는 역할
    
    
# 전체적인 Spring MVC 흐륾

    Client 요청 데이터 전송 -> Controller가 요청 데이터 수신 -> 비즈니스 로직 처리 ->Model 데이터 생성 -> Controller에게 Model 데이터 전송
    -> Controller가 View에게 Model 데이터 전달 -> View가 응답 데이터 생성


