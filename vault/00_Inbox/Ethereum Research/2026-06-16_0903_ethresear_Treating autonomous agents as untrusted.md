---
source: "Ethereum Research"
source_type: research
title: "Treating autonomous agents as untrusted participants: what the Claude Code harness suggests for on-chain mechanism design"
author: ""
pub_date: "Mon, 15 Jun 2026 20:02:59 +0000"

importance: medium
action: weekly_review
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-06-16
sources:
  - "https://ethresear.ch/t/treating-autonomous-agents-as-untrusted-participants-what-the-claude-code-harness-suggests-for-on-chain-mechanism-design/25202"
---
# Treating autonomous agents as untrusted participants: what the Claude Code harness suggests for on-chain mechanism design

> 출처: [Ethereum Research](https://ethresear.ch/t/treating-autonomous-agents-as-untrusted-participants-what-the-claude-code-harness-suggests-for-on-chain-mechanism-design/25202)  |  Mon, 15 Jun 2026 20:02:59 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review

**요약:** 온체인 메커니즘 설계에서 자율형 AI 에이전트를 신뢰할 수 없는 참여자로 전제하고, 오프라인 행동과의 격차를 줄이기 위해 부정직한 행동의 수익성을 낮추는 인센티브 구조 설계의 중요성을 강조합니다.

**리서치 앵글:** 자율형 AI 에이전트의 DeFi 프로토콜 참여가 본격화됨에 따라, 계정 추상화(EIP-7702) 및 MEV 관점에서 신뢰가 필요 없는 온체인 메커니즘을 설계하는 데 중요한 시사점을 제공합니다.

## 원문 미리보기
<p>This continues a line I have been posting here since early May about the gap between what a protocol can enforce on-chain and what actually happens off-chain, and how good mechanism design narrows that gap by making the dishonest action unprofitable rather than by trusting anyone to be honest. A recent event outside our usual subject matter gave me a clean, large external example of the same principle, and I think it is worth bringing back on topic because autonomous agents are about to become first-class participants in the systems we design here.</p>
<p>In late March an AI coding tool’s f