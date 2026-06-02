---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Gateway-to-gateway coordination for EIP-3668 / Proposing a mesh sync protocol"
author: ""
pub_date: "Tue, 02 Jun 2026 12:01:58 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-02
sources:
  - "https://ethereum-magicians.org/t/gateway-to-gateway-coordination-for-eip-3668-proposing-a-mesh-sync-protocol/28680"
---
# Gateway-to-gateway coordination for EIP-3668 / Proposing a mesh sync protocol

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/gateway-to-gateway-coordination-for-eip-3668-proposing-a-mesh-sync-protocol/28680)  |  Tue, 02 Jun 2026 12:01:58 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-3668(CCIP-Read) 게이트웨이 간의 효율적인 데이터 동기화 및 조정을 위한 메시 동기화 프로토콜 제안에 대한 논의.

**리서치 앵글:** RWA 및 기관 DeFi 도입에 필수적인 오프체인 데이터의 신뢰성과 확장성을 향상시키는 데 기여할 수 있음.

## 원문 미리보기
<p><strong>Category:</strong> EIPs / ERC Discussion<br>
<strong>Tags:</strong> eip-3668, ccip-read, gateways, attestation<br>
<strong>Co-authors:</strong> Tiago Merlini (<a class="mention" href="https://ethereum-magicians.org/u/tmerlini">@TMerlini</a>), Damon Zwicker (OCP), Vincent Wu (ERC-8263 / Composition Note), Jimmy Shi (ERC-8274)</p>
<hr>
<h2><a name="p-70526-the-gap-1" class="anchor" href="https://ethereum-magicians.org#p-70526-the-gap-1" aria-label="Heading link"></a>The gap</h2>
<p>EIP-3668 precisely specifies how a client talks to a CCIP-Read gateway: the request format, the response