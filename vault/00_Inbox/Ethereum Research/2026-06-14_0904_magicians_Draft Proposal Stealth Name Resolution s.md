---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Draft Proposal: Stealth Name Resolution (stealth meta-address names across asynchronous chains)"
author: ""
pub_date: "Sat, 13 Jun 2026 20:54:11 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-14
sources:
  - "https://ethereum-magicians.org/t/draft-proposal-stealth-name-resolution-stealth-meta-address-names-across-asynchronous-chains/28787"
---
# Draft Proposal: Stealth Name Resolution (stealth meta-address names across asynchronous chains)

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/draft-proposal-stealth-name-resolution-stealth-meta-address-names-across-asynchronous-chains/28787)  |  Sat, 13 Jun 2026 20:54:11 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 스텔스 메타 주소의 이름 해결 레이어를 정의하고, 이더리움 레지스트리와 ENS를 활용하며, 비동기 체인 간 미러링을 지원하는 초안 제안.

**리서치 앵글:** 스텔스 주소 및 이름 해결은 계정 추상화(EIP-7702)와 연관되어 사용자 경험 및 프라이버시 개선에 기여할 수 있음.

## 원문 미리보기
<h2><a name="p-70980-summary-1" class="anchor" href="https://ethereum-magicians.org#p-70980-summary-1" aria-label="Heading link"></a>Summary</h2>
<p>I am sharing a draft proposal for discussion. It defines a name-resolution layer for stealth meta-addresses. A canonical Ethereum registry acts as both registrar and ENSIP-10 wildcard resolver for a parent ENS name, serving a <code>com.opaque.meta</code> text record. The registry can store explicit keys or source them live from the ERC-6538 registry. The proposal also defines a transport-agnostic mirror payload so a second chain can maintain read-