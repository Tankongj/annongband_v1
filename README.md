# 🌾 안농밴드 (An-Nong Band) v1

> **웨어러블 IoT 기반 농업인 건강·안전 통합 관리 시스템**  
> NH [X StartUp] 2026 오픈이노베이션 제안 프로토타입

---

## 🎮 데모 체험

| 앱 | 설명 | 링크 |
|:---|:-----|:-----|
| ⌚ 워치 앱 | Apple Watch 시뮬레이터 (5화면) | [데모 →](https://Tankongj.github.io/annongband_v1/watch/) |
| 📱 사용자 앱 | 농업인 모바일 대시보드 (3탭 + AI 채팅) | [데모 →](https://Tankongj.github.io/annongband_v1/user/) |
| 🖥️ 관리자 앱 | Farm Worker 360 웹 대시보드 | [데모 →](https://Tankongj.github.io/annongband_v1/admin/) |

## 📋 프로젝트 개요

안농밴드는 농업인의 **근골격계 질환 예방**과 **안전사고 대응**을 위한 IoT 웨어러블 시스템입니다.

### 핵심 문제
- 농업인 업무상 질병 중 근골격계 비율: **84.6%**
- 농업인안전보험 손해율: **97.9%**
- 연간 사회적 손실: **5,194억원**

### 솔루션
```
손목보호대 + IMU/PPG 센서 → Edge AI HAR → 30분 넛지 → 운동 처방 → 보험 연계
```

## 🏗️ 시스템 아키텍처

```
📡 안농밴드 (ESP32+IMU+PPG)
    ↓ BLE
⌚ 스마트워치 (Apple/Galaxy) — Standalone 모드
    ↓ BLE/Wi-Fi
📱 사용자 앱 — 안농이(AI) 건강 대화 + 운동 처방
    ↓ API
☁️ Farm Worker 360 — 클라우드 분석
    ↓
🖥️ 관리자 대시보드 — 통합 관제
    ↓
🛡️ NH농협 — 보험 할인 연계
```

## 📂 폴더 구조

```
annongband_v1/
├── README.md
└── docs/               ← GitHub Pages
    ├── index.html       ← 랜딩 페이지
    ├── watch/index.html ← 워치 앱 시뮬레이터
    ├── user/index.html  ← 사용자 모바일 대시보드
    └── admin/index.html ← 관리자 웹 대시보드
```

## ⚙️ 기술 스택

| 영역 | 기술 |
|:-----|:-----|
| 프론트엔드 | HTML5 + CSS3 + Vanilla JS |
| AI 대화 | Google Gemini API |
| 운동 DB | 농진청 예방운동 210개 |
| 디자인 | 토스 스타일 + 고령 농업인 UI 7대 원칙 |
| 폰트 | Pretendard Variable |

## 📄 라이선스

비상업적 데모 목적. NH 오픈이노베이션 제안서 첨부용.

---

**팜러닝** © 2026
