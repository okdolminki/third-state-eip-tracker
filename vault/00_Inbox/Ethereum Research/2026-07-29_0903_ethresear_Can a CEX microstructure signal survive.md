---
source: "Ethereum Research"
source_type: research
title: "Can a CEX microstructure signal survive Ethereum execution latency and MEV?"
author: ""
pub_date: "Tue, 28 Jul 2026 21:53:23 +0000"

importance: medium
action: weekly_review
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-07-29
sources:
  - "https://ethresear.ch/t/can-a-cex-microstructure-signal-survive-ethereum-execution-latency-and-mev/25562"
---
# Can a CEX microstructure signal survive Ethereum execution latency and MEV?

> 출처: [Ethereum Research](https://ethresear.ch/t/can-a-cex-microstructure-signal-survive-ethereum-execution-latency-and-mev/25562)  |  Tue, 28 Jul 2026 21:53:23 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review

**요약:** CEX 거래 신호가 이더리움 DEX 유동성 공급 시 역선택을 줄이고 MEV 환경에서 유효한지 탐구하는 연구.

**리서치 앵글:** DEX 경쟁구도와 MEV 테마에 직접적으로 연관되며, CEX 신호의 DEX 적용 가능성을 통해 기관 DeFi 도입 전략에도 시사점을 제공한다.

## 원문 미리보기
<h2><a name="p-61574-motivation-1" class="anchor" href="https://ethresear.ch#p-61574-motivation-1"></a>Motivation</h2>
<p>We are investigating a narrow cross-venue market-microstructure question:</p>
<p><strong>Can a predictive signal generated from BTC and ETH perpetual trades on a centralized exchange reduce adverse selection when liquidity is provided on an Ethereum-based decentralized venue?</strong></p>
<p>We are not assuming that a profitable CEX construct can simply be copied to a DEX. Our starting prior is deliberately sceptical. Even if the source signal is informative, the edge may d