# 박현정 (Park Hyun Jung)

### Front-End / Robotics Software Engineer

[hyunjp03@gmail.com](mailto:hyunjp03@gmail.com) | [hyunjp03.netlify.app](https://hyunjp03.netlify.app) | [github.com/hyunjp03](https://github.com/hyunjp03) | 010-4284-0909

---

## 경력 및 프로젝트

### `AI · 로봇 엔지니어 양성과정 - 두산 8기` (2026.02 - 2026.08, 수료)

비전 인식(YOLO/CNN)부터 ROS2 로봇 제어까지 End-to-End 파이프라인을 구현하는
인식-제어 통합 팀 프로젝트 4건에 비전·로봇제어·프론트 담당으로 참여.

데이터 구축 → 모델 학습·선정 → ROS2 노드 배포 → 로봇 동작 연결까지 AI 모델 개발 전 과정을 프로젝트마다 반복 수행.

#### AI 기반 불법 주정차 무인 순찰 및 단속 시스템 (2026.06.17 - 2026.06.30)

YOLO 차량·번호판 탐지 + ROS2 다중 AMR 자율주행 제어 + Django/Supabase 통합 관제 시스템

- YOLO/v8 기반 차량·번호판 객체 탐지 모델 학습 및 데이터 라벨링, Google Vision OCR 연동
- 고정 웹캠 탐지 좌표를 Homography로 ROS 지도 좌표계로 변환해 불법 주정차 위치 산출, 번호판 미인식 시 LiDAR 클러스터링·RANSAC·PCA 기반 자가 위치 복구 루틴 설계
- 비전·프론트 엔지니어로 번호판 OCR 로직과 실시간 관제 대시보드 구축 (기여도 60%)

#### 약국 업무 보조 로봇 시스템 (2026.07.01 - 2026.07.14)

Doosan M0609 로봇팔 순응/힘 제어 + Flask·Django 웹 대시보드 + ROS2 상태 관리

- 처방·재고 비교 기반 리필 판정 로직 및 조제 이벤트 상태 통합 관리 구현
- movej/movel 정밀 좌표 제어와 순응/힘 제어(task_compliance_ctrl)로 약통 뚜껑 개폐 자동화
- 하드웨어 지그 직접 3D 모델링·제작
- 웹/DB 연동 및 스크래퍼(포장) 동작 노드 구현 담당 (기여도 60%)

#### 시각장애인 능동형 보조 로봇 (2026.07.15 - 2026.07.29)

YOLO11s-seg 객체 인식 + MediaPipe 손 추적 + LangChain 음성 파싱 + ROS2 상태 머신

- Voice Command → Object Detection → Hand Tracking → Active Assistance 4단계 파이프라인 설계
- 4개 클래스 Instance Segmentation 데이터 직접 라벨링, 4개 아키텍처 비교 실험 후 mAP50-95(M) 0.934로 최고 성능 모델 채택
- YOLO11s-seg 모델 학습·비교 실험 및 카메라 픽셀→Depth→로봇 베이스 좌표 변환(Hand-Eye Calibration) 파이프라인 구축 담당

#### 폐배터리 분해·검사·재조립 디지털 트윈 (2026.07.30 - 2026.08.12)

Isaac Sim + ROS2 + RMPFlow 기반 Doosan M0609 ×5대 Multi-Robot Orchestration

- 배터리 투입→분해→검사·선별→재조립 9단계 자동화 공정에서 위치 탐색(OpenCV)·판정(CNN ResNet34) 파이프라인 설계
- 소규모 데이터셋(120장)에서 Augmentation·활성화 함수·커널 크기 4종 Ablation 실험을 설계·비교, 구조를 복잡하게 할수록 성능이 저하되는 결과를 분석해 Baseline 구조 채택
- Vision 인식(CNN 셀 검사 모델, 로봇 제어 알고리즘)과 Isaac Sim MAP·환경 구성 담당

<br>

### DFZ (2023.11 - 2026.02)

*프론트엔드 엔지니어 @FE개발팀 (선임)*

LG U+ 홈페이지 운영·고도화 등 기업 웹/앱 서비스의 개발 및 유지보수 담당.

**LG U+ 홈페이지 운영 및 고도화(웹/앱)** (2024.10 - 2025.12) - [lguplus.com](https://www.lguplus.com/)

- Nuxt 기반 디스플레이 모듈 시스템 개발 및 SSR/CSR 하이브리드 렌더링 전략 적용으로 초기 로딩 성능 및 SEO 품질 개선
- 관심사 분리(SoC) 기반 컴포넌트 아키텍처 리팩토링을 통해 코드 재사용과 유지보수성 향상
- 레거시 의존성 제거 및 렌더링 병목 구간 최적화를 통해 페이지 렌더링 퍼포먼스 개선
- 레이어별 독립 테스트 및 운영 구조 정립으로 배포 안정성 확보 및 장애 대응 효율성 강화

**롯데카드 띵샵 홈페이지 리뉴얼(웹/앱)** (2024.05 - 2024.09) - [locashop.lottecard.co.kr](https://locashop.lottecard.co.kr/main)

- Vue 기반, 기존 베이스 컴포넌트를 재사용하며 새 디렉토리·구조로 전체 웹사이트 리뉴얼 진행
- 상세 페이지 내 팝업 이미지 확대 기능 플러그인 없이 자체 제작

<br>

### 언플러 (2021.03 - 2023.11)

*프론트엔드 엔지니어 @FE개발팀 (대리)*

교육 콘텐츠·이커머스 등 다양한 도메인의 반응형/적응형 웹 퍼블리싱 및 프론트엔드 개발 수행.

**웅진 라이브올 반응형 웹사이트** (2022.03 - 2022.08) - [liveall.co.kr](https://www.liveall.co.kr/)

- React 기반 실시간 교육 영상 플랫폼 퍼블리싱, 재사용 컴포넌트 설계 (기여도 80%)
- 프로젝트 마크업 구조, 반응형 스타일, 인터랙션 구현 스크립트 담당, 초기 컴포넌트 마크업 작업 담당 (기여도 80%)

**웅진 예비초/초등 게임성 학습 콘텐츠** (2021.03 - 2023.07)

- 캔버스 색칠·드래그앤드랍 인터랙션 학습 콘텐츠 퍼블리싱, 공통 스크립트화로 대량양산 설계 (기여도 100%)

**프리스비 적응형 웹사이트** (2021.10 - 2022.01) - [frisbeekorea.com](https://www.frisbeekorea.com/shop/main/main.do)

- 애플 프리미엄 스토어 이커머스 초기 마크업 및 유지보수 (기여도 50%)
- 회원가입, 마이페이지, 모바일 전체 페이지 퍼블리싱 작업 & 서비스 오픈 후 유지 보수

---

## 기술 스택

- **Robotics**: ROS2 Humble(Nav2, SLAM, TF2, Topic · Service · Action), Doosan M0609 DSR API(movej/movel, 순응/힘 제어), Hand-Eye Calibration, Isaac Sim, TurtleBot4, OAK-D, LiDAR
- **AI / Vision**: PyTorch, Ultralytics YOLO(v8 / 11, Detection · Instance Segmentation), CNN(ResNet 전이학습), OpenCV, MediaPipe, 데이터 수집·라벨링·Augmentation, mAP 기반 모델 비교 실험
- **Web / Backend**: Vue / Nuxt, React, Django, Flask, Supabase

---

## 활동

### 두산 AI·로봇 엔지니어 양성과정(초급) 8기 수료 (2026.08)

- 6년간 쌓은 웹 퍼블리셔 및 프론트엔드 개발 경력을 로봇 오퍼레이션 영역으로 확장하기 위해 자발적으로 지원, 비전 인식부터 로봇 제어까지 이어지는 Physical AI 파이프라인 전 과정을 처음부터 학습하며 수료
- PyTorch 기반 CNN·전이학습(Fine-tuning 전략 비교)·객체 탐지(YOLO, Faster R-CNN)·XAI(Grad-CAM) 등 딥러닝 이론 및 실습 이수
- 4개 팀 프로젝트(불법 주정차 단속 로봇, 약국 보조 로봇팔, 시각장애인 보조 로봇, 폐배터리 검사 디지털 트윈)에서 매번 비전파트를 맡아, YOLO/CNN 기반 객체 인식 모델 학습부터 ROS2 로봇 제어, Django/Flask 백엔드 연동까지 End-to-End로 직접 구현
- 기존에 다루던 "화면 상태 관리·실시간 통신·예외 처리" 역량을 "다중 로봇 상태 모니터링·ROS2 토픽 송출·현장 Fail-safe 로직 설계"로 재해석하며, 로봇 시스템에서도 사람이 보는 화면(관제 대시보드)까지 책임지는 엔지니어로서의 강점을 실증
- 처음 다뤄보는 로봇 기구학(ZYZ 오일러각), Hand-Eye Calibration, Isaac Sim 시뮬레이션 환경 구성 등을 프로젝트 진행 중 스스로 학습해 적용, 새로운 도메인에 대한 빠른 습득력과 현장 적용력을 확인

---

## 교육

**남서울 대학교**<br>
아동복지학과 학사 (2010 - 2015)

**한국직업전문학교**<br>
스마트컨텐츠 UI/UX 퍼블리싱 과정 수료 (2019)
