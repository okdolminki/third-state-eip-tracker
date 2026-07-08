---
date: 2026-07-08
roadmap_ids: [FM-6]
source: GITHUB
update_type: PROGRESS
importance: MEDIUM
link: "https://github.com/Uniswap/protocol-fees/commit/b3496fef03bb9d149325e6de803d7e29c61e88bb"
note_type: unification_update
auto_generated: true
---

# [Uniswap/protocol-fees] fix(v4): disambiguate zero fee events

> 출처: GITHUB | 2026-07-08 | 관련 항목: [[FM-6]]

## 요약
Uniswap v4 프로토콜 수수료 컨트랙트에서 명시적 0% 수수료와 설정 초기화를 구분하는 이벤트를 수정함.
인코딩된 수수료 값을 방출하여 인덱서가 수수료 데이터를 명확히 식별할 수 있도록 개선함.

## 시그널
Uniswap v4 프로토콜 수수료 데이터의 모호성을 제거하고 오프체인 인덱서의 파싱 정확도를 높여 수수료 어댑터 인프라의 안정성을 강화했습니다.

---
[원문 보기](https://github.com/Uniswap/protocol-fees/commit/b3496fef03bb9d149325e6de803d7e29c61e88bb)
