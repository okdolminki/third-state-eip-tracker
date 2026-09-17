---
date: 2026-09-17
roadmap_ids: [PL-2]
source: GITHUB
update_type: PROGRESS
importance: MEDIUM
link: "https://github.com/Uniswap/universal-router/commit/aebfa391d3e3466fb083f5c03aad53ff7d76361c"
note_type: unification_update
auto_generated: true
---

# [Uniswap/universal-router] revert: undo #491 and #497 input-bounding and nested-unlock changes (#514)

> 출처: GITHUB | 2026-09-17 | 관련 항목: [[PL-2]]

## 요약
메인넷에 배포되었던 유니버설 라우터의 입력 제한 및 중첩 언락(nested-unlock) 변경 사항을 롤백함.
UNWRAP_WETH_EXACT 명령 및 calldata 입력 길이 검증 로직 등이 제거되어 이전 안정 상태로 복구됨.

## 시그널
유니버설 라우터에서 Uniswap v4 관련 핵심 기능(중첩 언락 등)의 미승인 배포본을 롤백하여 메인넷 라우터의 동작 안정성과 보안을 확보합니다.

---
[원문 보기](https://github.com/Uniswap/universal-router/commit/aebfa391d3e3466fb083f5c03aad53ff7d76361c)
