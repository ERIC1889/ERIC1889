# 허준영

**백엔드 중심 풀스택 개발자** · 주식회사 Finz Labs 개발 총괄 · 한신대학교 소프트웨어전공

**문제를 이해하는 것에서 시작해, 신뢰할 수 있는 결과로 완성합니다.**

사용자의 불편을 이해하고 요구를 기술적 해결책으로 구체화하고, 이를 실제 작동하는 서비스로 구현해온 백엔드 개발자 허준영입니다. JavaScript와 TypeScript 중심으로 화면, 서버, AI 기능을 연결하며 제품 개발의 여러 단계를 경험했습니다. 개발 과정에서는 기술을 선택한 이유와 구현한 결과를 어떻게 확인할 수 있는지를 중요하게 생각합니다.

주식회사 Finz Labs에 초기 창업 멤버이자 회사 내 유일한 개발자로 함께해 세금 계산 서비스 [finz.kr](https://www.finz.kr)을 설계·개발·운영하고, 모바일 앱을 만들고, 협력 개발사와 세무사용 서비스의 설계와 검증을 진행했습니다. 학부에서는 WebDB 랩장과 AID 랩 학부 연구생으로 활동하며 프로젝트 17개, 학술대회 논문 7편(국제 1편 · 1저자 6편), 수상 13건을 쌓았습니다.

<a href="https://junyoung-portfolio.vercel.app"><img alt="Portfolio" src="https://img.shields.io/badge/Portfolio-18181B?style=flat-square" height="24" /></a> <a href="https://www.finz.kr"><img alt="finz.kr" src="https://img.shields.io/badge/finz.kr-18181B?style=flat-square" height="24" /></a>

## 기술

| 영역 | 기술 | 한 일 |
|---|---|---|
| 웹·API | `JavaScript` `TypeScript` `React` `Next.js` `Node.js` `Express` | 세금 계산기 화면과 API, 시세·환율 데이터 연동과 대체 조회, 공공 API 7종 정규화, 공통 컴포넌트 기반 화면 개편 |
| Python 백엔드 | `Python` `FastAPI` | 간편인증 상태 흐름, 서버 권한·결제 검증, 세금 계산 엔진 |
| 데이터 | `MySQL` `PostgreSQL` `MongoDB` | 정형 데이터와 AI 결과 분리 저장, 같은 요청의 AI 결과 재사용, 확정된 시세·환율만 캐시 |
| 실시간·배치 | `Fastify` `Socket.IO` `node-cron` | 발표 음성 스트리밍과 5초 단위 판정, 공공 데이터 주기 동기화 |
| AI 응용 | `OpenAI API` `Whisper` `PyTorch` | LLM 응답을 서버에서 검증, 음성 입력, 이미지 분류 모델 학습과 서버 추론 |
| 실행·배포 | `Expo` `Docker` `GitHub Actions` `Vercel` | Finz · Pitches · ClosetMate 모바일 앱, 로컬·Docker 실행, push마다 도는 보안 테스트, 이 포트폴리오의 Vercel 배포 |

## 실무 경험

### [주식회사 Finz Labs · 개발 총괄](https://junyoung-portfolio.vercel.app/projects/finz) · 2026.01–

직원 5명 스타트업. 부동산·디지털 자산·해외주식 세금 계산기가 있는 회사 웹 finz.kr을 혼자 설계·개발·운영하고, Finz 모바일 앱(청년 세금 환급 MVP)을 만들었으며, 세무사용 FINZ의 개발·배포·운영 준비를 협력 개발사와 함께 진행했습니다.

- **회사 웹 finz.kr 설계·개발·운영** — 세금 계산기 4종 운영 중, 저장소 테스트 192개 통과. 세무사와 함께 만든 6Way 계산 로직을 Python에서 TypeScript로 옮겨 기준 사례 21개 항목을 대조했고 최대 차이는 1원
- **Finz 모바일 앱** (Expo · FastAPI, 미출시) — 간편인증 1번으로 5개 연도 조회, 보안 단위 테스트 57개. 2026 AI-SW중심대학 AI·블록체인 비즈니스모델 경진대회 우수상
- **세무사용 FINZ** (협력 개발사와 공동 개발) — 완료 보고 269건 재검증·새 결함 45건, 배포 9번 연속 실패 원인 재현

개발 환경: Next.js · TypeScript · React · Vitest · Expo · FastAPI

## 대표 프로젝트

### [SkillPilot 자격증·커리어 플랫폼](https://junyoung-portfolio.vercel.app/projects/skillpilot) · [코드](https://github.com/ERIC1889/SkillPilot) · 2025.09–2026.06

흩어진 IT 자격증 정보를 한곳에 모으고, 자격증 선택부터 학습, 모의시험, 면접 준비까지 이어 주는 웹 서비스. 4인 캡스톤에서 팀장 · 백엔드 전체 · 프론트엔드 개편을 맡았습니다.

- **문제 해결** — HTTP 200 응답에 포함된 공공 API 오류: 상태 코드만으로 성공 여부 판단 불가 → 공통 API 클라이언트에 본문 검사와 재시도 추가 / XML·JSON 등 제각각인 응답 구조 → 공통 클라이언트 1개와 정규화 함수 7개로 처리 단계 분리
- **결과** — 공공데이터 API 7종을 하나의 자격증 데이터로 정규화하고 스케줄러가 자동 갱신(전체 613종목 중 IT 34종목 · 시험 일정 87건) · AI 호출이 실패해도 규칙 기반 대체 응답으로 온보딩 유지 · 13개 화면 · 16개 라우트 모듈로 캡스톤 완료
- 개발 환경: Node.js · Express 5 · MySQL · MongoDB · OpenAI API · node-cron · React 19

### [Pitches 발표 코칭](https://junyoung-portfolio.vercel.app/projects/pitches) · [코드](https://github.com/ERIC1889/pitches) · 2024.10–2026.10

발표하는 동안 말 속도·감정·음량을 분석해 색으로 바로 알려 주고, 발표가 끝나면 AI 코칭 보고서를 만들어 주는 모바일 서비스. 2024 해커톤 팀(팀장 · 백엔드·AI) → 2025 논문 → 2026 개인 리뉴얼(전체).

- **문제 해결** — 실시간 피드백이 멈추지 않는 구조: 분석 대기로 인한 지연 → 동시 요청, 제한 시간, 실패 처리 / 무음·잡음 구간: Whisper가 무음에서 전사를 만들어 내는 문제 → 무음은 호출 전에 건너뛰고 지어낸 문구는 호출 후 제거
- **결과** — 캡스톤 디자인 및 AI 해커톤 대상(1등, 2024.10) · SW중심대학 AI 창업 아이디어 경진대회 특별상(2025.05) · APIC-IST 2025 국제학술대회 논문 · 5초 단위 분석과 색 표시로 즉시 피드백(음성→지표 지연 평균 125ms, 동시 20세션 최악 170ms) · 사용자 조사 5명 모두 도움이 된다고 응답
- 개발 환경: Fastify · Socket.IO · BullMQ · PostgreSQL · Whisper · SenseVoice-Small · GPT-5-nano · Expo

### [ClosetMate 옷장·코디 추천 앱](https://junyoung-portfolio.vercel.app/projects/closetmate) · [코드](https://github.com/ERIC1889/ClosetMate) · 2026.03–2026.06

옷 사진을 찍으면 종류·색상·스타일을 분류해 옷장에 넣고, 말이나 글로 상황을 입력하면 가진 옷으로만 코디를 추천하는 모바일 앱. 기획 · 모델 학습 · 모바일·API 개발을 혼자 했습니다.

- **문제 해결** — 옷장에 없는 옷을 추천하는 LLM: 없는 옷 ID나 만들 수 없는 조합 생성 → 규칙으로 후보를 만들고 LLM은 후보 중에서만 선택, 서버에서 형식·옷 ID·조합 검증 / 분류 모델 선택: 모바일에서 빠르게 돌아갈 모델 필요 → MobileNetV3-Small과 ResNet50 동일 조건 비교, 헤드 3개를 얹은 MobileNetV3를 서버에서 ONNX로 추론
- **결과** — 가진 옷으로만 추천: 실측 23회 중 기본 모델 통과 19회 · 보조 모델 처리 4회 · 최종 실패 0건 · 사진 등록 → 분류 → 후보 생성 → LLM 추천 → 서버 검증 전체 흐름 구현 · 약 15분의 1 크기(6.0MB 대 90.2MB)의 MobileNetV3-Small 채택
- 개발 환경: Expo · Next.js · PostgreSQL · Drizzle · ONNX Runtime · PyTorch · OpenAI API · Whisper

## AI와 일하는 방식

Claude Code · Codex · Antigravity를 거의 매일, 역할을 나눠 씁니다. 구현 속도는 AI에 기대되, 무엇을 만들지, 어떤 구조로 갈지, 결과를 내보낼지는 제가 정하고, 내보낸 결과는 제가 책임집니다.

- **Claude Code** 구현 · 기획과 문서 / **Codex** 코드 리뷰 · 문제점 파악 · 전체 리뷰 / **Antigravity** 디자인
- 기획 → 설계(결정은 나) → 구현 · 디자인 → AI ↔ AI 교차 리뷰 → 직접 검토 · 보완 → 자동 테스트 + 직접 검증
- API 키는 도구에 보여 주지 않고, 고객 데이터는 가린 뒤에 넘깁니다. 자세한 내용은 [포트폴리오의 "AI와 일하는 방식"](https://junyoung-portfolio.vercel.app/#ai)

## 다른 프로젝트

- **[EduMatrix](https://junyoung-portfolio.vercel.app/projects/edumatrix)**: 목표, 노트, 퀴즈, 피드백, 계획 조정을 잇는 AI 학습 지원 시스템의 구상과 설계 (4인 캡스톤, 1저자 논문 2편)
- **[InnoView](https://junyoung-portfolio.vercel.app/projects/innoview)** · [코드](https://github.com/ERIC1889/InnoView): 이력서와 직무에 맞춰 질문하고 음성·텍스트·영상으로 답변을 분석하는 모의 면접 서비스 (기업·직무별 Assistant, 꼬리 질문은 서버에서 15문항 제한)
- **[Label Light](https://junyoung-portfolio.vercel.app/projects/label-light)**: 설문 대신 음성만으로 나누는 일상 대화 속에서 노인 우울 척도(GDS) 문항을 끌어내는 음성 챗봇 (1저자 논문)

[전체 프로젝트 보기](https://junyoung-portfolio.vercel.app/archive#projects)

## 수상 · 총 13건

| 날짜 | 수상 | 프로젝트 |
|---|---|---|
| 2026.05 | 2026년 AI-SW중심대학 AI·블록체인 비즈니스모델 경진대회 우수상 | Finz |
| 2025.11 | 2025 한신 AISW 페스티벌 캡스톤 디자인 부문 특별상 | EduMatrix |
| 2025.11 | 2025년도 추계종합학술대회 및 대학생 논문경진대회 은상 (한국디지털콘텐츠학회) | EduMatrix |
| 2025.05 | SW중심대학 AI 창업 아이디어 경진대회 특별상 | Pitches |
| 2024.10 | 캡스톤 디자인 및 AI 해커톤 대상(1등) | Pitches |

외 8건 · [전체 기록](https://junyoung-portfolio.vercel.app/archive)

## 경험 · 활동 · 논문

- **CES 2026 참관** (2026.01) — 한신대 학생 대표로 라스베가스 세계 전자제품 박람회 참관
- **한신대 AI 면접 특강 진행** (2025.10) — AI 면접 서비스 InnoView 소개 특강 2회, 학생 직접 사용 · 쏘랩 시연(2025.11)
- **WebDB 랩장** (2025.01–2026.07) — 학부 연구실 운영 총괄, 연구실 프로젝트 기획·관리
- **SW 인재 페스티벌** (2024.12) — 학교 대표로 부스 운영과 작품 출품
- **AID 랩실 학부 연구생** (2024.01–2025.06) — LLM 서비스 연구, Label Light 연구(1저자 논문 · 논문경진대회 동상)
- **웹 프로그래밍 멘토링 멘토 · 스터디 리더** (2023–2025, 3학기) — 후배 웹 개발 학습 지원

외 11건 · 논문은 학술대회 7편(국제 1 · 1저자 6)과 공모전·교내 3편 — *Pitches: Real-Time Presentation Coaching with Low-Latency Speech Analysis and Generative AI* (APIC-IST 2025, 2저자) · A2A 협업 기반 웰니스 일정 관리 시스템 (한국정보통신학회 2026, 1저자) · 개인 맞춤형 AI 학습 비서 시스템: EduMatrix 설계 및 제작 (한국디지털콘텐츠학회 2025, 1저자) 외 7편

[수상 · 논문 · 활동 전체 보기](https://junyoung-portfolio.vercel.app/archive)
