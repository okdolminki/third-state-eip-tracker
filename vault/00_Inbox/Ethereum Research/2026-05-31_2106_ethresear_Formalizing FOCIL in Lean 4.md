---
source: "Ethereum Research"
source_type: research
title: "Formalizing FOCIL in Lean 4"
author: ""
pub_date: "Mon, 25 May 2026 14:56:57 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-05-31
sources:
  - "https://ethresear.ch/t/formalizing-focil-in-lean-4/24950"
---
# Formalizing FOCIL in Lean 4

> 출처: [Ethereum Research](https://ethresear.ch/t/formalizing-focil-in-lean-4/24950)  |  Mon, 25 May 2026 14:56:57 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-7805(FOCIL)의 검열 저항성 메커니즘이 Lean 4를 통해 공식적으로 검증되었으며, 이는 1-out-of-N 정직성 가정을 기반으로 한다.

**리서치 앵글:** 검열 저항성 강화는 MEV 완화 및 공정한 트랜잭션 포함에 기여하여 DeFi 생태계의 신뢰성을 높인다.

## 원문 미리보기
<p>FOCIL (<a href="https://eips.ethereum.org/EIPS/eip-7805" rel="noopener nofollow ugc">EIP-7805</a>) is the censorship-resistance headliner scheduled for Hegotá. The selling point everyone repeats is “1-out-of-N honesty among IL committee members”: one non-equivocating member listing a transaction is enough to force its inclusion in the canonical block.</p>
<p>I wanted to know what that claim looks like under a microscope. The short answer is that it holds, derived end-to-end from Ethereum’s standard <span class="math">&gt;2/3</span> honest-validator assumption, but writing it down in Lean su