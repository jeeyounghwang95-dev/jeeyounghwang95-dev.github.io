---
title: "PIE BRIDGE"
excerpt: "Vision-Language-Action(VLA) 워크플로우를 체험시키는 초등 피지컬 AI 교육용 웹 애플리케이션<br/><img src='/images/pie-bridge-screenshot.png'>"
collection: portfolio
---

![PIE BRIDGE app screen — Make a Plan step](/images/pie-bridge-screenshot.png)

## 개요
AI는 Vision-Language-Action(VLA) 시스템을 통해 빠르게 물리적 환경으로 확장되고 있지만, 초등 로보틱스 교육은 여전히 규칙 기반(rule-based)에 머물러 있고, 기존 AI 교육은 AI 추론 과정에 대한 이해보다 AI 활용에 초점을 맞추는 경우가 많습니다. PIE BRIDGE는 이러한 간극을 메우기 위해 개발한 VLA 영감 기반 초등 교육용 웹 애플리케이션입니다.

PIE BRIDGE는 Vision → Language → Action의 각 단계를 눈으로 확인할 수 있는 형태로 구현하여, 검증 가능한(inspectable) VLA 워크플로우를 시뮬레이션함으로써 피지컬 컴퓨팅 교육과 피지컬 AI 교육 사이를 잇는 교육적 다리 역할을 합니다. 학생이 전 과정에서 AI의 판단을 검토하고 수정할 수 있도록 하는 인간-AI 협업(co-piloting) 방식을 지원합니다.

교실 환경의 기술적 제약과 현재 비전 모델의 한계를 고려해, 연속적인 루프 대신 이산적(discrete) 워크플로우를 채택했고, 로봇의 이동은 그리드 보드 환경으로 제한했습니다. 10인의 전문가가 참여한 2라운드 수정 델파이(Delphi) 연구를 통해 전 영역에서 합의를 도출했으며, 이를 통해 PIE BRIDGE가 초등학생을 위한 교육학적으로 견고한 VLA 영감 학습 환경임을 검증했습니다.

## 기술 스택
- **프론트엔드**: React, Vite, TailwindCSS
- **백엔드**: FastAPI, Uvicorn
- **AI/RAG**: Google Gemini 계열 모델, LangChain, ChromaDB(RAG 벡터 검색)
- **데이터**: SQLite(학생 행동 로그), 구조화된 JSON 로깅
- **배포**: Vercel(프론트엔드), Render(백엔드)

## 주요 기능
- Vision → Language → Action 단계를 시각적으로 구분해 보여주는 검증 가능한 VLA 워크플로우 시뮬레이션
- 학생이 AI의 판단(비전 인식 결과, 언어 해석, 행동 결정)을 매 단계 검토·수정할 수 있는 인간-AI 협업 구조
- 그리드 보드 기반의 제한된 이산적 로봇 이동으로 교실 환경 제약과 비전 모델 한계 보완
- RAG(ChromaDB) 기반 학습 콘텐츠 검색 및 응답
- 아동 대상 서비스에 맞춘 안전 필터링, 다국어(i18n) 지원

## 연구적 검증
10인의 전문가를 대상으로 한 2라운드 수정 델파이 연구를 통해 전 영역에서 합의를 도출, 초등학생 대상 VLA 영감 학습 환경으로서의 교육학적 타당성을 검증했습니다.

## 나의 역할
- 프론트엔드/백엔드 풀스택 설계 및 구현
- VLA 워크플로우(Vision-Language-Action)를 반영한 UX 및 RAG 파이프라인 설계
- 델파이 연구를 위한 시스템 설계 및 전문가 검토 반영

## 링크
- [GitHub](https://github.com/jeeyounghwang95-dev/PIE-Bridge)
