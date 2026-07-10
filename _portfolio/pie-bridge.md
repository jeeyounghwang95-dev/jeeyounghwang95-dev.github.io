---
title: "PIE BRIDGE"
excerpt: "An AI-powered educational web app that lets elementary students experience an inspectable Vision-Language-Action (VLA) workflow<br/><img src='/images/pie-bridge-screenshot.png'>"
collection: portfolio
---

![PIE BRIDGE app screen — Make a Plan step](/images/pie-bridge-screenshot.png)

## Overview
AI is rapidly expanding into physical environments through Vision-Language-Action (VLA) systems. However, primary robotics education remains largely rule-based, while existing AI education often emphasizes AI *use* rather than understanding AI *reasoning*. PIE BRIDGE was built to address this gap as a VLA-inspired educational web application for primary students.

PIE BRIDGE serves as a pedagogical bridge between physical computing and physical AI education by simulating an inspectable VLA workflow through visible stages of Vision, Language, and Action. The system supports human-AI co-piloting by allowing students to review and revise AI decisions throughout the process.

To accommodate classroom technical constraints and current vision model limitations, the system uses a discrete workflow rather than a continuous loop and restricts robot movements to a grid-board environment. A two-round modified Delphi study with ten experts yielded consensus across all domains, validating PIE BRIDGE as a pedagogically robust VLA-inspired learning environment for primary school students.

## Tech Stack
- **Frontend**: React, Vite, TailwindCSS
- **Backend**: FastAPI, Uvicorn
- **AI/RAG**: Google Gemini-family models, LangChain, ChromaDB (RAG vector search)
- **Data**: SQLite (student behavior logs), structured JSON logging
- **Deployment**: Vercel (frontend), Render (backend)

## Key Features
- Inspectable VLA workflow simulation with visually distinct Vision → Language → Action stages
- Human-AI co-piloting: students can review and revise the AI's decisions (vision recognition, language interpretation, action plan) at every stage
- Discrete, grid-board-constrained robot movement to work within classroom constraints and current vision-model limits
- RAG-based (ChromaDB) retrieval for grounded learning content and responses
- Safety filtering tailored to a child-facing product, plus multilingual (i18n) UI

## Research Validation
Validated through a two-round modified Delphi study with ten experts, reaching consensus across all domains on PIE BRIDGE's pedagogical soundness as a VLA-inspired learning environment for primary students.

## My Role
- Full-stack design and implementation of both frontend and backend
- Designed the UX and RAG pipeline around the Vision-Language-Action workflow
- Designed the system to support the Delphi study and incorporated expert review feedback

## Links
- [GitHub](https://github.com/jeeyounghwang95-dev/PIE-Bridge)
