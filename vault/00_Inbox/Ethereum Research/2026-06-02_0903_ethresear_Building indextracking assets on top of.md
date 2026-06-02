---
source: "Ethereum Research"
source_type: research
title: "Building index-tracking assets on top of options instead of debt"
author: ""
pub_date: "Mon, 01 Jun 2026 15:22:25 +0000"

importance: medium
action: weekly_review
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-06-02
sources:
  - "https://ethresear.ch/t/building-index-tracking-assets-on-top-of-options-instead-of-debt/25036"
---
# Building index-tracking assets on top of options instead of debt

> 출처: [Ethereum Research](https://ethresear.ch/t/building-index-tracking-assets-on-top-of-options-instead-of-debt/25036)  |  Mon, 01 Jun 2026 15:22:25 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review

**요약:** 이더리움 리서치 포스트는 부채 기반 대신 옵션을 활용하여 가격 지수를 추적하는 합성 자산을 구축하는 새로운 방법을 제안합니다.

**리서치 앵글:** 이 포스트는 옵션 기반 합성 자산 구축을 제안하며, 이는 RWA(실물자산) 지수 추적 및 DEX 경쟁 구도에 영향을 줄 수 있습니다.

## 원문 미리보기
<p><em>Special thanks to Vladimir Novakovski, Curve developers, and others for feedback and review.</em></p>
<p>Suppose that you have some ticker <code>T</code>, which represents a price index denominated in ETH. For example, <code>T</code> could equal the USD/ETH price (ie. inverse of ETH/USD). Or CPI/ETH (aka CPI/USD * USD/ETH). Or the same for any other commodity. Or more exotic indices (eg. average rent prices in a city). You want to give users the ability to have exposure to <code>T</code>.</p>
<p>In simpler terms, your goal is to create something like a synthetic asset that tracks <code>