---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8320: Regulated Asset Claim"
author: ""
pub_date: "Fri, 03 Jul 2026 10:19:58 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-03
sources:
  - "https://ethereum-magicians.org/t/erc-8320-regulated-asset-claim/28919"
---
# ERC-8320: Regulated Asset Claim

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8320-regulated-asset-claim/28919)  |  Fri, 03 Jul 2026 10:19:58 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 온체인 자산의 가치와 근거를 기계가 검증할 수 있도록 규제 자산 클레임에 대한 표준 레지스트리를 제안합니다.

**리서치 앵글:** RWA 및 기관 DeFi 도입을 위한 온체인 자산의 가치 및 근거를 기계적으로 검증하는 표준으로, 핵심 리서치 테마와 직결됩니다.

## 원문 미리보기
<p>We propose a registry standard for verifiable claims about on-chain assets.</p>
<p><strong>The gap:</strong><br>
Existing standards define how assets behave: ERC-4626/7540/7575 hold and settle value, ERC-3643/7943 enforce who may hold and transfer. None define what an asset is, what it is worth, or what backs it, in a form a machine can verify. That data lives in PDFs, so every integration is bespoke. Self-description doesn’t solve it: a self-reported NAV proves nothing about who stands behind it.</p>
<p><strong>The primitive:</strong><br>
A claim: a signed, versioned, hash-anchored stateme