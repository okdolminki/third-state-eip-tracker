---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Pre-ERC: Agent Linkability Report"
author: ""
pub_date: "Sat, 21 Nov 2026 08:03:56 +0000"

importance: medium
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-21
sources:
  - "https://ethereum-magicians.org/t/pre-erc-agent-linkability-report/30462"
---
# Pre-ERC: Agent Linkability Report

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/pre-erc-agent-linkability-report/30462)  |  Sat, 21 Nov 2026 08:03:56 +0000

## AI 분석
**중요도:** medium | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** ERC-8004 에이전트의 소유자, 지갑, 결제 주소가 공개 체인 데이터를 통해 연결될 수 있어 프라이버시 문제가 발생할 수 있다는 보고서 초안입니다.

**리서치 앵글:** 계정 추상화(EIP-7702)와 관련된 에이전트의 온체인 프라이버시 및 연결성 문제 분석.

## 원문 미리보기
<p>hi all. this is a draft for a small report format: what anyone can link about an ERC-8004 agent from public chain data.</p>
<p><strong>problem</strong></p>
<p>an 8004 agent publishes its owner, its <code>agentWallet</code> and (via its registration file) the x402 <code>payTo</code> it gets paid on. all of these are public addresses with public histories, so a payer or anyone watching the chain can often tie the payment address to the owner, the owner to its other agents, and every payer to the agent.</p>
<p>on Robinhood Chain (<code>chainId</code> <code>4663</code>) we read the identity reg