---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Draft ERC: Agent Identity (AID) — address-anchored identity for live agents, over ERC-8004 + assertion registries"
author: ""
pub_date: "Wed, 30 Sep 2026 03:43:47 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-09-30
sources:
  - "https://ethereum-magicians.org/t/draft-erc-agent-identity-aid-address-anchored-identity-for-live-agents-over-erc-8004-assertion-registries/29805"
---
# Draft ERC: Agent Identity (AID) — address-anchored identity for live agents, over ERC-8004 + assertion registries

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/draft-erc-agent-identity-aid-address-anchored-identity-for-live-agents-over-erc-8004-assertion-registries/29805)  |  Wed, 30 Sep 2026 03:43:47 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 이더리움 주소 기반의 에이전트 신원(AID) 표준 초안으로, ERC-8004와 어설션 레지스트리를 활용하여 라이브 에이전트의 신원을 정의합니다.

**리서치 앵글:** 이 제안은 계정 추상화(EIP-7702) 테마와 직접적으로 연관되며, 온체인 에이전트 신원 표준화를 통해 기관 DeFi 도입 및 L2 확장성에 기여할 수 있습니다.

## 원문 미리보기
<p><strong>Draft:</strong> <a href="https://github.com/garyyang-finchip/aid-standard/blob/main/ERCS/erc-aid.md" class="inline-onebox" rel="noopener nofollow ugc">aid-standard/ERCS/erc-aid.md at main · garyyang-finchip/aid-standard · GitHub</a> <strong>Filing variant (what goes to ethereum/ERCs):</strong> <a href="https://github.com/garyyang-finchip/aid-standard/blob/main/ercs-pr-package/ERCS/erc-9999.md" class="inline-onebox" rel="noopener nofollow ugc">aid-standard/ercs-pr-package/ERCS/erc-9999.md at main · garyyang-finchip/aid-standard · GitHub</a> <strong>Reference implementation, schemas, 