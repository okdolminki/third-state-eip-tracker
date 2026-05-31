---
source: "Ethereum Research"
source_type: research
title: "Coordination is Self-Defeating: A Structural Proof for Diversity-Weighted Byzantine Fault Tolerance"
author: ""
pub_date: "Sun, 24 May 2026 07:32:49 +0000"

importance: high
action: read_now
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-05-31
sources:
  - "https://ethresear.ch/t/coordination-is-self-defeating-a-structural-proof-for-diversity-weighted-byzantine-fault-tolerance/24935"
---
# Coordination is Self-Defeating: A Structural Proof for Diversity-Weighted Byzantine Fault Tolerance

> 출처: [Ethereum Research](https://ethresear.ch/t/coordination-is-self-defeating-a-structural-proof-for-diversity-weighted-byzantine-fault-tolerance/24935)  |  Sun, 24 May 2026 07:32:49 +0000

## AI 분석
**중요도:** high | **액션:** read_now

**요약:** 기존 비잔틴 장애 허용(BFT) 합의 시스템들이 정직한 슈퍼 과반수를 가정하지만 구조적으로 증명하지 못했음을 지적하며, 비잔틴 조정이 구조적으로 자멸적임을 증명하는 연구입니다.

**리서치 앵글:** DeFi 프로토콜 및 LST/LRT의 근간이 되는 블록체인 합의 시스템의 구조적 보안성에 대한 심층 분석으로, 기관 DeFi 도입 및 LST/LRT 구조의 신뢰도에 간접적 영향을 미칠 수 있습니다.

## 원문 미리보기
<p>Coordination is Self-Defeating: A Structural Proof for Diversity-Weighted Byzantine Fault Tolerance</p>
<p>License: CC0 — this belongs to everyone</p>
<p>Implementation: TRION Protocol — live on 37 chains</p>
<p>Date: May 2026</p>
<p>Abstract</p>
<p>Every Byzantine Fault Tolerant consensus system ever deployed — pBFT, Tendermint, HotStuff, Casper FFG, Streamlet — requires honest supermajority as an assumption. They assert ⅔ honest weight must hold and proceed on that basis. None of them prove it structurally.</p>
<p>This post presents a proof that Byzantine coordination is structurally self