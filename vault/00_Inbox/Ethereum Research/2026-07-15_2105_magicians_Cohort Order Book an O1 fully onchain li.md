---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Cohort Order Book: an O(1) fully on-chain limit order book via generational fungible liquidity"
author: ""
pub_date: "Wed, 15 Jul 2026 08:01:07 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-15
sources:
  - "https://ethereum-magicians.org/t/cohort-order-book-an-o-1-fully-on-chain-limit-order-book-via-generational-fungible-liquidity/29018"
---
# Cohort Order Book: an O(1) fully on-chain limit order book via generational fungible liquidity

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/cohort-order-book-an-o-1-fully-on-chain-limit-order-book-via-generational-fungible-liquidity/29018)  |  Wed, 15 Jul 2026 08:01:07 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 세대별 대체 가능한 유동성을 활용하여 O(1) 복잡도로 완전 온체인 리밋 오더북을 구현하는 방안을 제안하는 이더리움 매지션스 토론 초안.

**리서치 앵글:** 새로운 온체인 오더북 설계는 DEX 경쟁구도 및 MEV에 중장기적 영향을 미칠 수 있음.

## 원문 미리보기
<h1><a name="p-71871-cohort-order-book-an-o1-fully-on-chain-limit-order-book-via-generational-fungible-liquidity-1" class="anchor" href="https://ethereum-magicians.org#p-71871-cohort-order-book-an-o1-fully-on-chain-limit-order-book-via-generational-fungible-liquidity-1" aria-label="Heading link"></a>Cohort Order Book: an O(1) fully on-chain limit order book via generational fungible liquidity</h1>
<p><em>Draft for Ethereum Magicians. Looking for critique, especially on the one-sided-add justification in §4 and the FIFO concerns in §6.</em></p>
<h2><a name="p-71871-tldr-2" class="anchor" href="