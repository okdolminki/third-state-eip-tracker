---
date: 2026-07-14
roadmap_ids: [PL-2, PL-3]
source: GITHUB
update_type: PROGRESS
importance: MEDIUM
link: "https://github.com/Uniswap/v4-periphery/commit/3245c3cb99c48fa1dc2459c3b60abc37d4294aba"
note_type: unification_update
auto_generated: true
---

# [Uniswap/v4-periphery] fix(lens): ReservesLens follow-ups — graceful gas degradation, cursor hardening, default-parameter overloads (#577)

> 출처: GITHUB | 2026-07-14 | 관련 항목: [[PL-2]], [[PL-3]]

## 요약
v4-periphery의 ReservesLens 내 가스 고갈 처리 및 체인별 커서 고정 개선
훅 통계 탐색 중 가스 부족 시 Revert 대신 전용 상태를 반환하도록 예외 처리 강화

## 시그널
Uniswap v4 출시를 앞두고 주변부(Periphery) 조회 계약의 가스 예외 처리를 최적화하여 훅 기반 유동성 인프라의 안정성을 극대화하는 단계입니다.

---
[원문 보기](https://github.com/Uniswap/v4-periphery/commit/3245c3cb99c48fa1dc2459c3b60abc37d4294aba)
