---
source: "Ethereum Research"
source_type: research
title: "Letting the base fee be a midpoint: a temporal liquidity authorization for EIP-1559"
author: ""
pub_date: "Thu, 10 Sep 2026 01:00:57 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-09-10
sources:
  - "https://ethresear.ch/t/letting-the-base-fee-be-a-midpoint-a-temporal-liquidity-authorization-for-eip-1559/25958"
---
# Letting the base fee be a midpoint: a temporal liquidity authorization for EIP-1559

> 출처: [Ethereum Research](https://ethresear.ch/t/letting-the-base-fee-be-a-midpoint-a-temporal-liquidity-authorization-for-eip-1559/25958)  |  Thu, 10 Sep 2026 01:00:57 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-1559의 기본 수수료가 현재 최저치인 점을 지적하며, 이를 중간 지점으로 변경하고 시간적 선호도를 반영하여 트랜잭션 우선순위를 개선하는 방안을 제안한다.

**리서치 앵글:** EIP-1559 기본 수수료 메커니즘 변경 제안은 MEV 및 L2 확장성에 중대한 영향을 미칠 수 있다.

## 원문 미리보기
<p>Date: September 9, 2026</p>
<p>Under EIP-1559 the base fee is a floor. Every included transaction pays at least <code>base_fee</code> per gas, no sender can offer to take a later position in exchange for paying less, and a transaction whose <code>max_fee</code> falls below the base fee is invalid before it reaches a block.</p>
<p>The protocol also observes willingness to pay rather than temporal preference. A liquidation that loses its value within seconds and a treasury transfer that would be equally good three blocks later can submit the same bid, and nothing distinguishes them. The secon