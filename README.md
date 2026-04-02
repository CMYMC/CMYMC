
#  안녕하세요! 임베디드 개발자 윤찬민 입니다.
---
하드웨어와 소프트웨어를 아우르는 임베디드 시스템 개발자로 성장하고 있습니다.

---
## Education 
[Intel] Edge AI SW Academy (8기) (2025.07 ~ 2026.01) [수료]
 - STM32 펌웨어 및 FreeRTOS 기반 IoT 제어부터 리눅스 BSP, 디바이스 드라이버 설계, ROS2 등 임베디드 시스템 전반을 이수함
---

## 🔥 주요 프로젝트

### 🏋️ [자세어때 (AI Smart GYM)](https://github.com/CMYMC/Project-AI-Smart-Gym) 🏅Intel Edge AI Academy 프로젝트 경진대회 – 우수상 수상작

RaspberryPi5 + Hailo-8(NPU) 기반 실시간 운동 자세 분석 시스템

* YOLOv8-Pose + TCN 모델로 스쿼트 등 7개 운동 동작 실시간 분류 및 채점
* EMG·IMU 센서 융합으로 근육 피로도(FI)·좌우 불균형(BI)·템포 일관성 정량 분석
* Hailo-8 NPU 온디바이스 추론으로 30FPS  실시간 처리 달성
* PySide6 대시보드에서 운동 점수·세션 리포트 시각화

---
### 🤖 [Relay-Bot (재난 통신 복구 로봇)](https://github.com/CMYMC/Project-Relay_Bot)

재난 현장에서 끊어진 네트워크를 로봇이 스스로 이동하며 복구하는 자율 이동형 메시 중계 로봇 시스템

* BATMAN-adv 기반 Layer-2 메시 네트워크 구성, 기지국 없이 독립 통신망 구축
* 통신 품질(TQ) 변화량(Gradient)만으로 지도 없이 최적 중계 위치를 스스로 탐색
* ROS2 기반 자율 주행과 Qt 관제 대시보드를 통한 실시간 영상 스트리밍 및 네트워크 모니터링
* 실제 건물 복도·계단에서 RelayBot 중계 통신 성공 실증

---
### 🕐 [Linux Kernel Device Driver Clock](https://github.com/CMYMC/Device-Driver-Clock)

Raspberry Pi 4 + Linux Kernel 기반의 임베디드 시계 시스템

* 유저 공간 없이 커널 드라이버 자체적으로 시간 설정 및 UI 제어 구현
* FSM 기반 선택/수정 모드 전환, 로터리 엔코더 인터럽트로 시간 설정
* Workqueue로 인터럽트 문맥과 I2C 통신을 분리하여 커널 안정성 확보
* DS1302 RTC 동기화로 전원 차단 후에도 시간 유지

---
### 🚗 [대형차 전방 제어 시스템 (SmartCar)](https://github.com/CMYMC/Project-SmartCar)

STM32, Arduino, Raspberry Pi, MariaDB를 연동한 차량 안전 제어 시스템

* 초음파 센서 거리 측정 + 엔코더 피드백 기반 PID 알고리즘으로 모터 속도 자동 제어
* TCP/IP 소켓 통신으로 주행 데이터(속도·거리·PWM)를 1초 주기 DB 실시간 저장
* Arduino LCD·LED로 운전자에게 현재 상태 및 안전 거리 경고 표시
* 10cm 미만 강제 정지 / 30cm 이하 비례 감속 / 30cm 초과 정속 주행 구현



---
### 🌐 [RTOS-CAN Gateway System](https://github.com/CMYMC/Project-RTOS-CAN-Gateway-System)

STM32 + FreeRTOS 환경에서 CAN 분산 노드 데이터를 이더넷으로 전달하는 게이트웨이 시스템

* FreeRTOS 멀티 태스크 구조 + Event/Semaphore 기반 CAN 수신 동기화 설계
* CAN Filter 직접 설정 및 메시지 ID 기반 분기 처리, 프레임 패킹으로 데이터 구조화
* Board C를 게이트웨이 노드로 설정해 CAN → Ethernet 데이터 흐름 설계
* 수집 데이터를 UDP 기반으로 Raspberry Pi에 전달, SQLite DB에 1초 주기 스냅샷 저장


---

### 🌱 [스마트팜](https://github.com/CMYMC/Project-SmartFarm)

STM32 + FreeRTOS 기반 환경 자동 제어 스마트팜 시스템

* DHT11·수위 센서 데이터를 기능별 독립 태스크로 분리해 FreeRTOS 멀티태스킹 구현
* 온도 30℃ 초과 시 스텝모터 팬 자동 가동, 수위 부족 시 서보모터 펌프 자동 급수
* RGB LED 3단계(정상/경계/경고) 및 부저로 시스템 상태 직관적 알림
* 태스크 우선순위 최적화로 센서·LCD 동시 동작 안정성 확보

---

### ⏰ [STM32 Alarm Clock](https://github.com/CMYMC/Project-Alarm-Clock)

STM32 내부 자원(Flash, Timer, ADC)을 최대 활용한 디지털 알람 시계

* FSM 기반 4가지 모드(시계/시간설정/알람설정/음악선택) 상태 전환 구현
* 단일 ADC 핀으로 5개 버튼 식별, Short/Long/Double Click 동작 구분 처리
* PWM 주파수 변조로 멜로디 알람 재생, 사용자 선택 알람음 지원
* Flash 메모리 직접 제어로 전원 차단 후에도 시간·알람·음악 설정 유지

---



## 🛠 Tech Stack

### 💻 Languages
![C](https://img.shields.io/badge/Language-C-A8B9CC?style=flat-square&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/Language-C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)
![Python](https://img.shields.io/badge/Language-Python-3776AB?style=flat-square&logo=python&logoColor=white)

### 🔌 Embedded & Hardware
![STM32](https://img.shields.io/badge/MCU-STM32-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)
![Arduino](https://img.shields.io/badge/MCU-Arduino-00979D?style=flat-square&logo=arduino&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Board-Raspberry_Pi-C51A4A?style=flat-square&logo=raspberry-pi&logoColor=white)
![ARM](https://img.shields.io/badge/Architecture-ARM-0091BD?style=flat-square&logo=arm&logoColor=white)
![Hailo](https://img.shields.io/badge/NPU-Hailo-333333?style=flat-square&logoColor=white)

### ⚙️ OS & Frameworks
![Linux](https://img.shields.io/badge/OS-Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![ROS2](https://img.shields.io/badge/Framework-ROS2-22314E?style=flat-square&logo=ros&logoColor=white)
![RTOS](https://img.shields.io/badge/OS-FreeRTOS-008A97?style=flat-square&logoColor=white)
![PyTorch](https://img.shields.io/badge/Framework-PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)

### 🛠 Tools & DB & Vision
![Qt Creator](https://img.shields.io/badge/IDE-Qt_Creator-41CD52?style=flat-square&logo=qt&logoColor=white)
![MariaDB](https://img.shields.io/badge/DB-MariaDB-003545?style=flat-square&logo=mariadb&logoColor=white)
![OpenCV](https://img.shields.io/badge/Vision-OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![Git](https://img.shields.io/badge/Tool-Git-F05032?style=flat-square&logo=git&logoColor=white)

