---
date: 2026-08-10
roadmap_ids: [PL-2, PL-3]
source: GITHUB
update_type: PROGRESS
importance: MEDIUM
link: "https://github.com/Uniswap/v4-periphery/commit/bbd43468f07a7e0cbf43bb17eda2e5442fc4549c"
note_type: unification_update
auto_generated: true
---

# [Uniswap/v4-periphery] fix: tolerate hook-funded input on exact-output swaps (#584)

> 출처: GITHUB | 2026-08-10 | 관련 항목: [[PL-2]], [[PL-3]]

## 요약
Uniswap v4-periphery에서 exact-output 스왑 시 훅이 입력 자금을 대신 지불하는 상황을 허용함.
훅이 비용을 전액 충당하여 입력 델타가 0인 상태에서도 솔벤시를 유지하며 정상 작동하도록 수정함.

## 시그널
v4 periphery 라우터가 훅 자금 지원 방식의 스왑을 정상적으로 허용하도록 수정하여, v4 메인넷 출시를 위한 훅 네이티브 인프라의 완성도를 높였습니다.

---
[원문 보기](https://github.com/Uniswap/v4-periphery/commit/bbd43468f07a7e0cbf43bb17eda2e5442fc4549c)
