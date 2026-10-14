---
source: "Ethereum Research"
source_type: research
title: "Measuring priority fees, positions and transaction classification of Ethereum blocks, July 2025 to October 2026"
author: ""
pub_date: "Wed, 14 Oct 2026 01:46:30 +0000"

importance: high
action: read_now
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-10-14
sources:
  - "https://ethresear.ch/t/measuring-priority-fees-positions-and-transaction-classification-of-ethereum-blocks-july-2025-to-october-2026/26156"
---
# Measuring priority fees, positions and transaction classification of Ethereum blocks, July 2025 to October 2026

> 출처: [Ethereum Research](https://ethresear.ch/t/measuring-priority-fees-positions-and-transaction-classification-of-ethereum-blocks-july-2025-to-october-2026/26156)  |  Wed, 14 Oct 2026 01:46:30 +0000

## AI 분석
**중요도:** high | **액션:** read_now

**요약:** 이더리움 L1 블록 내 트랜잭션의 우선순위 수수료, 위치, 유형 분류 및 MEV-Boost를 통한 블록 내 포지션 가격 책정 방식을 분석하는 연구.

**리서치 앵글:** 이더리움 L1 블록 내 트랜잭션 우선순위 및 MEV-Boost를 통한 포지션 가격 책정 방식 분석은 Third State의 주요 리서치 테마인 MEV와 직접적으로 연관됩니다.

## 원문 미리보기
<h1><a name="p-62768-h-13-october-2026-1" class="anchor" href="https://ethresear.ch#p-62768-h-13-october-2026-1" aria-label="Heading link"></a><em>13 October 2026</em></h1>
<h2><a name="p-62768-motivation-2" class="anchor" href="https://ethresear.ch#p-62768-motivation-2" aria-label="Heading link"></a>Motivation</h2>
<p>I work on pricing position within the block on Ethereum L1, mainly out of protocol through MEV-Boost (vs in protocol under EIP-1559). Any such design needs to know what the front of the block pays today, what types of transactions are there, and how they pay.</p>
<h2><a name="p-