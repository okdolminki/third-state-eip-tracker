---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-TBA: Agent Repay-First Payees"
author: ""
pub_date: "Tue, 20 Oct 2026 15:24:23 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-21
sources:
  - "https://ethereum-magicians.org/t/erc-tba-agent-repay-first-payees/30025"
---
# ERC-TBA: Agent Repay-First Payees

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-tba-agent-repay-first-payees/30025)  |  Tue, 20 Oct 2026 15:24:23 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 에이전트의 수입이 발생하면 등록된 채권자에게 자동으로 우선 상환하는 온체인 메커니즘(수익 주소)에 대한 EIP 논의.

**리서치 앵글:** RWA 및 기관 DeFi 도입을 위한 신뢰성 높은 온체인 대출 상환 메커니즘으로, 계정 추상화와 연계될 수 있음.

## 원문 미리보기
<p>Credit that grows with an agent’s income has to be repaid from that income before it is spent. This draft is a revenue address for an agent identity (an x402 <code>payTo</code>, an ERC-8183 provider, an ERC-8004 payment wallet) that pays the agent’s registered creditors before its owner: whenever anyone sweeps it, each creditor is paid what it is owed, most senior first and up to its agreed share of the sweep, and the rest goes to the owner’s beneficiary. The owner cannot drop a creditor that is still owed, which is what makes the revenue worth lending against. A beneficiary holds only whil