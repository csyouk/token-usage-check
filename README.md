# AI CLI 토큰 사용량 비교 프로젝트

동일한 프롬프트를 여러 AI CLI 도구에 입력했을 때의 토큰 사용량을 비교하는 프로젝트입니다.

## 목적

AI 코딩 어시스턴트 도구별로 동일한 작업에 대해 얼마나 많은 토큰을 소비하는지 측정하고 비교합니다.
이를 통해 비용 효율성과 응답 품질 간의 트레이드오프를 파악할 수 있습니다.

## 비교 대상 도구

| 도구 | 상태 |
|------|------|
| [Claude Code](https://claude.ai/code) | 측정 중 |
| [Codex CLI](https://github.com/openai/codex) | 예정 |
| [Gemini CLI](https://github.com/google-gemini/gemini-cli) | 예정 |
| [Cursor AI](https://www.cursor.com/) | 예정 |

## 측정 방법

- 각 도구에 동일한 프롬프트를 입력
- 작업 완료 후 토큰 사용량 기록
- 결과를 각 도구별 markdown 파일에 누적 기록

## 기록 파일

| 파일 | 설명 |
|------|------|
| `claude-token-usage.md` | Claude Code 토큰 사용량 기록 |

## 기록 형식

| 프롬프트 수행 시점 | 작업 시간 | 프롬프트 | 토큰 사용량 |
|----------------|---|---|---|
| YYYY-MM-DD hh:mm:ss | mm | 프롬프트 내용 | 사용량 |

## 디렉토리 구조

```
prompt-test/
├── README.md
├── CLAUDE.md                  # Claude Code 작업 규칙
├── claude-token-usage.md      # Claude Code 토큰 사용량 기록
└── voting-app-by-claude/      # Claude로 생성한 샘플 앱
```
