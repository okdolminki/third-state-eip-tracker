---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8478: x402 Payee Verification for ERC-8004 Agents"
author: ""
pub_date: "Fri, 30 Oct 2026 18:03:57 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-31
sources:
  - "https://ethereum-magicians.org/t/erc-8478-x402-payee-verification-for-erc-8004-agents/30137"
---
# ERC-8478: x402 Payee Verification for ERC-8004 Agents

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8478-x402-payee-verification-for-erc-8004-agents/30137)  |  Fri, 30 Oct 2026 18:03:57 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** ERC-8004 에이전트 간 x402 결제 시 수신자의 신원(agentWallet) 검증이 부족하여 자금 탈취 위험이 있으며, ERC-8478은 이를 해결하기 위한 방안을 제시한다.

**리서치 앵글:** 기관 DeFi 도입 시 필요한 에이전트 신원 및 결제 보안 강화와 계정 추상화(EIP-7702) 관련 에이전트 모델의 안전한 상호작용에 대한 연구.

## 원문 미리보기
<p>when an agent pays another agent over x402, the payTo comes from the 402 answer, and nothing ties it to the paid agent’s ERC-8004 identity. whoever controls that HTTP answer (a hijacked domain, a proxy in the path, an instruction injected into a tool result) chooses where the money goes. the payment still settles, the resource may even be delivered, and the funds are gone.</p>
<p>ERC-8004 already has the right anchor: agentWallet, which can only be set with a signature of that wallet, so it is the one address proven to be under the agent’s control. today no rule says a payer should compare 