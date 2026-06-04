---
date: 2026-06-04
roadmap_ids: [LG-8]
source: GITHUB
update_type: PROGRESS
importance: MEDIUM
link: "https://github.com/Uniswap/universal-router/commit/999d561c3ad58fb5cab91b602911f3c75591a9c7"
note_type: unification_update
auto_generated: true
---

# [Uniswap/universal-router] feat: add SwapProxy contract for permit2-less swap flow (#469)

> 출처: GITHUB | 2026-06-04 | 관련 항목: [[LG-8]]

## 요약
Permit2 서명 없이 '승인+스왑'의 2단계 흐름을 지원하는 SwapProxy 컨트랙트 추가
첫 거래 시 3번의 트랜잭션이 요구되던 통합사들의 피드백을 반영하여 사용자 경험 개선

## 시그널
Permit2 서명이 불필요한 대체 경로를 제공하여 통합사들의 연동 허들을 낮추고, API 기반 최초 사용자 온보딩 경험을 개선합니다.

---
[원문 보기](https://github.com/Uniswap/universal-router/commit/999d561c3ad58fb5cab91b602911f3c75591a9c7)
