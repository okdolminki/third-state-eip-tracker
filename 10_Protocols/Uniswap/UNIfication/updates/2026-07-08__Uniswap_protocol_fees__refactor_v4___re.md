---
date: 2026-07-08
roadmap_ids: [FM-6]
source: GITHUB
update_type: PROGRESS
importance: MEDIUM
link: "https://github.com/Uniswap/protocol-fees/commit/ae55fd9e71f73d4b78e1f2e8a2c65326f86f935d"
note_type: unification_update
auto_generated: true
---

# [Uniswap/protocol-fees] refactor(v4): remove HookFeeFlags library in favor of documented conventions

> 출처: GITHUB | 2026-07-08 | 관련 항목: [[FM-6]]

## 요약
Uniswap v4 프로토콜 수수료 시스템에서 불필요한 HookFeeFlags 라이브러리를 제거하고
온체인 비트 검증 대신 문서화된 약속을 준수하는 방식으로 리팩토링을 진행했습니다.

## 시그널
v4 프로토콜 수수료 계약의 불필요한 복잡성을 줄이고 수수료 연동 훅(Hook) 설계의 유연성을 높여 v4 수수료 어댑터 구현을 최적화합니다.

---
[원문 보기](https://github.com/Uniswap/protocol-fees/commit/ae55fd9e71f73d4b78e1f2e8a2c65326f86f935d)
