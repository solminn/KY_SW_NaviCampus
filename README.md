# Shuttle Tag :bus:
스마트 캠퍼스 셔틀버스 관리 시스템  
# 서비스 링크
**[NaviCampus 웹 서비스 바로가기](https://solminn.github.io/KY_SW_NaviCampus/index.html)**
#  프로젝트 소개
**NaviCampus**는 대학생들이 겪는 셔틀버스 이용 시 발생하는 불편함을 해소하기 위해 기획된 스마트 캠퍼스 어플리케이션
# 프로젝트 목표
* **버스 도착 예정 시 제공**: 교통·날씨 데이터를 결합한 지연률 및 도착 예상 시간 제공
* **체계적인 혼잡도 관리**: 실시간 탑승 인원 데이터를 기반으로 차량 내 혼잡 상태를 시각화하여 재학생들의 분산 탑승을 유도한다.
* **안전하고 신속한 탑승 인증**: QR 인증 모듈을 구현하여, 재학생 인증 절차를 간소화하고 외부인의 무단 탑승을 방지한다.
* **운행 효율성 극대화**: 버스 기사용 운행 대시보드와 관리자 전용 노선 관리 툴을 제공하여 학기별 유연한 배차 최적화를 지원한다.
# 세부 기능
* **로그인 관리**: 가입된 소속 학교가 아닌 경우 페이지 접근 차단, 노선 일부 기능 이용 불가
* **실시간 버스 조회 & 예측**: GPS와 API 연동을 통한 실시간 차량 위치 추적 (5~7초 간격 자동 갱신)
* **QR 탑승 인증**: 재학생 학번 기반의 안전한 자체 QR 토큰 발행 및 유효성 검사
* **좌석 사전 예약**: 노선별 잔여 좌석 현황을 실시간 조회하고 중복 예약을 제어하는 좌석 배치 및 예약 시스템
* **기사 운행 대시보드**: 실시간 노선·시간표 조회 및 실시간 교통 정보(체증/사고) 수신 기능
* **시스템 관리자 모드**: 노선 정보(정류장, 운행 시간, 배차 간격)의 유연한 등록·수정·삭제
  
# 시스템 아키텍처
<img width="1280" height="720" alt="Image" src="https://github.com/user-attachments/assets/7dc7911e-0215-43fc-86f6-275c2582b2ba" />

# 기술 스택 및 개발 환경
* **모델 개발:** Python, Jupyter Notebook

* **데이터베이스:** Firebase (Firestore)

* **웹 개발:** HTML5, Visual Studio Code

* **버전 관리:** GitHub

# 프로젝트 구조
```text
KY_SW_NaviCampus/
├── index.html           
├── admin.html           
│
├── dankook_shuttle.html    
├── kaist_shuttle.html    
├── kongju_shuttle.html    
├── konyang_shuttle.html  
├── mokwon_shuttle.html 
│
├── manifest.json        
├── service-worker.js      
├── icon-192.png       
├── icon-512.png        
└── README.md
