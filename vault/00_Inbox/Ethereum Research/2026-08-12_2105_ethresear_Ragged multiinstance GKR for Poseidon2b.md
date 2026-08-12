---
source: "Ethereum Research"
source_type: research
title: "Ragged multi-instance GKR for Poseidon2b: one walk, unequal regions, no max-width padding"
author: ""
pub_date: "Wed, 12 Aug 2026 07:20:07 +0000"

importance: medium
action: weekly_review
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-08-12
sources:
  - "https://ethresear.ch/t/ragged-multi-instance-gkr-for-poseidon2b-one-walk-unequal-regions-no-max-width-padding/25691"
---
# Ragged multi-instance GKR for Poseidon2b: one walk, unequal regions, no max-width padding

> 출처: [Ethereum Research](https://ethresear.ch/t/ragged-multi-instance-gkr-for-poseidon2b-one-walk-unequal-regions-no-max-width-padding/25691)  |  Wed, 12 Aug 2026 07:20:07 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review

**요약:** 이더리움의 해시 집약적인 증명 시스템(예: 검증자 집계, WHIR)에서 Poseidon2b 해시 함수의 효율성을 높이기 위한 GKR 최적화 방안을 제안합니다.

**리서치 앵글:** L2 확장성: ZK 롤업의 핵심 구성 요소인 해시 함수의 효율성 개선은 L2 확장성 및 비용 절감에 직접적인 영향을 미칩니다.

## 원문 미리보기
<p>Two current Ethereum proving efforts are explicitly hash-heavy. A recent post-quantum validator aggregation design says that verification is dominated by hash evaluations, while a separate WHIR implementation reports Poseidon2 Merkle hashing at 58% of GPU time for a representative configuration:</p>
<aside class="quote quote-modified" data-post="1" data-topic="25040">
  <div class="title">
    <div class="quote-controls"></div>
    <img alt="" width="24" height="24" src="https://ethresear.ch/user_avatar/ethresear.ch/tcoratger/48/20719_2.png" class="avatar">
    <div class="quote-title__text