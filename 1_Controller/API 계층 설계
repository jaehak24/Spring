# API 계충 설계

클라이언트의 요청을 직접적으로 처리해 주는 계층

## 기능 기반 패키지 구조
패키지 이름을 구성하는 면에서 패키지 이름을 
### 기능
으로 설계하는 것을 말한다.

ex>> Navigation 어플
package_1: map
package_2: route_to_direction
package_3: GPS Synchronization
...

등등 


## 계층 기반 패키지 구조
Spring work flow에서 있던 흐름과 같이 어플의 계층을 묶어서 패키지를 분배하는 시스템
ex> Navigation 어플

Package_1: Controller
  controller/ mapController
  controller/ GPS_sync_controller
  controller/ MainController
  
Pacakge_2: dto
  DTO/ MapDTO
  DTO/ GPSDTO
  ....
  
  등등
