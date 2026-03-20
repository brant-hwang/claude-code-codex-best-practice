# AI 코딩 에이전트 셋업 가이드

> **Claude Code + Codex + gstack + Ralph** — AI 코딩 에이전트를 구조화된 가상 개발팀으로 만드는 완전 가이드.

**<a href="https://ai-coding-guide-with-gstack.vercel.app" target="_blank">가이드 보러가기</a>**

<a href="https://ai-coding-guide-with-gstack.vercel.app/ai-coding-setup-guide-ko.html" target="_blank">한국어</a> | <a href="https://ai-coding-guide-with-gstack.vercel.app/ai-coding-setup-guide-en.html" target="_blank">English</a> | <a href="https://ai-coding-guide-with-gstack.vercel.app/ai-coding-setup-guide-ja.html" target="_blank">日本語</a>

---

## 이게 뭔가요?

대부분의 개발자는 AI 코딩 에이전트를 고급 자동완성 정도로 씁니다. 이 가이드는 AI 에이전트를 **역할이 분리된 개발팀**처럼 운영하는 방법을 알려줍니다 — 기획, 구현, 리뷰, QA, 배포를 각각 전문화된 워크플로로 처리합니다.

처음부터 끝까지 다룹니다:

1. **기초 환경** — 터미널, 셸, Homebrew, Node.js, 에디터 설정
2. **Claude Code** — 설치, 설정, CLAUDE.md 작성법, 서브 에이전트 워크플로
3. **Codex** — OpenAI의 CLI 에이전트를 세컨드 오피니언 & 코드 리뷰어로 활용
4. **MCP 서버** — 브라우저, GitHub, Slack 등과 에이전트 연결
5. **gstack** — 개발 프로세스를 강제하는 스킬 기반 워크플로 엔진
6. **CLAUDE.md / AGENTS.md** — 프로덕션 수준의 프롬프트 설정
7. **Ralph (Ouroboros)** — 스펙 우선 자율 개발 루프
8. **부록** — Claude Code 내부 구조, `.claude/` 디렉토리, 훅, 퍼미션

## 누구를 위한 가이드인가요?

- AI 기반 개발에 **구조와 프로세스**가 필요한 **창업자 / 테크리드**
- Claude Code, Codex, gstack을 처음 접하는 **개발자**
- "AI랑 채팅"을 넘어 "AI를 팀처럼 운영"하고 싶은 **모든 분**

## 네비게이션

슬라이드 형식의 프레젠테이션입니다:

- **방향키** (상하좌우 모두), **Space**, **PageUp/Down**
- **마우스 휠** (세로 스크롤이 좌우 슬라이드 이동에 매핑)
- 모바일에서는 **터치 스와이프**

---

**제작: [Brant Hwang](mailto:brant@querypie.com)** — [QueryPie AI](https://www.querypie.com) 대표
