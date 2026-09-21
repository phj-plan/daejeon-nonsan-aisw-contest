# 대전·논산 AI·SW 활용 콘텐츠 경진대회 — 팀 시장에가면

> **대전 중앙시장**을 주제로 AI 캐릭터 · AI 노래 · 지역 활성화 아이디어 3개 부문에 참가한 팀 프로젝트

| 항목 | 내용 |
|---|---|
| 대회 | 대전·논산 AI·SW 활용 콘텐츠 경진대회 |
| 기간 | 2026년 9월 (9월 18일 접수 마감) |
| 팀 | **시장에가면** |
| 참가 부문 | 전체 4개 부문 중 3개 (SNS·디지털 홍보 콘텐츠 제외) |
| 담당 | **AI 캐릭터·브랜딩 콘텐츠**, **지역 활성화 아이디어 콘텐츠** |
| 결과 | 온라인 심사 중 |

## 제출 작품

| 부문 | 작품 | 제작 | 자세히 |
|---|---|---|---|
| 🚂 AI 캐릭터·브랜딩 콘텐츠 | 마스코트 「첫차」 | 직접 제작 | [character-branding](character-branding/) |
| 🎵 AI 활용 노래·음원 콘텐츠 | 「대전 중앙시장 다 있슈~」 | 팀원 제작 | [ai-song](ai-song/) |
| 🏮 지역 활성화 아이디어 콘텐츠 | 중앙시장 AI 탐험대 (모바일 웹) | 직접 기획·제작 | [regional-idea](regional-idea/) · [Live Demo](https://jungang-market-ai-explorer.netlify.app/) |

---

## 🚂 AI 캐릭터·브랜딩 콘텐츠 — 마스코트 「첫차」

<img src="character-branding/mascot-cheotcha.png" width="600">

> 경부선 대전역이 문을 열던 날, 첫 기차와 함께 내린 아이. 100년째 시장에서 손님을 맞고 있습니다.

- 대전역(역장 모자)과 중앙시장(앞치마·장바구니)을 합친 대전 중앙시장 마스코트
- 모양·색·스타일을 항목별로 지정한 프롬프트로 이미지 생성 AI를 활용해 제작

👉 [캐릭터 소개와 생성 프롬프트 보기](character-branding/README.md)

## 🎵 AI 활용 노래·음원 콘텐츠 — 「대전 중앙시장 다 있슈~」

- 대전 중앙시장을 주제로 AI를 활용해 만든 노래 (팀원 제작)
- 음원: [`ai-song/daejeon-jungang-market-song.mp3`](ai-song/daejeon-jungang-market-song.mp3)

## 🏮 지역 활성화 아이디어 콘텐츠 — 중앙시장 AI 탐험대

> 방문객의 동행·시간·예산·취향을 분석해 **대전 중앙시장 맞춤 탐험 미션 5개**를 만들고, **방문 인증에 성공해야만 도장을 주는** 모바일 웹 프로토타입

**🔗 Live Demo:** https://jungang-market-ai-explorer.netlify.app/

| 조건 선택 | 미션 5개 생성 | 인증 실패 | 도장 획득 |
|:---:|:---:|:---:|:---:|
| <img src="regional-idea/docs/01-question.png" width="160"> | <img src="regional-idea/docs/02-missions.png" width="160"> | <img src="regional-idea/docs/03-fail.png" width="160"> | <img src="regional-idea/docs/04-success.png" width="160"> |

- 방문객이 입구 근처만 보고 떠나는 문제 → 조건별 탐험 미션으로 시장 안쪽까지 걷게 만들기
- 사진·QR 업로드 또는 GPS(시장 반경 700m) 확인이 있어야만 도장 지급, 5개 모으면 완주
- 외부 라이브러리 없는 HTML 파일 하나로 구현, ChatGPT·Claude를 개발 도구로 활용

👉 [기획 배경, 핵심 로직, 트러블슈팅 보기](regional-idea/README.md)

## 저장소 구조

```
daejeon-nonsan-aisw-contest/
├── README.md               # 대회 개요 (이 문서)
├── character-branding/     # AI 캐릭터·브랜딩 — 마스코트 「첫차」
│   ├── README.md
│   └── mascot-cheotcha.png
├── ai-song/                # AI 활용 노래·음원 — 「대전 중앙시장 다 있슈~」
│   ├── README.md
│   └── daejeon-jungang-market-song.mp3
└── regional-idea/          # 지역 활성화 아이디어 — 중앙시장 AI 탐험대
    ├── README.md
    ├── index.html
    ├── PROMPT.md
    └── docs/               # 스크린샷, 단계별 사용 프롬프트
```
