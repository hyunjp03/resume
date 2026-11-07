# 박현정 (Park Hyun Jung)

### Front-End / Robotics Software Engineer

[hyunjp03@gmail.com](mailto:hyunjp03@gmail.com) | [hyunjp03.netlify.app](https://hyunjp03.netlify.app) | [github.com/hyunjp03](https://github.com/hyunjp03) | 010-4284-0909

---

## 핵심역량

- **협동로봇 티칭·운용**: Doosan M0609를 DART-Platform 티칭과 DSR API 코드(movej/movel, posj/posx) 두 방식으로 운용, Joint/Task Jog, 작업별 TCP 설정, 순응/힘 제어 기반 접촉 작업 경험
- **로봇 셋업과 좌표계 이해**: Hand-Eye Calibration으로 카메라·로봇 좌표 정합, Isaac Sim에서 로봇 5대 자동화 공정 구성 및 그리퍼 셋업
- **비전 연동과 모니터링 화면**: YOLO 인식 결과를 로봇 파지 동작에 연결, 5년 프론트엔드 경력으로 로봇 관제 대시보드 구현

---

## 경력 및 프로젝트

### `AI · 로봇 엔지니어 양성과정 - 두산 8기` (2026.02 - 2026.08, 수료)

비전 인식(YOLO/CNN)부터 ROS2 로봇 제어까지 End-to-End 파이프라인을 구현하는
인식-제어 통합 팀 프로젝트 4건에 비전·로봇제어·프론트 담당으로 참여.

데이터 구축 → 모델 학습·선정 → ROS2 노드 배포 → 로봇 동작 연결까지 AI 모델 개발 전 과정을 프로젝트마다 반복 수행.

#### AI 기반 불법 주정차 무인 순찰·단속 시스템 (2026.06.17 - 2026.06.30)

*AMR·비전 / 팀 프로젝트 / 기여도 40%*

단일 카메라의 사각지대를 AMR 2대의 순찰과 교차검증으로 보완하는 특수구역(일반/장애인/소방차) 불법 주정차 무인 관제 시스템

**사용기술**: TurtleBot4, OAK-D, ROS2 Humble, Nav2, SLAM, YOLOv8, Google Cloud Vision OCR, Django, Supabase

- 차량·번호판 탐지 데이터 수집·라벨링 및 YOLOv8 학습, ROS2 노드로 배포해 순찰 중 실시간 추론
- 번호판 OCR 노드 구현: document_text_detection(한국어 힌트) 적용, 번호판 크롭 이미지 업스케일링, 정규식 기반 번호판 정규화
- AMR1 1차 등록 후 AMR2가 근접 교차검증하는 2단계 판독 흐름, confidence 기반 중복 제거, 구역별 단속 로직
- 실시간 관제 대시보드 구축 (MJPEG 스트리밍)

**획득 역량**: 여러 대의 로봇을 하나의 운영 흐름으로 묶는 통합 경험, 로봇 상태와 이벤트를 운영자가 보는 관제 화면까지 연결하는 경험

#### 약국 업무 보조 로봇 시스템 (2026.07.01 - 2026.07.14)

*협동로봇 / 팀 프로젝트 / 기여도 60%*

처방·재고 정보를 바탕으로 약 리필 여부를 판정하고, 협동로봇이 약통 개폐와 포장(스크래퍼) 동작을 수행하는 약국 업무 보조 시스템

**사용기술**: Doosan M0609 DSR API, ROS2, Flask, Django

- (담당) 스크래퍼 포장 동작 노드 구현, 작업별 TCP 프로파일(Tool_v1/Tool_scraper) 설정·전환
- (담당) 웹 대시보드와 DB 연동, 조제 이벤트 상태 통합 관리
- movej/movel 좌표 제어와 순응/힘 제어(task_compliance_ctrl)로 약통 뚜껑 개폐 자동화
- 처방·재고 비교 기반 리필 판정 로직

**획득 역량**: 작업 도구에 맞춰 TCP를 나눠 설정하고 협동로봇의 접촉 작업을 셋업한 경험, 로봇 동작을 웹·DB의 업무 상태와 연결하는 시스템 통합 경험

#### 시각장애인 능동형 보조 로봇 (2026.07.15 - 2026.07.29)

*협동로봇·비전 / 팀 프로젝트 / 기여도 50%*

음성 명령을 받아 물체를 인식하고 사용자의 손 위치를 추적해 물건 전달을 돕는 능동형 보조 로봇

**사용기술**: Doosan M0609, Hand-Eye Calibration, YOLO11s-seg, MediaPipe, LangChain, ROS2

- 카메라 픽셀과 Depth를 결합해 로봇 베이스 좌표로 변환(Hand-Eye Calibration)하고 파지 동작까지 연결
- 4개 클래스 Instance Segmentation 데이터 직접 구축·라벨링, 4개 모델 구조 비교 후 mAP50-95(M) 0.934 모델 채택, ROS2 노드로 배포해 실시간 추론
- Voice Command, Object Detection, Hand Tracking, Active Assistance 4단계 파이프라인 설계

**획득 역량**: 카메라와 로봇 좌표계를 맞추고 단계별로 검증하는 방법, 인식 결과를 실제 로봇 동작으로 연결하는 경험

#### 폐배터리 분해·검사·재조립 디지털 트윈 (2026.07.30 - 2026.08.12)

*로봇 공정·비전 / 팀 프로젝트 / 기여도 50%*

폐배터리 투입부터 분해, 검사·선별, 재조립까지 여러 공정을 Isaac Sim에서 Doosan M0609 5대로 자동화한 디지털 트윈

**사용기술**: Isaac Sim, ROS2, RMPFlow, VG10 진공 그리퍼, PyTorch(ResNet34), OpenCV

- (담당) Isaac Sim 환경 세팅: 수평·Z축 기준을 정리해 작업대와 물품의 물리 조건 조정
- (담당) 로봇 모델을 통일하고, 방향별 도달 범위에 맞춰 배치, 도달 불가·팔 간 충돌 구간 해소
- (담당) 흡착 시 살짝 누르며 잡도록 그리퍼 동작을 수정해 파지 실패·낙하 문제 해결
- OpenCV 위치 탐색과 CNN(ResNet34) 판정을 잇는 셀 검사 파이프라인 설계, 4종 Ablation 실험 비교 후 Baseline 구조 채택

**획득 역량**: 여러 대의 로봇이 이어지는 자동화 공정을 시뮬레이션으로 먼저 구성하고 검증하는 경험, 소규모 데이터에서 실험 결과를 근거로 판단하는 방법

<br>

### DFZ (2023.11 - 2026.02)

*프론트엔드 엔지니어 @FE개발팀 (선임)*

LG U+ 홈페이지 운영·고도화 등 기업 웹/앱 서비스의 개발 및 유지보수 담당.

**LG U+ 홈페이지 운영 및 고도화(웹/앱)** (2024.10 - 2025.12) - [lguplus.com](https://www.lguplus.com/)

*사용기술: Nuxt, Vue, JavaScript*

- 디스플레이 모듈 시스템 개발, 로그인·회선 정보 기준 SSR/CSR 하이브리드 렌더링 적용
- 공통 컴포넌트(모달·알럿·폼)와 유효성 검사 유틸 정리
- API 호출 레이어(api/services) 분리, API mock 기반 프론트·백엔드 분리 검증
- 환경별 설정 분리 및 배포 전 QA

**롯데카드 띵샵 홈페이지 리뉴얼(웹/앱)** (2024.05 - 2024.09) - [locashop.lottecard.co.kr](https://locashop.lottecard.co.kr/main)

*사용기술: Vue2, Vanilla JavaScript*

- 기존 베이스 컴포넌트를 재사용하며 새 디렉토리 구조로 리뉴얼
- 플러그인 없이 줌 인/아웃 팝업 슬라이더 직접 구현

<br>

### 언플러 (2020.09 - 2023.11)

*프론트엔드 엔지니어 @FE개발팀 (대리)*

교육 콘텐츠·이커머스 등 다양한 도메인의 반응형/적응형 웹 퍼블리싱 및 프론트엔드 개발 수행.

**웅진 라이브올 반응형 웹사이트** (2022.03 - 2022.08) - [liveall.co.kr](https://www.liveall.co.kr/)

*사용기술: React, HTML/CSS*

- 실시간 교육 영상 플랫폼 퍼블리싱, 재사용 컴포넌트 설계 (기여도 80%)

**웅진 예비초/초등 게임성 학습 콘텐츠** (2021.03 - 2023.07)

- 캔버스 색칠·드래그앤드랍 인터랙션 학습 콘텐츠 퍼블리싱, 공통 스크립트화로 대량양산 설계 (기여도 100%)

**프리스비 적응형 웹사이트** (2021.10 - 2022.01) - [frisbeekorea.com](https://www.frisbeekorea.com/shop/main/main.do)

- 애플 프리미엄 스토어 이커머스 초기 마크업 및 유지보수 (기여도 50%)
- 회원가입, 마이페이지, 모바일 전체 페이지 퍼블리싱 작업 & 서비스 오픈 후 유지 보수

---

## 기술 스택

### 기술역량

| 구분 | 활용수준 | 보유스킬 |
|---|---|---|
| 로봇 티칭/운용 | ●●●○○ | Doosan M0609(DART-Platform 티칭, DSR API), Joint/Task Jog, TCP 설정, 순응/힘 제어 |
| 로봇 셋업 | ●●●○○ | Hand-Eye Calibration, Isaac Sim 공정 시뮬레이션(진공 그리퍼·Surface Gripper), TurtleBot4 |
| OS/SW | ●●●○○ | Ubuntu, ROS2 Humble(Nav2, SLAM, TF2), Python, Git/GitHub |
| 비전/딥러닝 | ●●●○○ | YOLO(v8/11), PyTorch, OpenCV, OAK-D |
| 웹 개발 | ●●●●● | Vue/Nuxt, React, JavaScript, Django, Flask |

### 상세 기술스택

| 구분 | 경험 및 활용수준 |
|---|---|
| **Doosan M0609** | DART-Platform에서 포인트 티칭, DSR API(movej/movel, posj/posx) 코드로 동작 작성 · Joint/Task Jog, 작업별 TCP 설정, 순응/힘 제어 기반 접촉 작업, Hand-Eye Calibration 기반 좌표 변환 |
| **Isaac Sim** | 로봇 5대 자동화 공정 시뮬레이션 환경 구성, 진공 그리퍼(Surface Gripper) 물리 설정 · RMPFlow 기반 경로 생성과 ROS2 연동 |
| **ROS2** | ROS2 Humble 기반 Topic·Service·Action 통신과 노드 설계로 센서 데이터 수집과 로봇 제어를 연결 · TF2·URDF로 로봇과 센서 좌표계 관리 |
| **SLAM & Navigation** | TurtleBot4로 SLAM 지도 작성 및 Nav2 BasicNavigator 웨이포인트 순찰 구현 · AMCL 위치 구독 기반 목표 추적·정지 동작 구현 |
| **Python** | ROS2 노드, 로봇 동작 스크립트, 비전 추론 등 로봇 시스템의 주요 구현 언어로 사용 · Flask·Django 백엔드와 데이터 처리 스크립트 작성 |
| **YOLO / OpenCV** | YOLOv8·YOLO11s-seg 데이터 구축, 학습, 모델 비교 후 ROS2 노드로 배포해 실시간 추론 · 탐지 결과를 좌표 변환과 연결해 로봇 파지·단속 로직에 활용 |
| **PyTorch / CNN** | CNN, 전이학습(ResNet, VGG), 학습 루프(Early Stopping, 학습률 스케줄러) 구현 · ResNet34 기반 불량 판정 모델과 Ablation 실험 수행 |
| **JavaScript / Vue·Nuxt** | 5년간 웹 퍼블리싱·프론트엔드 실무, Nuxt SSR/CSR 하이브리드 렌더링과 공통 컴포넌트 설계 · 로봇 프로젝트에서 실시간 관제 대시보드 구현 |
| **Git / GitHub** | 팀 프로젝트 브랜치 규칙 운영, stash·pull·pop 충돌 해결과 force-push 복구 경험 |

---

## 활동

### 두산 AI·로봇 엔지니어 양성과정(초급) 8기 수료 (2026.08)

- 5년간 쌓은 웹 퍼블리셔 및 프론트엔드 개발 경력을 로봇 오퍼레이션 영역으로 확장하기 위해 자발적으로 지원, 비전 인식부터 로봇 제어까지 이어지는 Physical AI 파이프라인 전 과정을 처음부터 학습하며 수료
- PyTorch 기반 CNN·전이학습(Fine-tuning 전략 비교)·객체 탐지(YOLO, Faster R-CNN)·XAI(Grad-CAM) 등 딥러닝 이론 및 실습 이수
- 4개 팀 프로젝트(불법 주정차 단속 로봇, 약국 보조 로봇팔, 시각장애인 보조 로봇, 폐배터리 검사 디지털 트윈)에서 매번 비전파트를 맡아, YOLO/CNN 기반 객체 인식 모델 학습부터 ROS2 로봇 제어, Django/Flask 백엔드 연동까지 End-to-End로 직접 구현
- 기존에 다루던 "화면 상태 관리·실시간 통신·예외 처리" 역량을 "다중 로봇 상태 모니터링·ROS2 토픽 송출·현장 Fail-safe 로직 설계"로 재해석하며, 로봇 시스템에서도 사람이 보는 화면(관제 대시보드)까지 책임지는 엔지니어로서의 강점을 실증
- 처음 다뤄보는 로봇 기구학(ZYZ 오일러각), Hand-Eye Calibration, Isaac Sim 시뮬레이션 환경 구성 등을 프로젝트 진행 중 스스로 학습해 적용, 새로운 도메인에 대한 빠른 습득력과 현장 적용력을 확인

---

## 교육

**두산로보틱스 ROKEY — 두산 AI·로봇 엔지니어 양성과정 8기** (2026.02 - 2026.08, 수료)<br>
PyTorch 기반 CNN·전이학습·객체 탐지(YOLO, Faster R-CNN)·XAI, ROS2 Humble(Nav2, SLAM, TF2), Doosan M0609 로봇팔 제어, Isaac Sim 시뮬레이션, 팀 프로젝트 4건 수행

**남서울 대학교**<br>
아동복지학과 학사 (2010 - 2015)

**한국직업전문학교**<br>
스마트컨텐츠 UI/UX 퍼블리싱 과정 수료 (2019)
