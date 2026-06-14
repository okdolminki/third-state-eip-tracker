---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Draft ERC: AI Agent Execution"
author: ""
pub_date: "Sat, 13 Jun 2026 19:34:33 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-14
sources:
  - "https://ethereum-magicians.org/t/draft-erc-ai-agent-execution/28785"
---
# Draft ERC: AI Agent Execution

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/draft-erc-ai-agent-execution/28785)  |  Sat, 13 Jun 2026 19:34:33 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 온체인 AI 에이전트 생태계의 여러 ERC 개발에도 불구하고 AI 에이전트 실행에 있어 발견된 격차를 논의하는 초기 ERC 초안입니다.

**리서치 앵글:** AI 에이전트의 온체인 실행 및 신원 관리는 계정 추상화(EIP-7702)와 기관 DeFi 도입에 잠재적 영향을 미칠 수 있습니다.

## 원문 미리보기
<p>Hi everyone <img src="https://ethereum-magicians.org/images/emoji/twitter/waving_hand.png?v=15" title=":waving_hand:" class="emoji" alt=":waving_hand:" loading="lazy" width="20" height="20">,</p>
<p>Wanted to share a gap that has come up repeatedly while working across ERC-8274, ERC-8183, and ERC-8004 — and see if others have run into the same friction.</p>
<p>The on-chain AI agent ecosystem has made real progress across several layers: agent identity (ERC-8004), inference proof verification (ERC-8274), proof anchoring (ERC-8263), agentic commerce (ERC-8183). But there is one foundational p