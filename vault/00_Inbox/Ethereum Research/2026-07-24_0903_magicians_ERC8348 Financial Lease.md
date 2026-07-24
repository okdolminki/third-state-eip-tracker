---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8348: Financial Lease"
author: ""
pub_date: "Thu, 23 Jul 2026 12:29:17 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-24
sources:
  - "https://ethereum-magicians.org/t/erc-8348-financial-lease/29076"
---
# ERC-8348: Financial Lease

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8348-financial-lease/29076)  |  Thu, 23 Jul 2026 12:29:17 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 온체인 토큰화된 금융 리스(할부 상환 및 구매 옵션 포함 신용 상품)를 표준화하여 맞춤형 통합 문제를 해결하기 위한 새로운 ERC 초안 논의.

**리서치 앵글:** RWA 및 기관 DeFi 도입을 위한 온체인 금융 리스 표준화의 잠재적 영향 분석.

## 원문 미리보기
<p>Hi all,</p>
<p>We’ve been building tokenized financial leases and kept running into the same problem: there’s no standard way to expose a lease contract on-chain, so every integration is a custom adapter. We drafted an ERC for it and want to sanity-check the design here before opening the PR to ethereum/ERCs.</p>
<p>Quick scope note: by “financial lease” we mean the credit instrument (lessor funds an asset, lessee pays installments, usually with a purchase option at the end) — not NFT rentals. ERC-4907 handles temporary usage rights well, but it has no notion of installments, arrears, purch