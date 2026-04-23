# PromptFactory

> 크리에이터와 비즈니스를 잇는 AI 기반 크리에이티브 플랫폼

PromptFactory는 **크리에이터 포트폴리오 탐색·검색·매칭**을 핵심으로, AI로 증폭된 비즈니스 인사이트와 함께 브랜드·에이전시·크리에이터를 연결하는 플랫폼을 만듭니다.

대외적으로는 **PFAC**, 내부적으로는 **Nexus**라는 이름으로 플랫폼을 운영하고 있습니다.

---

## 🧭 Platforms

| Surface | 역할 |
|---|---|
| **Platform Web** | 크리에이터 검색, 포트폴리오·컬렉션 탐색 (퍼블릭) |
| **Production Tool** | 작업의뢰서 작성, 크리에이터 매칭·확정 워크플로우 (어드민) |
| **AE Workbench** | 3C / SWOT / 포지셔닝 분석으로 시작하는 AI 광고 전략 엔트리포인트 |

## 🧱 Architecture

플랫폼은 7개 도메인으로 경계를 나눕니다.

| 도메인 | 책임 |
|---|---|
| Identity & Access | 계정·인증·세션·권한 |
| People | 크리에이터·클라이언트·프로젝트 |
| Discovery | 피드·컬렉션·시맨틱 검색 |
| Production | 의뢰 생성 → 제출 → 배정 → 확정 워크플로우 |
| Intelligence | LLM 기반 분석·리포트 (Bedrock / OpenAI) |
| Activity | 유저 활동 이벤트 수집·어드민 대시보드 |
| Platform Services | S3, 메일, DI, 로깅, i18n 공통 기반 |

## 🛠 Tech Stack

- **Frontend** — Next.js, Vite, React, TypeScript, Turborepo (pnpm)
- **Backend** — FastAPI, Python 3.11 / 3.13
- **Data** — DynamoDB, OpenSearch (KNN 벡터), S3 + CloudFront
- **AI** — AWS Bedrock (Claude), OpenAI
- **Infra** — Docker, AWS ECS Fargate, CodeBuild / CodePipeline

## 📚 Nexus — 플랫폼의 기반 문서

[**Nexus**](https://github.com/promptfactory/nexus)는 플랫폼 전체가 공유하는 **규칙·용어·도메인 경계·스펙**을 단일 진실의 원천으로 관리하는 문서 레포입니다. 코드는 포함되어 있지 않습니다.

- `constitution/` — 반드시 따라야 하는 코드·아키텍처·워크플로우 규칙
- `architecture/` — 시스템 구성도, 서비스 토폴로지, 인프라 상세
- `data/` — DB 스키마, API 계약, 이벤트 정의
- `modules/` — 도메인·모듈별 상세 문서
- `specs/` — 기능별 스펙 아카이브

모든 코드 레포(`frontend`, `pf-platform-api`, `insight-engine`, `creator-notification-service`, `c-dabari`)는 Nexus를 플랫폼의 계약서로 참조합니다. **nexus PR은 코드 PR보다 먼저 머지**되는 것을 원칙으로 합니다.

## 🤝 Contact

- Web — [promptfactory.pro](https://promptfactory.pro)
