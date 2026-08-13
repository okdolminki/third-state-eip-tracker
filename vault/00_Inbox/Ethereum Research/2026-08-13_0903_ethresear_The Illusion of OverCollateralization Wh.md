---
source: "Ethereum Research"
source_type: research
title: "The Illusion of Over-Collateralization: Why Static C-Ratios Fail in T+0 Macro Panics (and a Proposed On-Chain Solution)"
author: ""
pub_date: "Wed, 12 Aug 2026 14:37:28 +0000"

importance: high
action: read_now
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-08-13
sources:
  - "https://ethresear.ch/t/the-illusion-of-over-collateralization-why-static-c-ratios-fail-in-t-0-macro-panics-and-a-proposed-on-chain-solution/25692"
---
# The Illusion of Over-Collateralization: Why Static C-Ratios Fail in T+0 Macro Panics (and a Proposed On-Chain Solution)

> 출처: [Ethereum Research](https://ethresear.ch/t/the-illusion-of-over-collateralization-why-static-c-ratios-fail-in-t-0-macro-panics-and-a-proposed-on-chain-solution/25692)  |  Wed, 12 Aug 2026 14:37:28 +0000

## AI 분석
**중요도:** high | **액션:** read_now

**요약:** 정적 담보비율은 T+0 거시적 패닉 상황에서 무한한 유동성 가정을 깨뜨리며 시스템적 실패를 막기에는 불충분하다는 점을 지적하고 온체인 해결책을 제안한다.

**리서치 앵글:** RWA 및 LST/LRT 구조의 핵심인 담보화 모델의 근본적인 취약점을 분석하고 개선 방안을 모색한다.

## 원문 미리보기
<p><strong>The Illusion of Over-Collateralization: Why Static C-Ratios Fail in T+0 Macro Panics (and a Proposed On-Chain Solution)</strong></p>
<p><strong>1. The False Assumption of Infinite T+0 Liquidity</strong></p>
<p>Current DeFi and RWA architectures (e.g., MakerDAO, Synthetix) rely heavily on a singular defense mechanism: the static over-collateralization ratio (C-Ratio). The prevailing logic assumes that a 150% or 200% C-Ratio guarantees systemic solvency.</p>
<p>However, this architecture suffers from a fatal structural flaw when exposed to the Diamond-Dybvig bank-run model. It assumes