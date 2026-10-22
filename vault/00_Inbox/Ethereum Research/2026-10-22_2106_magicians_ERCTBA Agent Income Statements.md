---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-TBA: Agent Income Statements"
author: ""
pub_date: "Thu, 22 Oct 2026 09:22:17 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-22
sources:
  - "https://ethereum-magicians.org/t/erc-tba-agent-income-statements/30047"
---
# ERC-TBA: Agent Income Statements

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-tba-agent-income-statements/30047)  |  Thu, 22 Oct 2026 09:22:17 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 이더리움 매지션스에서 ERC-TBA: Agent Income Statements 초안이 논의 중이며, 이는 에이전트의 수입을 ERC-8004 `agentWallet`에 기록하여 투명한 재무 상태를 제공하는 표준을 제안합니다.

**리서치 앵글:** 에이전트의 수입 명세서 표준화는 기관 DeFi 도입을 위한 투명성 및 신뢰도 확보에 기여하며, RWA 관련 대출 프로토콜에도 활용될 수 있습니다.

## 원문 미리보기
<p>An agent that sells over x402 is paid to its ERC-8004 <code>agentWallet</code>, and a lender or a buyer wants to know what it earns. This draft is a profile of the ERC-8004 Reputation Registry: a writer posts chained statements of what an agent’s <code>agentWallet</code> received in one asset, each incoming transfer a leaf of a Merkle root, under ERC-8004’s <code>revenues</code> tag (<code>tag2</code> <code>x402.statement</code>; x402 payments are the motivating case, but the totals are gross receipts). Windows are cut at the logs of an owner or wallet change (the ERC-721 <code>Transfer</co