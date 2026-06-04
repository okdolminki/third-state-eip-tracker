---
date: 2026-06-04
roadmap_ids: [LG-8]
source: GITHUB
update_type: PROGRESS
importance: MEDIUM
link: "https://github.com/Uniswap/permit2/commit/2fa27a37d23ac97a5e4402810fcd61cc5c178250"
note_type: unification_update
auto_generated: true
---

# [Uniswap/permit2] feat: update permit2lib address (#151)

> 출처: GITHUB | 2026-06-04 | 관련 항목: [[LG-8]]

## 요약
여러 체인에 동일한 고정 주소로 배포된 Permit2의 올바른 주소를 참조하도록 permit2lib 포인터를 업데이트함.
이를 통해 다양한 네트워크 환경에서 스마트 컨트랙트가 올바른 Permit2 주소를 가리키도록 보장함.

## 시그널
다중 체인 환경에서 Permit2 인프라가 올바른 배포 주소를 참조하도록 보장함으로써, API zero-margin(LG-8) 구현을 위한 멀티체인 토큰 승인 레이어의 안정성을 강화합니다.

---
[원문 보기](https://github.com/Uniswap/permit2/commit/2fa27a37d23ac97a5e4402810fcd61cc5c178250)
