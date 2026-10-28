---
source: "Ethereum Research"
source_type: research
title: "Ephemeral Rollup: The New 'L1.5' of Ethereum"
author: ""
pub_date: "Wed, 28 Oct 2026 02:40:27 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-28
sources:
  - "https://ethresear.ch/t/ephemeral-rollup-the-new-l1-5-of-ethereum/26187"
---
# Ephemeral Rollup: The New "L1.5" of Ethereum

> 출처: [Ethereum Research](https://ethresear.ch/t/ephemeral-rollup-the-new-l1-5-of-ethereum/26187)  |  Wed, 28 Oct 2026 02:40:27 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 이더리움의 핵심 역할인 상태 전이 검증과 롤업의 사용자 상태 보유 문제를 해결하며, 네이티브 계정 추상화와 연관된 새로운 'L1.5' 개념인 Ephemeral Rollup을 제안한다.

**리서치 앵글:** L2 확장성 및 계정 추상화(EIP-7702)와 관련된 이더리움 아키텍처의 근본적인 변화 가능성을 탐구한다.

## 원문 미리보기
<h1><a name="p-62888-ephemeral-rollup-the-new-l15-of-ethereum-1" class="anchor" href="https://ethresear.ch#p-62888-ephemeral-rollup-the-new-l15-of-ethereum-1" aria-label="Heading link"></a>Ephemeral Rollup: The New “L1.5” of Ethereum</h1>
<h2><a name="p-62888-tldr-2" class="anchor" href="https://ethresear.ch#p-62888-tldr-2" aria-label="Heading link"></a>TLDR;</h2>
<p>Ethereum’s core job has always been verifying state transitions. While rollups made that verification succinct, they at the same time hold their users’ state, which is why every rollup needs an exit. Native account abstraction (<a