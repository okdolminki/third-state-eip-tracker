---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Inheritable Agent Mandates — a non-strippable, inherited leash for on-chain agents"
author: ""
pub_date: "Tue, 04 Aug 2026 21:39:04 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-05
sources:
  - "https://ethereum-magicians.org/t/inheritable-agent-mandates-a-non-strippable-inherited-leash-for-on-chain-agents/29275"
---
# Inheritable Agent Mandates — a non-strippable, inherited leash for on-chain agents

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/inheritable-agent-mandates-a-non-strippable-inherited-leash-for-on-chain-agents/29275)  |  Tue, 04 Aug 2026 21:39:04 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 온체인 AI 에이전트가 부모 계정의 통제권을 상속받아 탈출하지 못하도록 하는 새로운 ERC 아이디어를 제안합니다.

**리서치 앵글:** AI 에이전트의 온체인 활동 및 통제 메커니즘에 대한 논의로, 계정 추상화(EIP-7702) 및 기관 DeFi 도입과 밀접하게 연관됩니다.

## 원문 미리보기
<p>Hi all — I’d like to put an idea in front of this group before I open a PR for it, as the process asks. Draft ERC and reference material are linked at the bottom; this post is the short version and the invitation to tear into it.</p>
<p><strong>The gap.</strong> AI agents are starting to hold money on-chain and to spawn copies of themselves to work in parallel. Almost every guardrail we have — signing-time policy engines, session keys, per-wallet caps, ERC-8226-style mandates — is attached to a <em>single</em> account and doesn’t follow that account’s children. So an agent can escape its ow