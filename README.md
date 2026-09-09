# 바이브 코딩 제작 가이드

지구과학 교사를 위한 바이브 코딩(Vibe Coding) 단계별 안내 웹앱입니다.
AI와 대화하며 교육용 웹앱을 만들고 학생과 공유하는 두 가지 방법을 소개합니다.

- **방법 1 · 채팅으로 바로 만들기** — Gemini Canvas, ChatGPT Canvas, Claude Artifacts에서 만들고 링크로 공유
- **방법 2 · 코드를 만들어 배포하기** — AI가 만든 코드를 GitHub에 저장하고 Vercel로 배포
- **핵심 원칙** — "바로 코드를 짜지 말고, 먼저 나와 충분히 대화한 다음에 코드를 짜줘"

## 구성

```
index.html   # 웹앱 전체 (HTML + CSS + JS, 빌드 도구 없음)
README.md
```

의존성이나 빌드 과정이 없는 정적 페이지입니다. `index.html`을 더블클릭하면 바로 열립니다.

## 배포

이 저장소를 Vercel에 Import 하면 설정 변경 없이 그대로 배포됩니다. (Framework Preset: Other)
GitHub Pages로도 배포할 수 있습니다. (Settings → Pages → Branch: `main`, folder: `/`)

## 수정

`index.html` 한 파일만 수정하면 됩니다. 각 섹션은 `id`로 구분되어 있습니다.

| id | 내용 |
|----|------|
| `#intro` | 바이브 코딩 소개, 두 방법 비교표 |
| `#principle` | 핵심 원칙(대화 먼저), 예시 대화(암석의 분류), 체크리스트 |
| `#method1` | 방법 1 단계 (5단계) |
| `#method2` | 방법 2 단계 (6단계, 예시: 판의 경계 시뮬레이션), 자주 겪는 문제 |
| `#prompts` | 복사해서 쓰는 프롬프트 모음 |
| `#faq` | 자주 묻는 질문 |

단계 체크박스 진행 상황은 브라우저 `localStorage`에만 저장됩니다.
