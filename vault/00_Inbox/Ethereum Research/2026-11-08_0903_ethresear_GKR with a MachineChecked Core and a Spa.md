---
source: "Ethereum Research"
source_type: research
title: "GKR with a Machine-Checked Core, and a Sparse Prover Made Faster with Byte-Identical Proofs"
author: ""
pub_date: "Sat, 07 Nov 2026 15:08:19 +0000"

importance: high
action: read_now
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-11-08
sources:
  - "https://ethresear.ch/t/gkr-with-a-machine-checked-core-and-a-sparse-prover-made-faster-with-byte-identical-proofs/26226"
---
# GKR with a Machine-Checked Core, and a Sparse Prover Made Faster with Byte-Identical Proofs

> 출처: [Ethereum Research](https://ethresear.ch/t/gkr-with-a-machine-checked-core-and-a-sparse-prover-made-faster-with-byte-identical-proofs/26226)  |  Sat, 07 Nov 2026 15:08:19 +0000

## AI 분석
**중요도:** high | **액션:** read_now

**요약:** 2025년 Vitalik의 GKR 튜토리얼에서 영감을 받아, 일반 계층 회로에 대한 GKR의 기계 검증된 건전성 경계를 확립하고 희소 머클 업데이트에 대한 건전성 증명을 개발했다.

**리서치 앵글:** L2 확장성: GKR 및 희소 머클 업데이트의 건전성 증명은 L2 확장성 솔루션의 보안 및 효율성 향상에 기여한다.

## 원문 미리보기
<p>In October 2025, Vitalik’s <a href="https://vitalik.eth.limo/general/2025/10/19/gkr.html" rel="noopener nofollow ugc">GKR tutorial</a> was my first encounter with GKR. Its central observation, that the protocol commits only to a circuit’s input and output and never to the layers in between, made GKR look like the natural tool for proving hash-heavy computation. A year later, that has led to what is, as far as we know, the first machine-checked soundness bound for GKR on general layered circuits, in Isabelle/HOL. The same work produced a soundness proof for sparse-Merkle updates built on tha