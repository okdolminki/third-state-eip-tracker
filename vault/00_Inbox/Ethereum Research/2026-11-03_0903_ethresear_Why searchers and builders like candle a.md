---
source: "Ethereum Research"
source_type: research
title: "Why searchers and builders like candle auctions (and why it matters for the builder market post-Glamsterdam)"
author: ""
pub_date: "Mon, 02 Nov 2026 13:00:47 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-03
sources:
  - "https://ethresear.ch/t/why-searchers-and-builders-like-candle-auctions-and-why-it-matters-for-the-builder-market-post-glamsterdam/26211"
---
# Why searchers and builders like candle auctions (and why it matters for the builder market post-Glamsterdam)

> 출처: [Ethereum Research](https://ethresear.ch/t/why-searchers-and-builders-like-candle-auctions-and-why-it-matters-for-the-builder-market-post-glamsterdam/26211)  |  Mon, 02 Nov 2026 13:00:47 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 캔들 경매(무작위 마감 기한을 가진 공개 입찰)가 봉인 입찰보다 빌더 수익을 높여, 글램스터담 이후 이더리움 빌더 시장에서 기존 참여자들이 외부 입찰을 제한하며 현재의 공개 입찰 시스템을 유지하려는 강한 동기를 부여할 수 있다.

**리서치 앵글:** MEV 및 빌더 시장 경쟁 구도에 대한 심층 분석으로, 글램스터담 이후 이더리움 프로토콜 변화가 시장 참여자 인센티브에 미치는 영향을 다룬다.

## 원문 미리보기
<p><em>tl;dr Open-bidding with random deadline (candle auctions) and few auction participants can lead to higher bidder profits than sealed-bid auctions. This is already true in a one-shot auction without explicit coordination or collusion. For the Ethereum builder-market post-Glamsterdam, I conjecture that this gives current participants a strong incentive to maintain the current open-bid auction by restricting outside bidding and per-missioning participation in relay auctions.</em></p>
<p>In this post I want to formalize a piece of folk knowledge which I think is well-known among many search