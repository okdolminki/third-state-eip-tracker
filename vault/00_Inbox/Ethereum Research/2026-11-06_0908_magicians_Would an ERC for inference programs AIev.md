---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Would an ERC for inference programs (AI-evaluated contracts) be feasible on Ethereum?"
author: ""
pub_date: "Thu, 05 Nov 2026 16:50:00 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-06
sources:
  - "https://ethereum-magicians.org/t/would-an-erc-for-inference-programs-ai-evaluated-contracts-be-feasible-on-ethereum/30291"
---
# Would an ERC for inference programs (AI-evaluated contracts) be feasible on Ethereum?

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/would-an-erc-for-inference-programs-ai-evaluated-contracts-be-feasible-on-ethereum/30291)  |  Thu, 05 Nov 2026 16:50:00 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 솔라나에서 논의 중인 '추론 프로그램' 또는 '실제 스마트 계약'이라는 AI 기반 계약 모델의 이더리움 ERC 도입 가능성을 타진하며, 오프체인 AI 모델이 계약 로직을 평가하는 방식을 제안한다.

**리서치 앵글:** AI 기반 스마트 계약은 L2 확장성을 통해 더 복잡한 온체인 로직 구현을 가능하게 하고, 기관 DeFi 도입을 위한 정교한 정책 집행 메커니즘을 제공할 수 있다.

## 원문 미리보기
<p>Hi all. We recently opened a discussion in the Solana SIMD repository about a new class of smart contracts we’re loosely calling “inference programs,” or “Actually Smart Contracts.” We’d value technical input from this community on whether a similar proposal could be feasible on Ethereum, before we write anything for it.</p>
<p>The idea, briefly: a contract stores a prompt and the rules that shape it (a DAO constitution, a policy, a standard). Another contract asks it a question with evidence. AI models from different operators answer off chain, each signs a vote, and the caller checks the 