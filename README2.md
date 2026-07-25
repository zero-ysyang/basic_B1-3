# [프로젝트 2]
## ⚡자유 주제 자동화 설계 및 구현 
<br>

### ● 반복 업무 정의 : 매일 RSS로 뉴스기사(경제)를 수집하여, 제목에 'AI' 가 있는 경우 Discord로 공유해주는 작업
<br>

### ● 선정 도구 : Make 
| NO | 선정 이유 |
|:---:|-----------|
| 1 | 시각적 플로우차트 방식으로 설계가 직관적 |
| 2 | 무료 Ops 범위 내 구현 가능 |
| 3 | 각 모듈의 입출력 데이터를 단계별로 확인하여 디버깅에 유리   |
<br>

### ● 워크플로우 설계 문서 
#### 1. RSS : 연합뉴스(경제) RSS URL 사용 (재시도전략 : 수집 실패시 15분)
#### 2. Router : 뉴스제목의 'AI' 키워드 분기     
#### 3-1. Google Sheets : 'AI' 가 포함된 경우, 'AI키워드 Sheet' 저장(일시, 제목, 내용, URL)
#### 3-2. Google Sheets : 'AI' 가 포함되지 않은 경우, '나머지 Sheet' 저장(일시, 제목, 내용, URL)  
#### 4. Discord : 3-1 처리건 Discord 채널 공유 (일자, 제목, URL)
<br>
<img width="1170" height="631" alt="image" src="https://github.com/user-attachments/assets/fbcaaaf1-593e-4656-9add-8dffb452501a" />


### ● 구현 화면 캡처
<img width="400" height="400" alt="image" src="https://github.com/user-attachments/assets/11d1697c-e9ac-4f52-a454-5bbe854a1b9b" /> <img width="400" height="400" alt="image" src="https://github.com/user-attachments/assets/f0304f55-e579-4ed5-ae1b-6a4d1d4de60a" />
<img width="722" height="583" alt="image" src="https://github.com/user-attachments/assets/c8c0f725-b833-4285-ace3-db3e19208c20" />
<img width="621" height="837" alt="image" src="https://github.com/user-attachments/assets/9ded58b8-2443-49c0-a6dd-7374c05d2dfb" />
<img width="630" height="681" alt="image" src="https://github.com/user-attachments/assets/c812cb9e-183d-4cef-8f88-3167a8a72b95" />




### ● 실행 결과 화면 캡처
<img width="1529" height="415" alt="image" src="https://github.com/user-attachments/assets/c6c96f9e-844e-482e-b24f-f0c3cea6176e" />
<img width="1529" height="505" alt="image" src="https://github.com/user-attachments/assets/75620039-3807-4a49-838b-eb570633e1c5" />
<img width="943" height="698" alt="결과화면2" src="https://github.com/user-attachments/assets/b1248a56-010a-4e2c-b8f6-b9be104cc3c3" />



