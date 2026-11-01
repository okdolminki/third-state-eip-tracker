---
source: "Ethereum Research"
source_type: research
title: "PropAMM fills on Ethereum mainnet and PropAMM support for TEMBRI (toolbox): same-block quotes, a small spread, and flow taken from lagging AMMs"
author: ""
pub_date: "Sat, 31 Oct 2026 21:25:55 +0000"

importance: medium
action: weekly_review
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-11-01
sources:
  - "https://ethresear.ch/t/propamm-fills-on-ethereum-mainnet-and-propamm-support-for-tembri-toolbox-same-block-quotes-a-small-spread-and-flow-taken-from-lagging-amms/26201"
---
# PropAMM fills on Ethereum mainnet and PropAMM support for TEMBRI (toolbox): same-block quotes, a small spread, and flow taken from lagging AMMs

> 출처: [Ethereum Research](https://ethresear.ch/t/propamm-fills-on-ethereum-mainnet-and-propamm-support-for-tembri-toolbox-same-block-quotes-a-small-spread-and-flow-taken-from-lagging-amms/26201)  |  Sat, 31 Oct 2026 21:25:55 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review

**요약:** PropAMM은 단일 메이커가 가격을 설정하는 온체인 거래소로, 9개의 이더리움 PropAMM에서 30일간의 거래 데이터를 분석하여 WETH/스테이블코인 거래의 성능을 평가했습니다.

**리서치 앵글:** PropAMM의 온체인 거래 메커니즘 분석은 DEX 경쟁 구도에 대한 통찰을 제공합니다.

## 원문 미리보기
<h2><a name="p-62924-abstract-1" class="anchor" href="https://ethresear.ch#p-62924-abstract-1" aria-label="Heading link"></a>Abstract</h2>
<p>PropAMMs are on-chain venues whose prices are set by a single maker. The maker<br>
pushes quote state on-chain, and fills read that state. We decoded 92,627<br>
fills on nine Ethereum PropAMMs over 30 days (10 September to 9 October 2026)<br>
from execution data. We priced the 69,827 WETH/stablecoin fills against<br>
Binance one-second trades.</p>
<ul>
<li>Three of the registry venues accept maker state only if it is stamped with<br>
the current block’s 