---
source: "Ethereum Research"
source_type: research
title: "Anatomy of a Fill: PropAMMs on Ethereum"
author: ""
pub_date: "Thu, 19 Nov 2026 18:17:34 +0000"

importance: medium
action: weekly_review
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-11-20
sources:
  - "https://ethresear.ch/t/anatomy-of-a-fill-propamms-on-ethereum/26271"
---
# Anatomy of a Fill: PropAMMs on Ethereum

> 출처: [Ethereum Research](https://ethresear.ch/t/anatomy-of-a-fill-propamms-on-ethereum/26271)  |  Thu, 19 Nov 2026 18:17:34 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review

**요약:** Uniswap 등 기존 AMM에서 발생하는 차익거래로 인한 LP 손실을 방지하기 위해 마켓 메이커가 블록 빌더에게 직접 가격을 스트리밍하는 PropAMM의 체결 구조와 트레이드오프를 분석합니다.

**리서치 앵글:** Uniswap의 LVR 손실 완화 및 MEV 구조 변화를 다루며, DEX 아키텍처 진화와 MEV 생태계 경쟁 구도 분석에 직접적으로 연관됩니다.

## 원문 미리보기
<p><em>Authors: <a class="mention" href="https://ethresear.ch/u/santidipaolo">@santidipaolo</a>, <a class="mention" href="https://ethresear.ch/u/jpinasco">@jpinasco</a>, <a class="mention" href="https://ethresear.ch/u/agustinpolfinance">@agustinpolfinance</a> (<a href="https://pol.finance" rel="noopener nofollow ugc">POL Finance</a>)</em></p>
<p>On Uniswap, the first trade of a block is often an arbitrageur hitting a price up to 12 seconds old, and liquidity providers pay for it. PropAMMs on Ethereum avoid this by having the market maker stream prices to block builders, at the cost of trusting