---
source: "Ethereum Research"
source_type: research
title: "How Much Screening Buys a Second? Speed, Selection, and the Maker's Spread"
author: ""
pub_date: "Thu, 15 Oct 2026 13:04:19 +0000"

importance: medium
action: weekly_review
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-10-16
sources:
  - "https://ethresear.ch/t/how-much-screening-buys-a-second-speed-selection-and-the-makers-spread/26158"
---
# How Much Screening Buys a Second? Speed, Selection, and the Maker's Spread

> 출처: [Ethereum Research](https://ethresear.ch/t/how-much-screening-buys-a-second-speed-selection-and-the-makers-spread/26158)  |  Thu, 15 Oct 2026 13:04:19 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review

**요약:** LP가 지연된 호가 노출에 따른 손실을 방어하기 위해 신속한 가격 갱신과 유해 주문 스크리닝 간의 손익분기 상관관계를 수학적으로 모델링하고 USDC-WETH 풀 데이터로 검증한 연구입니다.

**리서치 앵글:** DEX 경쟁구도 및 MEV 테마와 직결되며, Uniswap v4 훅 기반 LVR 완화 및 오더플로우 스크리닝 설계가 LP 수익성에 미치는 영향을 평가하는 데 유용합니다.

## 원문 미리보기
<p>We study the spread a liquidity provider needs to break even against counterparties that can exploit a stale quote, and we place two defenses on a single scale: repricing sooner and screening informed flow. A break-even condition pins down the exact screening rate at which a slower maker matches a faster unscreened venue: the selection that buys back the extra staleness. The result requires only an integrable price innovation and therefore holds under jumps, atoms and infinite variance. We take the model to four USDC-WETH pools benchmarked against Binance ETH-USDT from June to August 2026.<