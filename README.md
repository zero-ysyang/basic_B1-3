## ⚡자동화 도구 비교 구현 (Make vs Zapier)

### 워크플로우: "Google Form 제출 → Google Sheets 기록 -> 조건 분기(유형 기준) → Discord 알림

### [Make 구현]
- Trigger: Google Forms – Watch Responses   
- Action 1: Google Sheets – Add a Row            
- Filter : 긴급 요청만 통과
- Action 2: Discord – Send a Message

<img width="1423" height="762" alt="Make 워크플로우" src="https://github.com/user-attachments/assets/8ea76f20-174e-48d9-a48a-f977f2bf4965" />
<img width="569" height="494" alt="4 필터조건" src="https://github.com/user-attachments/assets/29810367-3bc0-4918-9a06-943d483ee75e" />



### [Zapier 구현]
- Trigger: Google Forms – New Form Response
- Action 1: Google Sheets – Create Spreadsheet Row
- Filter: 긴급 요청만 통과
- Action 2: Discord – Send Channel Message

<img width="895" height="689" alt="Zapier 워크플로우" src="https://github.com/user-attachments/assets/ac4d718e-b731-40f4-a31a-9116bc8e78a2" />

---


## 실행 결과 화면

### 1. Google Forms

<img width="671" height="874" alt="1 설문작성" src="https://github.com/user-attachments/assets/ed300fc6-08f5-4d44-8f0e-f723c3e648a2" />

<br><br>

### 2. Google Sheets

<img width="590" height="233" alt="2 엑셀저장" src="https://github.com/user-attachments/assets/ed5f3864-72ad-4b7e-b4f1-b52d4c06a4f6" />

<br><br>

### 3. Discord

<img width="528" height="303" alt="3 디스코드 메시지(Make)" src="https://github.com/user-attachments/assets/bfeb1c99-7c98-4ba0-9a8c-c8b5d988bd7c" />
<img width="503" height="287" alt="3 디스코드 메시지(Zapier)" src="https://github.com/user-attachments/assets/0bf0f201-515b-472e-8f36-3e16e1d4501d" />

<br><br>

---

## 📊 비교 항목

| 항목 | Make (구 Integromat) | Zapier |
|------|----------------------|--------|
| **UI/UX** | 시각적 플로우차트 방식의 캔버스 UI.<br>노드를 연결하는 방식으로 전체 흐름을 한눈에 파악 가능. | 단계별 리스트(Step-by-Step) 방식의 UI.<br>직관적이고 단순하여 처음 사용자도 빠르게 적응 가능. |
| **설정 난이도** | 중~고급. 복잡한 분기·반복·필터 처리에 강하지만<br>초보자에게는 진입 장벽이 있음. | 낮음. 트리거→액션 구조가 단순하여<br>비개발자도 수분 내 자동화 구성 가능. |
| **연동 서비스 범위** | 1,000개 이상의 앱 연동 지원.<br>HTTP/Webhook 모듈로 미지원 서비스도 커스텀 연동 가능. | 7,000개 이상의 앱 연동 지원.<br>업계 최다 수준의 서드파티 앱 커버리지 보유. |
| **무료 플랜** | 월 1,000 오퍼레이션(작업 단위), 시나리오 수 제한 없음.<br>5분 간격 실행 주기 지원. | 월 100 태스크(작업 단위), Zap 5개 제한.<br>단일 단계(Single-Step) Zap만 무료 제공. |
| **실행 로그** | 시나리오별 상세 실행 이력 제공.<br>각 모듈의 입출력 데이터를 단계별로 확인 가능하여 디버깅에 유리. | Zap별 실행 이력 및 오류 로그 제공.<br>무료 플랜은 로그 보관 기간이 제한됨(7일). |

<br><br>

## ✅ 장단점 정리

| 구분 | Make (구 Integromat) | Zapier |
|------|----------------------|--------|
| **👍장점**| 시각적 캔버스 UI로 복잡한 흐름도 한눈에 파악 가능 | 트리거→액션 구조가 단순하여 누구나 빠르게 설정 가능 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| 복잡한 분기·반복·필터 등 고급 로직 구현 가능 | 업계 최다 수준의 앱 연동 지원 (7,000개+) |
| | 무료 플랜에서 월 1,000 오퍼레이션 제공 (Zapier 대비 넉넉함) | 비개발자·입문자도 수 분 내 자동화 구성 가능 |
| | HTTP/Webhook 모듈로 미지원 서비스도 커스텀 연동 가능 | 공식 문서 및 커뮤니티가 풍부하여 레퍼런스 찾기 쉬움 |
| | 실행 로그에서 각 모듈의 입출력 데이터를 상세히 확인 가능 | AI 기반 자동화 추천 기능 제공 |
| **👍단점**| 초보자에게 진입 장벽이 높음 | 무료 플랜이 월 100 태스크, Zap 5개로 매우 제한적 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| 연동 앱 수가 Zapier 대비 적음 (약 1,000개+) | 복잡한 로직(분기·반복) 구현이 어렵고 유료 플랜 필요 |
| | 한국어 공식 지원 미흡 | 요금제가 비교적 비싼 편 |
| | 복잡한 시나리오 설계 시 학습 시간이 많이 필요 | 무료 플랜은 실행 로그 보관 기간이 7일로 짧음 |

<br><br>

## 💡 한눈에 보는 선택 가이드

| 상황 | 추천 도구 |
|------|-----------|
| 처음 자동화를 시작하는 경우 | ✅ **Zapier** |
| 복잡한 데이터 처리·분기가 필요한 경우 | ✅ **Make** |
| 최대한 많은 앱과 연동해야 하는 경우 | ✅ **Zapier** |
| 무료로 최대한 활용하고 싶은 경우 | ✅ **Make** |
| 개발 지식 없이 빠르게 구축해야 하는 경우 | ✅ **Zapier** |
| 세밀한 디버깅과 로그 분석이 필요한 경우 | ✅ **Make** |

> 💬 **정리**
> - **Make** → 복잡한 자동화 시나리오, 세밀한 데이터 제어가 필요한 **중급~고급 사용자**에게 적합
> - **Zapier** → 빠른 설정과 폭넓은 앱 연동이 필요한 **입문자 및 비개발자**에게 적합
