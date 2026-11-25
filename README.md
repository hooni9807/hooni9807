## 안녕하세요, AI 개발자 김세훈입니다

**보이지 않는 것은 읽어 주고, 보여선 안 되는 것은 가립니다.**

시각장애인의 일상(화장, 장보기, 옷 고르기, 식사, 음료 고르기)을 음성·OCR·비전 AI로 돕는 서비스를 만들어 왔고, 지금은 문서 속 개인정보가 빠짐없이 가려졌는지 검증하는 도구를 만들고 있습니다.

### [포트폴리오 열기 → hooni9807.github.io/portfolio](https://hooni9807.github.io/portfolio/)


---

### 읽어 주기: 시각장애인 보조 AI

| 기간 | 프로젝트 | 핵심 기술 |
|---|---|---|
| 2026.10&nbsp;~&nbsp;2026.11 | [What Is This?](https://hooni9807.github.io/portfolio/#whatisthis) · 손끝이 가리킨 음료를 읽어 주는 모바일 웹 | MediaPipe, PaddleOCR, DINOv2 |
| 2026.10&nbsp;~&nbsp;2026.11 | [소리한상](https://hooni9807.github.io/portfolio/#sorihansang) · 가리킨 반찬과 옮겨진 반찬을 알려 주는 식사 안내 | Gemma 4, MediaPipe |
| 2026.11&nbsp;~&nbsp;2026.12 | [손끝옷장](https://hooni9807.github.io/portfolio/#closet) · 말과 사진으로 등록하는 음성 옷장 도우미 | Gemma 4, GPT API, 기상청 API |
| 2025.09&nbsp;~&nbsp;2025.12 | [편하CU](https://hooni9807.github.io/portfolio/#pyeonhacu) · 편의점 행사 상품 음성 안내 앱 | OCR, Gemma3, Android |
| 2025.03&nbsp;~&nbsp;2025.07 | [뷰티프렌즈](https://hooni9807.github.io/portfolio/#beautyfriends) · 메이크업 도우미 | Gemma3, OpenCV |

### 가리기: 문서 비식별 검증 (인턴십 · 지란지교 1연구소 AI연구팀)

| 기간 | 프로젝트 | 핵심 기술 |
|---|---|---|
| 2026.10&nbsp;~&nbsp;2026.11 | [Crawling‑Document‑Data](https://hooni9807.github.io/portfolio/#cdd) · 공공문서 실제 샘플 수집기 | Playwright, pytest |
| 2026.10&nbsp;~&nbsp;2026.11 | [라벨링 클릭 매크로](https://hooni9807.github.io/portfolio/#macro) · KNN으로 화면을 보정하는 클릭 매크로 | k-NN, OpenCV ORB·RANSAC |
| 2026.09&nbsp;~&nbsp;2026.12 | [문서 비식별 자동 테스트](https://hooni9807.github.io/portfolio/#deid) · 시험 문서 생성과 마스킹 회귀 테스트 | Python, Docker, FastAPI |

### 그 밖의 프로젝트

| 기간 | 프로젝트 | 구분 |
|---|---|---|
| 2026.10&nbsp;~&nbsp;2026.11 | [문장곁](https://hooni9807.github.io/portfolio/#munjang) · 자기소개서 비교·편집과 AI 면접관 피드백 | 개인 |
| 2026.03&nbsp;~&nbsp;2026.06 | [모르는거없쌤](https://hooni9807.github.io/portfolio/#aitutor) · RAG 기반 AI 튜터 | 팀 |
| 2024.09&nbsp;~&nbsp;2025.02 | [레포트메이트](https://hooni9807.github.io/portfolio/#reportmate) · LLM 자료 조사 협업 플랫폼 | 팀 |

프로젝트 이름을 누르면 포트폴리오의 해당 설명으로 바로 이동합니다. 시연 영상, 설계 결정, 측정 결과는 포트폴리오에 정리했습니다.

---

### 어떻게 만들었는지

레포마다 README에 **왜 만들었나 → 설계 → 단계별 개발 과정 → 트러블슈팅** 순서로 정리했습니다. 개발 과정은 실제 커밋 기록에서 뽑았습니다.

| 프로젝트 | 기간 · 커밋 | 개발 과정 |
|---|---|---|
| [문서 비식별 자동 테스트](https://hooni9807.github.io/portfolio/#deid) | 2026.09.14&nbsp;~&nbsp;11.25&nbsp;·&nbsp;175 | 형식별 시험 문서 생성(1차 14개 형식) → OLE 196조합·확장 기능(2·3차) → 기대값 사전 계산과 OCR 캐시 → 추가 확장 1~5안(암호·대용량·레거시·비정상 PDF·OOXML) → Claude 스킬·웹 콘솔 |
| [라벨링 클릭 매크로](https://hooni9807.github.io/portfolio/#macro) | 2026.11.11&nbsp;~&nbsp;11.25&nbsp;·&nbsp;77 | 클릭 기록·재생 → ORB·RANSAC 화면 보정과 안전장치 → 정답 클릭 자동 기록 → KNN으로 가장 닮은 기준 화면 고르기 → 양식 자동 분류와 설정 학습 |
| [Crawling‑Document‑Data](https://hooni9807.github.io/portfolio/#cdd) | 2026.11.24&nbsp;~&nbsp;11.25&nbsp;·&nbsp;41 | 포털 다운로드 요청 분석 → 기관 사이트 Playwright 수집 → 시그니처로 진짜 형식 판별·중복 제거 → 웹 화면·Windows 실행 파일 → 테스트 100개로 검증 |

저장소는 회사 업무와 관련되어 비공개이고, 자세한 내용은 포트폴리오에서 볼 수 있습니다. AI 코딩 도구(Claude Code)를 함께 썼습니다. 기획, 설계 결정, 시험, 최종 검토는 직접 했습니다.

---

### 기술

- **AI · LLM** · Gemma 3·4(Ollama), GPT API, Groq, LangChain RAG, Pinecone, OCR(PaddleOCR), MediaPipe, DINOv2, k-NN, Claude Code 스킬 제작
- **서버** · FastAPI, Flask, Node.js, WebSocket, JWT, MySQL, Firebase Firestore, Cloudflare Workers
- **화면 · 앱** · JavaScript, HTML/CSS, React·Redux, Electron, Android(CameraX), Swift, ONNX Runtime Web, 음성 인식·합성
- **테스트 · 도구** · Python 회귀 테스트, pytest, Playwright, 문서 형식 바이트 분석, LibreOffice, Docker, Makefile, OpenCV(ORB·RANSAC)·NumPy
