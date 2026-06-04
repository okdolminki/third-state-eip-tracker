---
date: 2026-06-04
roadmap_ids: [LG-8]
source: GITHUB
update_type: PROGRESS
importance: MEDIUM
link: "https://github.com/Uniswap/permit2/commit/2141eef4c8b1ceb352fc48de441d7ea50fa2b967"
note_type: unification_update
auto_generated: true
---

# [Uniswap/permit2] fix(Permit2Lib): add gas cap to DOMAIN_SEPERATOR staticcall  (#166)

> 출처: GITHUB | 2026-06-04 | 관련 항목: [[LG-8]]

## 요약
Permit2Lib의 DOMAIN_SEPARATOR 호출에 가스 한도를 추가해 가스 과다 소모를 방지함.
WETH 토큰일 경우 도메인 구분자 검사를 건너뛰도록 성능을 최적화함.

## 시그널
Permit2를 통한 토큰 승인 시 비정상적인 가스 소모를 방지하고 트랜잭션 처리 효율을 개선합니다.

---
[원문 보기](https://github.com/Uniswap/permit2/commit/2141eef4c8b1ceb352fc48de441d7ea50fa2b967)
