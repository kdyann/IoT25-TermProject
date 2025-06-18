# IoT25-TermProject
# IoT 기반 실내 흡연 감지와 웨어러블 금연 유도 기능의 스마트 시스템
Integrated smart system for smoking detection and quitting smoking


## 📘 프로젝트 소개

이 프로젝트는 공공장소에서의 흡연을 실시간으로 감지하고, 동시에 개인의 흡연 습관과 스트레스 패턴을 분석하여 금연을 유도하는 **IoT 기반 통합 스마트 시스템**입니다.  
ESP32, 다양한 센서, TinyML 모델, BLE 비콘, 모바일 앱, 대시보드 등으로 구성되며, 공공보건과 건강 증진을 동시에 목표로 합니다.

## 주요 기능

- **공공장소 흡연 감지**
  - MQ-135 센서 기반 연기 및 유해가스 감지
  - DHT22 온습도 보정
  - TinyML 모델 기반 실시간 추론
  - 환풍기/창문 자동 제어 + 관리자 알림
- **개인 웨어러블 금연 유도**
  - 자이로/가속도 센서를 통한 손목 동작 분석
  - 심박 센서로 스트레스 상태 측정
  - 흡연 행동 탐지 시 진동 피드백 및 대체 행동 제시
- **BLE 비콘 기반 금연구역 인식**
  - 금연 감지기에서 BLE 비콘 송신
  - 웨어러블이 감지해 “금연 구역입니다” 진동/알림 제공
- **서버 및 UI 연동**
  - 관리자 웹 대시보드: 실시간 감지 현황, 로그 기록
  - 사용자 앱: 스트레스 상태, 흡연 추이 리포트 제공
 
## 🛠 기술 스택
센서/하드웨어	MQ-135, DHT22, MPU6050, MAX30100, ESP32
AI	TensorFlow Lite Micro (TinyML), SVM, Random Forest
앱	Flutter + BLE
서버	Node.js + Firebase
대시보드	React.js
통신	Wi-Fi, BLE, MQTT
