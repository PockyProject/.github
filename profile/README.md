# 📌 2024 전공종합설계

<p align = "center"><img src="https://github.com/PockyProject/.github/assets/122958854/2c97fa5d-3bc4-4094-8149-a6cea925aafa"></img></p>

<p align = "center">주머니속 키오스크
<p align = "center">

<img width="966" src="https://github.com/PockyProject/.github/assets/122958854/56e0a389-98bc-4922-a6c3-d1d7ada00e2f">
<a href="https://github.com/cdjsdjwkfgkrhtlvek">
<img src="https://img.shields.io/badge/Github%20%ED%95%9C%EC%84%B1%EC%A7%84-181717?style=flat&logo=GitHub&logoColor=white"></a>
<a href="https://github.com/yolominwoo">           
<img src="https://img.shields.io/badge/Github%20%EC%A0%95%EB%AF%BC%EC%9A%B0-181717?style=flat&logo=GitHub&logoColor=white"></a>

<a href="https://github.com/conquest2023">        
<img src="https://img.shields.io/badge/Github%20%EA%B0%95%EC%A3%BC%ED%98%95-181717?style=flat&logo=GitHub&logoColor=white"></a>

  <a href="https://github.com/centerfoward">        
<img src="https://img.shields.io/badge/Github%20%EC%A0%95%EC%84%B1%EC%9A%B1-181717?style=flat&logo=GitHub&logoColor=white"></a>
</p>

## 🛠 Stack 🛠
<p align="center">
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=Python&logoColor=white"/></a>
<img src="https://img.shields.io/badge/Java-007396?style=flat&logo=OpenJDK&logoColor=white"/></a>

<p align="center">
<img src="https://img.shields.io/badge/Android%20Studio-A4C639?style=flat-square&logo=android&logoColor=white"/></a>
<img src="https://img.shields.io/badge/IntelliJIDEA-000000.svg?style=flatsquare&logo=intellij-idea&logoColor=white"/>
</p>
<p align="center">
<img src="https://img.shields.io/badge/springboot-6DB33F?style=flatsquare&logo=springboot&logoColor=white">
<a href="https://www.mysql.com/" target="_blank"><img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=MySQL&logoColor=white"/></a>
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=FastAPI&logoColor=white"/></a>  
<img src="https://img.shields.io/badge/Retrofit-48b983?style=flat-square&logo=Android&logoColor=white">
</a>
</a>
</p>
<p align="center">
<a>
<img src="https://img.shields.io/badge/ZXING-343434?style=flat-square&logo=&logoColor=white"/>
<img src="https://img.shields.io/badge/Raspberry%20Pi-A22846?style=flat-square&logo=Raspberrypi&logoColor=white"/>
</p>

<p align="center">
<img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=Redis&logoColor=white"> 
<img src="https://img.shields.io/badge/AWS%20EC2-FF9900?style=flat-square&logo=amazonWebServices&logoColor=white">
<img src="https://img.shields.io/badge/docker-%230db7ed.svg?style=flat-square&logo=docker&logoColor=white"/>
<img src ="https://img.shields.io/badge/Hibernate-59666C?style=flat-square&logo=Hibernate&logoColor=white"/>
</p> 

 ⚙ Used Technique

| Stack | Technique | Role Officer |
| :--------------------------: | :-----------------------------------------------: | :------------------------------: |
| <center> Front-End </center> | <center> AndroidStudio(Xml/Java) </center> | <center> 한성진 ,정성욱 </center>                     |
| <center>  Back-End </center> | <center> SpringBoot3,AWS(EC2)  </center>                  | <center> 정성욱,강주형 </center> |
| <center>  Embedded-System </center> | <center> Python</center>                  | <center> 정민우 </center> |
| <center>  AI </center> | <center> Python,FastAPI</center>                  | <center> 강주형 </center> |


### **<목차>**

**1️⃣, 프로젝트 개요**

1.  프로젝트 소개/제안 배경
2.  역할 분담

**2️⃣, 프로젝트 기획**

1.  UI 구성
2.  기능 구성

**3️⃣, 아키텍처 구성도**

1.  아키텍처 구성도

---

### **1️⃣, 프로젝트 개요**

## 1-1. 프로젝트 소개/제안 배경

-   제안 배경 <br/>
    기존의 오프라인 키오스크 환경의 경우 사용환경에 따라 사용인원에 제한이 생기거나 사용자의 상황에 따라 제한이 생기는 상황이 발생하게 된다. 이를 해결하고자 모바일 앱을 통한 온라인 환경을 구축하여 사용자에게 일관된 서비스환경을 제공하여 거부감을 줄이고 빠른 주문 프로세스를 통해 높은 사용 만족감을 제공하고자 설계하였다.  <br/>
    <p align = "center">
    <img width="405" alt="2" src="https://github.com/PockyProject/.github/assets/94755822/db5522b0-1feb-481b-8d36-9b57284e61ea">
    <img width="405" alt="1" src="https://github.com/PockyProject/.github/assets/94755822/ab05e0aa-5977-454f-933a-2424e20b064d"><br/>
    </p>
    
    위 그래프는 한국소비자원에서 키오스크 이용실태조사 중 왼쪽은 키오스크 이용 중 불편 또는 피해 경험 조사 결과를 도식화하였고, 오른쪽은 불편함을 느낀 이유에 대한 조사 결과를 도식화한 자료이다.
    생각보다 높은 인원이 키오스크 이용에대해 불편함을 겪었고, 이 중 키오스크 사용 시 가장 불편했던 점으로 뒷사람 눈치를 꼽았다.<br/>
    이런 불편한 점을 어떻게 개선할까 고민하던 와중 키오스크별로 조작 방법,화면 구성은 다르지만 QR 리더기가 모든 키오스크에 부착되어있는 사실을 알게되었다.<a>  </a>
    그렇다면 핸드폰에서 미리 주문을 하고 주문한 정보를 담은 QR 코드를 키오스크에 인식만 한다면 현행 키오스크 주문 프로세스를 획기적으로 줄일 수 있고 <br/>
    이로인해 현재 키오스크 이용 불편 사례 중 가장 큰 점인 뒷사람 눈치 문제를 해결할 수 있다고 생각이 들어 본 앱을 기획하게 되었다.
    
-  프로젝트 소개 <br/>
   본 프로젝트는 주머니속 키오스크(Pocket Kiosk) 즉 키오스크를 앱으로 간편하게 주문 할 수 있는 프로젝트이다. <br/>
   본 앱의 목표는 일반인뿐만 아니라 디지털 취약계층도 손 쉽게 사용할수 있게 하는것을 목표로 잡았다.

## 1-2. 역할 분담

###  한성진

- **현재까지 진행한 업무**
  
    - KakaoLoginApI를 사용해서 사용자 정보 생성
    - KakaoLoginApI를 사용해서 로그인 구현
    - Zxing 라이브러리를 이용한 QR코드 출력 기능 완성
    - 피드 화면 최적화를 위한 데이터 캐싱 구현
    - 즐겨찾기, 주문내역 데이터구조 설계
    - QR 출력을 위한 데이터구조 설계
    - Glide 라이브러를 사용한 메뉴 사진, 사용자 사진 출력 완성

<br>
    
###  정민우

- **현재까지 진행한 업무**
  
    - ZXing 라이브러리를 사용해서 QR 코드 출력 기능 완성
    - 프로토타입 키오스크 완성
<br>

### 강주형 

- **현재까지 진행한 업무**
    - SpringBoot의 Jpa를 활용하여 MysqlDB와 연결하고, MysqlDB와 앱간 통신을 위해 API를 구현
    - AWS EC2로 Docker 컨테이너 환경 구성
    - DockerSwarm을 통해 로드 밸런서 구축
    - github Action으로 Docker hub를 통해 CI/CD 구축
    - 사용자 피드,댓글, 알람기능을 위한 서버 구축

<br>

### 정성욱

- **현재까지 진행한 업무**
    - Aws Ec2, RDS 환경 구축
    - mysql DB 환경 구축
    - 스플래시,메인,주문,즐겨찾기,주문내역,더보기,피드 화면 구현
    - 피드 화면 최적화를 위한 데이터 캐싱 구현
    - 서비스 내부 Room DB 구현
    - 즐겨찾기, 주문내역 데이터구조 설계
    - QR 출력을 위한 데이터구조 설계
    - Zxing 라이브러리를 이용한 QR코드 출력 기능 완성
    - Retrofit2 라이브러리를 사용한 서버 연결 환경 구현
    - Glide 라이브러를 사용한 메뉴 사진, 사용자 사진 출력 완성
    
<br>




---

### **2️⃣. 프로젝트 기획**
## 2-1. UI 구성

<img width="877" alt="image" src="https://github.com/user-attachments/assets/1d5e9b80-1f1b-406f-8569-8c690abc3477">

- https://www.figma.com/design/q6rdXpACnryMbhxYHXLipV/%EB%B0%9C%ED%91%9C%EC%9E%90%EB%A3%8C?node-id=78-469&t=s0FF0j3v4tU8hbVo-4

---
## 2-2. 기능 구성

- **사용자 선택메뉴 QR코드화** <br>
  - 사용자가 선택한 메뉴를 QR코드안에 담아 매장 내 키오스크에 스캔 시 사용자가 선택한 메뉴가 키오스크로 전송
<img width="420" alt="image" src="https://github.com/user-attachments/assets/6d8a3150-d918-41c3-8786-7821200a496b">

- **생성된 QR코드 공유** <br>
  - 사용자가 생성한 QR코드를 타 사용자에게 공유
<img width="423" alt="image" src="https://github.com/user-attachments/assets/bdff4f47-ccb8-4e72-a215-707b7fca4305"> 

- **메뉴 즐겨찾기** <br>
  - 사용자가 선택한 메뉴를 저장하는 기능으로 사용자가 차후 같은 메뉴를 주문하려고 할 시 즐겨찾기 기능을 통해 시간을 절약
<img width="409" alt="image" src="https://github.com/user-attachments/assets/975f2b32-6ccf-465f-9979-7c3a43b080ab"> 

- **커뮤니티 피드** <br>
  - 타사용자에게 자신만의 메뉴 조합을 추천 및 댓글기능을 활용하여 의견 공유
<img width="427" alt="image" src="https://github.com/user-attachments/assets/2779c8a8-c39a-4efa-87de-54f7d8f4a0bf"> 
  
- **AI 메뉴 추천 기능** <br>
  - 사용자의 주문내역을 토대로 AI를 활용하여 사용자에게 맞춤 메뉴 추천
<img width="720" src="https://github.com/PockyProject/App/assets/52391699/4b10d88c-37a3-4dd3-950a-51de883a7532">



### **3️⃣. 아키텍처 구성도**

## 3-1. 아키텍처 구성도

![image](https://github.com/user-attachments/assets/9e20788b-343e-44b8-b1fb-a68671a3865f)


