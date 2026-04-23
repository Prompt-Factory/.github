# PromptFactory

> 크리에이터와 브랜드를 AI로 연결하는 크리에이티브 플랫폼

PromptFactory는 크리에이터의 포트폴리오를 탐색하고, 브랜드·에이전시의 비즈니스 맥락에 맞는 크리에이터를 AI로 매칭하는 플랫폼을 만듭니다. 마케팅 기획 단계부터 크리에이티브 제작까지, 그 사이에 존재하던 마찰을 데이터와 AI로 줄이는 것이 우리의 과제입니다.

대외적으로는 **PFAC**, 내부적으로는 **Nexus**라는 코드네임으로 플랫폼을 운영합니다.

## Services

| 서비스 | 설명 | 주소 |
|---|---|---|
| **PFAC Platform** | 크리에이터 탐색·포트폴리오·컬렉션을 제공하는 메인 웹 서비스 | [www.promptfactory.dev](https://www.promptfactory.dev) |
| **AE Workbench** | 3C · SWOT · 포지셔닝 기반 AI 광고 전략 분석 진입점 | — |

## Tech

- **Frontend** — Next.js, React, TypeScript, Turborepo (pnpm)
- **Backend** — FastAPI (Python)
- **Data** — DynamoDB · OpenSearch (시맨틱 검색) · S3 + CloudFront
- **AI** — AWS Bedrock (Claude), OpenAI
- **Infra** — Docker · AWS ECS Fargate · CodePipeline

## Nexus — 플랫폼 운영 헌법

Nexus는 PromptFactory 플랫폼의 **도메인 경계 · 아키텍처 규칙 · 데이터 계약**을 단일 진실의 원천으로 관리하는 문서 체계입니다. 모든 서비스는 Nexus에 명시된 규칙과 스펙을 기준으로 구현되며, 문서가 코드보다 먼저 갱신되도록 운영합니다.

## Contact

- Web — [promptfactory.pro](https://promptfactory.pro)
- Email — [info@promptfactory.pro](mailto:info@promptfactory.pro)
