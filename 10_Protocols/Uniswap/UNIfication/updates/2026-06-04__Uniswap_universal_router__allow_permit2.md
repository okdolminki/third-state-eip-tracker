---
date: 2026-06-04
roadmap_ids: [LG-8]
source: GITHUB
update_type: PROGRESS
importance: MEDIUM
link: "https://github.com/Uniswap/universal-router/commit/5aefc7e9654af12c78e551deca5854c9f6b1fb32"
note_type: unification_update
auto_generated: true
---

# [Uniswap/universal-router] allow permit2 to silently fail to avoid dos (#417)

> 출처: GITHUB | 2026-06-04 | 관련 항목: [[LG-8]]

## 요약
Universal Router에서 Permit2 호출 실패 시 전체 트랜잭션이 revert되는 대신 조용히 실패하도록 수정하여 DoS를 방지합니다.
라우팅 안정성 향상을 통해 트랜잭션 실패율을 낮추고 사용자 경험을 개선합니다.

## 시그널
Universal Router와 Permit2 연동 과정에서의 예외 처리를 개선하여 DoS 공격 벡터를 차단하고 라우팅의 안정성을 강화합니다.

---
[원문 보기](https://github.com/Uniswap/universal-router/commit/5aefc7e9654af12c78e551deca5854c9f6b1fb32)
