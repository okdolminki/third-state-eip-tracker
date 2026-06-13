---
source: "Ethereum Research"
source_type: research
title: "Three fixes, three new attacks: decaying vote weight in a weighted consensus"
author: ""
pub_date: "Fri, 12 Jun 2026 12:19:16 +0000"

importance: medium
action: weekly_review
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-06-13
sources:
  - "https://ethresear.ch/t/three-fixes-three-new-attacks-decaying-vote-weight-in-a-weighted-consensus/25164"
---
# Three fixes, three new attacks: decaying vote weight in a weighted consensus

> 출처: [Ethereum Research](https://ethresear.ch/t/three-fixes-three-new-attacks-decaying-vote-weight-in-a-weighted-consensus/25164)  |  Fri, 12 Jun 2026 12:19:16 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review

**요약:** 가중치 기반 합의 메커니즘에서 여러 자원을 혼합하여 검증인 가중치를 부여할 때 발생하는 취약점과 그 해결책이 새로운 공격을 유발하는 문제점을 다룬 연구.

**리서치 앵글:** 가중치 기반 합의 메커니즘의 취약점은 LST/LRT 구조의 근본적인 보안 및 안정성에 영향을 미칠 수 있음.

## 원문 미리보기
<p>Suppose a chain weights validators by more than one resource. Say a combined weight that mixes proof of work, staked capital, and an earned contribution score, finalizing a block when the supporting weight passes a two thirds supermajority. This is a reasonable design. It is also the start of a chain of failures where every fix you reach for opens the next hole. I built the reference model and tested each step, and I want to lay out the sequence, because the trap is general and not specific to any one weighting. Start with a real and sensible goal. You want voting weight to track live parti