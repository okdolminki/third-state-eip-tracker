---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Draft ERC: Agent Information Flow Paradigm (AIFP) - versioned, composable rules for how agents provide, observe and redistribute information"
author: ""
pub_date: "Sun, 08 Nov 2026 11:26:13 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-08
sources:
  - "https://ethereum-magicians.org/t/draft-erc-agent-information-flow-paradigm-aifp-versioned-composable-rules-for-how-agents-provide-observe-and-redistribute-information/30300"
---
# Draft ERC: Agent Information Flow Paradigm (AIFP) - versioned, composable rules for how agents provide, observe and redistribute information

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/draft-erc-agent-information-flow-paradigm-aifp-versioned-composable-rules-for-how-agents-provide-observe-and-redistribute-information/30300)  |  Sun, 08 Nov 2026 11:26:13 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** AIFP는 에이전트 간 정보 계층을 위한 프레임워크 ERC로, 에이전트가 정보를 제공, 관찰, 재분배하는 방식에 대한 버전 관리되고 구성 가능한 규칙을 정의합니다.

**리서치 앵글:** 에이전트 간 정보 흐름 표준화는 기관 DeFi 도입 및 L2 확장성 개선에 기여할 수 있습니다.

## 원문 미리보기
<p><strong>Summary.</strong> AIFP is a framework ERC for the information layer between agents. It defines a flow paradigm<br>
as a content-addressed, versioned description of an interaction context - which carriers (addressed<br>
delivery, shared object) and structural operators (fan-out, fan-in, feedback, n-party, select, forward,<br>
derive, merge) it uses, and how thirteen separately declared rule dimensions are set (discovery,<br>
observation, contribution, management, redistribution, history, time, disclosure timing, contributor<br>
visibility, admission basis, representation, object rela