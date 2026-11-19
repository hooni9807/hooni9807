## 안녕하세요, AI 개발자 김세훈입니다

**보이지 않는 것은 읽어 주고, 보여선 안 되는 것은 가립니다.**

시각장애인이 화장하고, 장을 보고, 옷을 고르는 일을 음성과 OCR로 돕는 서비스를 만들어 왔습니다.
지금은 문서 속 개인정보가 빠짐없이 가려졌는지 검증하는 도구를 만들고 있습니다.

<p>
  <a href="https://hooni9807.github.io/portfolio/"><img alt="포트폴리오 바로가기" src="https://img.shields.io/badge/%ED%8F%AC%ED%8A%B8%ED%8F%B4%EB%A6%AC%EC%98%A4_%EB%B0%94%EB%A1%9C%EA%B0%80%EA%B8%B0-3A32C8?style=for-the-badge"></a>
</p>

### 프로젝트

| 기간 | 프로젝트 | 구분 |
|---|---|---|
| 2026.11 ~ 2026.12 | [손끝옷장](https://hooni9807.github.io/portfolio/#closet) — 시각장애인용 음성 옷장 도우미 (Gemma 4 · GPT API) | 개인 |
| 2026.09 ~ 2026.12 | [문서 비식별 자동 테스트](https://hooni9807.github.io/portfolio/#deid) — 비식별 문서 생성 및 마스킹 검증 도구 | 인턴십 |
| 2026.03 ~ 2026.06 | [모르는거없쌤](https://hooni9807.github.io/portfolio/#aitutor) — RAG 기반 AI 튜터 서비스 | 팀 |
| 2025.09 ~ 2025.12 | [편하CU](https://hooni9807.github.io/portfolio/#pyeonhacu) — 생성형 AI·OCR 기반 시각장애인용 편의점 도우미 앱 | 개인 |
| 2025.03 ~ 2025.07 | [뷰티프렌즈](https://hooni9807.github.io/portfolio/#beautyfriends) — Gemma3 기반 시각장애인 메이크업 도우미 | 개인 |
| 2024.09 ~ 2025.02 | [레포트메이트](https://hooni9807.github.io/portfolio/#reportmate) — LLM 기반 자료 조사 협업 플랫폼 | 팀 |

프로젝트 이름을 누르면 포트폴리오의 해당 설명으로 바로 이동합니다.

### 브라우저에서 바로 해 볼 수 있는 것

- [SPP — Snap Ping Pong](https://playspp.site/) · 인터랙티브 탁구 게임 ([코드](https://github.com/hooni9807/spp))
- [Auto Ping Pong](https://hooni9807.github.io/auto-ping-pong/) · SPP 탁구 캐릭터로 만든 오토배틀러 ([코드](https://github.com/hooni9807/auto-ping-pong))
- [BeamRPG](https://hooni9807.github.io/beamrpg/) · 마을을 돌아다니며 성장하는 탁구 RPG ([코드](https://github.com/hooni9807/beamrpg))
- [BeamCatch](https://hooni9807.github.io/beamcatch/) · BeamRPG 캐릭터가 나오는 레트로 탐험·수집 RPG ([코드](https://github.com/hooni9807/beamcatch))

### 어떻게 만들었는지

레포마다 README에 **왜 만들었나 → 설계 → 단계별 개발 과정 → 트러블슈팅** 순서로 정리했습니다. 개발 과정은 실제 커밋 기록에서 뽑았습니다.

| 프로젝트 | 기간 · 커밋 | 개발 과정 |
|---|---|---|
| SPP | 2026.10.12 ~ 11.17 · 1,567 | [프로토타입부터 공개 가이드까지 10단계](https://github.com/hooni9807/spp#3-개발-과정) |
| SPP Android | 2026.10.12 ~ 11.09 · 1,149 | [웹 게임을 Capacitor로 앱 빌드](https://github.com/hooni9807/spp-android#3-개발-과정) |
| BeamRPG | 2026.10.12 ~ 10.16 · 317 | [개발 과정](https://github.com/hooni9807/beamrpg#3-개발-과정) |
| Auto Ping Pong | 2026.10.28 ~ 10.29 · 33 | [개발 과정](https://github.com/hooni9807/auto-ping-pong#3-개발-과정) |
| TTT | 2026.10.26 ~ 10.27 · 37 | [개발 과정](https://github.com/hooni9807/ttt#3-개발-과정) |
| BeamCatch | 2026.10.19 · 2 | [개발 과정](https://github.com/hooni9807/beamcatch#3-개발-과정) |

AI 코딩 도구(Claude Code)를 함께 썼습니다. 기획, 설계 결정, 플레이 테스트, 최종 검토는 직접 했습니다.

### 기술

- **AI · LLM** Gemma 3·4(Ollama), GPT API, Groq, LangChain RAG, Pinecone, OCR, Claude Code 스킬 제작
- **서버** FastAPI, Flask, WebSocket, JWT, MySQL, Firebase Firestore
- **화면 · 앱** JavaScript, HTML/CSS, React·Redux, Electron, Android(CameraX), 음성 인식·합성
- **테스트 · 도구** Python 회귀 테스트, 문서 형식 바이트 분석, LibreOffice, Docker, Makefile, OpenCV·NumPy
