---
date: 2026-08-04
roadmap_ids: [PL-2]
source: GITHUB
update_type: PROGRESS
importance: MEDIUM
link: "https://github.com/Uniswap/universal-router/commit/d203e7f5525aeae385800f9490b93886711701df"
note_type: unification_update
auto_generated: true
---

# [Uniswap/universal-router] fix: bound router command input decoding (#497)

> 출처: GITHUB | 2026-08-04 | 관련 항목: [[PL-2]]

## 요약
Universal Router의 명령 입력 디코딩 범위를 제한하고 가스 소모를 최적화함.
UNWRAP_WETH_AMOUNT를 UNWRAP_WETH_EXACT로 대체해 중복 로직을 제거함.

## 시그널
유니버설 라우터의 트랜잭션 디코딩 및 디스패처 명령을 최적화하여 향후 v4 메인넷 라우팅의 보안과 가스 효율성을 높입니다.

---
[원문 보기](https://github.com/Uniswap/universal-router/commit/d203e7f5525aeae385800f9490b93886711701df)
