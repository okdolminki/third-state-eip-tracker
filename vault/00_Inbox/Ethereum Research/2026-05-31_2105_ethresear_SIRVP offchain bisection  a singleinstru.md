---
source: "Ethereum Research"
source_type: research
title: "SI-RVP: off-chain bisection + a single-instruction Groth16 proof for optimistic-rollup dispute resolution"
author: ""
pub_date: "Sat, 30 May 2026 08:07:39 +0000"

importance: high
action: read_now
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-05-31
sources:
  - "https://ethresear.ch/t/si-rvp-off-chain-bisection-a-single-instruction-groth16-proof-for-optimistic-rollup-dispute-resolution/25005"
---
# SI-RVP: off-chain bisection + a single-instruction Groth16 proof for optimistic-rollup dispute resolution

> 출처: [Ethereum Research](https://ethresear.ch/t/si-rvp-off-chain-bisection-a-single-instruction-groth16-proof-for-optimistic-rollup-dispute-resolution/25005)  |  Sat, 30 May 2026 08:07:39 +0000

## AI 분석
**중요도:** high | **액션:** read_now

**요약:** 옵티미스틱 롤업의 분쟁 해결 프로토콜을 개선하여 오프체인 이분법과 단일 명령어 Groth16 증명을 통해 온체인 가스 비용을 획기적으로 절감하는 방안을 제시한다.

**리서치 앵글:** 옵티미스틱 롤업의 분쟁 해결 효율성 개선을 통한 L2 확장성 강화.

## 원문 미리보기
<h2><a name="p-60240-tldr-1" class="anchor" href="https://ethresear.ch#p-60240-tldr-1"></a>TL;DR</h2>
<p>We built and measured a hybrid optimistic-rollup dispute protocol that keeps the 1-of-N permissionless trust model of Cannon but moves the bisection <strong>off-chain</strong> and replaces the on-chain MIPS leaf execution with a <strong>single-instruction Groth16 proof</strong>. On a Sepolia PoC the contested path is <strong>4 core dispute transactions (~0.72M gas), plus the resolveDispute settlement (~0.11M) — 5 on-chain txs, ~0.83M total</strong>. That is roughly an order of magnitude bel