# 컴퓨터 시스템의 3계층 구조
- 가장 아랫층에 H/W, 가운데에 Kernel 모드, 제일 위에 User 모드로 이루어져있다
![image](https://github.com/Hwan0518/OperatingSystem-Study/assets/108791919/ca70c21c-bfca-484d-a32f-a6b1c005dbed)

<br>

### 운영체제(Operating System)란?
- 프로그램이 실행되기 위해 필요한 자원을 할당하고, 프로그램이 올바르게 실행되도록 돕는 특별한 프로그램
- 컴퓨터 시스템 3계층에서 Kernel 모드와 User 모드를 합쳐서 운영체제라고 한다

<br>

### 커널(Kernel)
- OS의 핵심 부분으로 자원관리와 S/W와 H/W사이에서 인터페이스 역할을 한다

<br>

### 프로세스(Process)
- 컴퓨터에 설치된 프로그램이 실행이되면 이를 곧 프로세스라 한다
- OS로부터 자원을 할당받은 "작업"의 단위로, 메모리에 적재되고 CPU 자원을 할당받는다 
- 시스템 프로세스와 사용자 프로세스로 나뉜다
  - System Process
    - 기능 : 시스템 운영에 필요한 핵심 기능 수행과, 시스템의 안정성과 성능을 유지하는 관리자 역할을 한다
    - 동작 : 일반적으로 백그라운드에서 동작한다
    - 예시 : Scheduler, Interrupt Handler, Momory Manager, Device Driver, Network Stack 등이 존재한다
    - 권한 : Admin 권한을 가지고 있다. 추가적으로 System Process의 Shell 명령에 의해 실행되는 Process는, Shell의 권한(Admin)을 상속받는다
      
  - User Process
    - 기능 : 사용자가 실행시킨 프로그램으로, 사용자의 요청에 따라 생성되며 사용자와 상호 작용하는 역할을 한다
    - 동작 : 주로 GUI나 터미널을 통해 사용자의 입력을 받고 출력을 생성한다
    - 예시 : 워드 프로세서, 웹 브라우저, 게임 등 다양한 응용 프로그램이 여기에 속한다
    - 권한 : 권한이 제한되어 있으며, 시스템 레벨의 작업을 직접적으로 수행하지 않는다
  
