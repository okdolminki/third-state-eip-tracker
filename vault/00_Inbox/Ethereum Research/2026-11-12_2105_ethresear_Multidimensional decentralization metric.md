---
source: "Ethereum Research"
source_type: research
title: "Multi-dimensional decentralization metrics, and an open question on first-broadcast double-spend rules"
author: ""
pub_date: "Thu, 12 Nov 2026 08:16:17 +0000"

importance: medium
action: weekly_review
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-11-12
sources:
  - "https://ethresear.ch/t/multi-dimensional-decentralization-metrics-and-an-open-question-on-first-broadcast-double-spend-rules/26242"
---
# Multi-dimensional decentralization metrics, and an open question on first-broadcast double-spend rules

> 출처: [Ethereum Research](https://ethresear.ch/t/multi-dimensional-decentralization-metrics-and-an-open-question-on-first-broadcast-double-spend-rules/26242)  |  Thu, 12 Nov 2026 08:16:17 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review

**요약:** 이더리움 리서치 포스트는 블록체인 아키텍처의 탈중앙화 수준을 다차원적으로 분석하는 새로운 측정 지표와 도구를 제안하며, 기존 나카모토 계수의 한계를 지적합니다.

**리서치 앵글:** 블록체인 탈중앙화 측정 지표는 LST/LRT 구조의 안정성과 L2 확장성의 핵심 요소인 노드/검증자 집중도 분석에 직접적으로 연관됩니다.

## 원문 미리보기
<p>Disclosure: I am the creator of Atomic Ownership Blockchains (AOB), which this repo covers in more detail than the other designs.</p>
<p>What this is</p>
<p>An open-source skill (SKILL.md format, Apache-2.0) that lets LLM agents analyze blockchain architectures on several independent dimensions instead of one number. The Nakamoto coefficient is a single-subsystem snapshot, goes stale, and is not comparable across consensus mechanisms, so the skill treats it as one input per subsystem, not a ranking.</p>
<p>Dimensions currently covered:</p>
<pre><code>Node/validator concentration (NC per sub