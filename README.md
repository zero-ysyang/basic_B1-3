## ⚡자동화 도구 비교 구현 (Make vs Zapier)

### 워크플로우: "Google Form 제출 → Google Sheets 기록 -> 조건 분기(유형 기준) → Discord 알림

### [Make 구현]
- Trigger: Google Forms – Watch Responses   
- Action 1: Google Sheets – Add a Row            
- Filter : 긴급 요청만 통과
- Action 2: Discord – Send a Message

### [Zapier 구현]
- Trigger: Google Forms – New Form Response
- Action 1: Google Sheets – Create Spreadsheet Row
- Filter: 긴급 요청만 통과
- Action 2: Discord – Send Channel Message


## 📊 비교 항목

| 항목 | Make (구 Integromat) | Zapier |
|------|----------------------|--------|
| **UI/UX** | 시각적 플로우차트 방식의 캔버스 UI.<br>노드를 연결하는 방식으로 전체 흐름을 한눈에 파악 가능. | 단계별 리스트(Step-by-Step) 방식의 UI.<br>직관적이고 단순하여 처음 사용자도 빠르게 적응 가능. |
| **설정 난이도** | 중~고급. 복잡한 분기·반복·필터 처리에 강하지만<br>초보자에게는 진입 장벽이 있음. | 낮음. 트리거→액션 구조가 단순하여<br>비개발자도 수분 내 자동화 구성 가능. |
| **연동 서비스 범위** | 1,000개 이상의 앱 연동 지원.<br>HTTP/Webhook 모듈로 미지원 서비스도 커스텀 연동 가능. | 7,000개 이상의 앱 연동 지원.<br>업계 최다 수준의 서드파티 앱 커버리지 보유. |
| **무료 플랜** | 월 1,000 오퍼레이션(작업 단위), 시나리오 수 제한 없음.<br>5분 간격 실행 주기 지원. | 월 100 태스크(작업 단위), Zap 5개 제한.<br>단일 단계(Single-Step) Zap만 무료 제공. |
| **실행 로그** | 시나리오별 상세 실행 이력 제공.<br>각 모듈의 입출력 데이터를 단계별로 확인 가능하여 디버깅에 유리. | Zap별 실행 이력 및 오류 로그 제공.<br>무료 플랜은 로그 보관 기간이 제한됨(7일). |
