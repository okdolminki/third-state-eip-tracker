---
date: 2026-07-24
roadmap_ids: [FM-4, FM-6]
source: GITHUB
update_type: PROGRESS
importance: HIGH
link: "https://github.com/Uniswap/protocol-fees/commit/17190e0bd2cf249f8575b8193949a979b457dfea"
note_type: unification_update
auto_generated: true
---

# [Uniswap/protocol-fees] fix(proposal-6): activate WorldChain & XLayer v4 fees via CrossChainAccount (XDM), not OptimismPortal2

> 출처: GITHUB | 2026-07-24 | 관련 항목: [[FM-4]], [[FM-6]]

## 요약
월드체인 및 엑스레이어(XLayer)의 v4 프로토콜 수수료 활성화를 위한 코드 수정
OptimismPortal2 대신 CrossChainAccount(XDM)를 통해 호출 경로 및 소유권 검증 해결

## 시그널
L2 체인(월드체인, XLayer)에서 Uniswap v4 수수료를 성공적으로 활성화하기 위해, 메인넷 거버넌스의 L2 제안 실행 경로 오류를 해결하고 수수료 수집 인프라를 확장합니다.

---
[원문 보기](https://github.com/Uniswap/protocol-fees/commit/17190e0bd2cf249f8575b8193949a979b457dfea)
