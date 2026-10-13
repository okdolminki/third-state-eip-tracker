---
source: "Ethereum Research"
source_type: research
title: "Rapidblocks, take two: a pipelined consensus for independent blocks"
author: ""
pub_date: "Tue, 13 Oct 2026 08:27:07 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-13
sources:
  - "https://ethresear.ch/t/rapidblocks-take-two-a-pipelined-consensus-for-independent-blocks/26152"
---
# Rapidblocks, take two: a pipelined consensus for independent blocks

> 출처: [Ethereum Research](https://ethresear.ch/t/rapidblocks-take-two-a-pipelined-consensus-for-independent-blocks/26152)  |  Tue, 13 Oct 2026 08:27:07 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 이더리움 L1의 블록 빌딩 파이프라인을 개선하여 독립적인 블록 생성을 통해 슬롯 시간을 단축하고 효율성을 높이는 새로운 파이프라인 합의 메커니즘을 제안한다.

**리서치 앵글:** L1 블록 처리 효율성 개선이 L2 확장성 및 전반적인 이더리움 생태계 성능에 미치는 영향을 분석한다.

## 원문 미리보기
<p>Last year, <a href="https://ethresear.ch/t/rapidblocks-minimizing-merge-conflicts-in-the-block-building-pipeline/22590">rapidblocks</a> proposed building blocks that don’t depend on their immediate predecessor. Block i+1 builds on i−1’s state, and respects i’s <a href="https://ethresear.ch/t/bafs-scaling-ethereum-l1-with-block-level-access-filters/22585">BMF</a>, a Bloom filter of the keys i modified. A block can then be skipped without a reorg, and slots can get much shorter. That post’s design part ended with a promissory note: <em>“I think we can create a consensus mechanism that is pipe