---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-TBA: Liquidity Locks"
author: ""
pub_date: "Tue, 20 Oct 2026 15:32:33 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-21
sources:
  - "https://ethereum-magicians.org/t/erc-tba-liquidity-locks/30028"
---
# ERC-TBA: Liquidity Locks

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-tba-liquidity-locks/30028)  |  Tue, 20 Oct 2026 15:32:33 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 유동성 잠금 방식의 표준화를 위한 ERC-TBA 초안으로, 풀 유동성 잠금 계약의 인터페이스를 정의하여 보안 및 상호운용성을 개선하려는 제안입니다.

**리서치 앵글:** DEX 경쟁구도 및 기관 DeFi 도입에 있어 유동성 잠금의 표준화는 보안과 신뢰도를 높여 중요한 영향을 미칠 수 있습니다.

## 원문 미리보기
<p>“The liquidity is locked” is every launch’s safety story, and no two lockers say it the same way, so scanners and launchpads keep allowlists of lockers they have integrated. This draft is one interface for any contract that locks pool liquidity (v2 pool tokens, v3 and v4 positions): which pool, how much, until when, for whom, who collects the locked position’s fees, with events, and per pool <code>lockedLiquidity</code> (permanent, timed, earliest unlock) at a cost that does not grow with the number of locks. Release is only at or after <code>unlockAt</code>, only to the beneficiary, and ne