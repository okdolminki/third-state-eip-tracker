---
date: 2026-08-04
roadmap_ids: [PL-2]
source: GITHUB
update_type: PROGRESS
importance: MEDIUM
link: "https://github.com/Uniswap/v4-periphery/commit/545a5d2a87228167edde48f3b9eda122d1e3c4d6"
note_type: unification_update
auto_generated: true
---

# [Uniswap/v4-periphery] fix: revert on exact-output partial fills in V4Router (#564)

> 출처: GITHUB | 2026-08-04 | 관련 항목: [[PL-2]]

## 요약
Uniswap v4 라우터(V4Router)에서 exact-output 스왑 시 유동성 부족으로 일부만 체결되는 경우 거래를 revert하도록 수정했습니다.
출력 금액을 검증하지 않아 요청보다 적은 금액이 체결된 채 성공하던 문제를 해결했습니다.

## 시그널
Uniswap v4 라우터의 exact-output 거래 시 발생하던 불완전 체결 취약점을 수정하여 v4 메인넷 출시를 위한 거래 안정성을 보완했습니다.

---
[원문 보기](https://github.com/Uniswap/v4-periphery/commit/545a5d2a87228167edde48f3b9eda122d1e3c4d6)
