---
source: "Ethereum Research"
source_type: research
title: "Proof boundaries in a minimal homomorphic tally for token weighted voting"
author: ""
pub_date: "Thu, 27 Aug 2026 15:13:25 +0000"

importance: medium
action: weekly_review
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-08-28
sources:
  - "https://ethresear.ch/t/proof-boundaries-in-a-minimal-homomorphic-tally-for-token-weighted-voting/25831"
---
# Proof boundaries in a minimal homomorphic tally for token weighted voting

> 출처: [Ethereum Research](https://ethresear.ch/t/proof-boundaries-in-a-minimal-homomorphic-tally-for-token-weighted-voting/25831)  |  Thu, 27 Aug 2026 15:13:25 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review

**요약:** 토큰 가중치 투표를 위한 동형 합산 방식에서 증명의 경계를 정의하고, 이를 이더리움 세폴리아에서 구현 및 검증한 연구.

**리서치 앵글:** 기관 DeFi 도입을 위한 투표 시스템의 신뢰성과 프라이버시 강화 방안 연구.

## 원문 미리보기
<h2><a name="p-62126-motivation-1" class="anchor" href="https://ethresear.ch#p-62126-motivation-1"></a>Motivation</h2>
<p>Homomorphic tallying is easy to summarize: encrypt each ballot, add the ciphertexts, and decrypt the sum. The harder part is specifying exactly what a proof must bind for that sum to represent an election rather than merely a valid group computation.</p>
<p>I built Commitra, a solo research implementation of token weighted voting, and exercised it end to end on Ethereum Sepolia. It uses two Groth16 circuits, BabyJubJub ElGamal, browser side proving, a relayer, and a fixed t