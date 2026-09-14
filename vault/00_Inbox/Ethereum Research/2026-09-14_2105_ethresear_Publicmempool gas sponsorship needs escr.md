---
source: "Ethereum Research"
source_type: research
title: "Public-mempool gas sponsorship needs escrow, a bond, or trust"
author: ""
pub_date: "Mon, 14 Sep 2026 11:07:59 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-09-14
sources:
  - "https://ethresear.ch/t/public-mempool-gas-sponsorship-needs-escrow-a-bond-or-trust/25995"
---
# Public-mempool gas sponsorship needs escrow, a bond, or trust

> 출처: [Ethereum Research](https://ethresear.ch/t/public-mempool-gas-sponsorship-needs-escrow-a-bond-or-trust/25995)  |  Mon, 14 Sep 2026 11:07:59 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 계약이 타인의 트랜잭션 가스를 지불하고, 공개 멤풀이 잠긴 자금이나 오프체인 신뢰 없이 해당 트랜잭션을 중계하려면 이 세 가지를 동시에 가질 수 없다는 것을 증명하는 글.

**리서치 앵글:** 계정 추상화(EIP-7702) 구현 시 가스 스폰서십 모델 설계에 대한 근본적인 제약을 다룸.

## 원문 미리보기
<h1><a name="p-62464-public-mempool-gas-sponsorship-needs-escrow-a-bond-or-trust-1" class="anchor" href="https://ethresear.ch#p-62464-public-mempool-gas-sponsorship-needs-escrow-a-bond-or-trust-1"></a>Public-mempool gas sponsorship needs escrow, a bond, or trust</h1>
<p><strong>In one sentence:</strong> if you want a contract to pay gas for someone else’s transaction, and you want the public mempool to relay that transaction with no locked money and no off-chain trust, you cannot have all three. This article proves that, and shows that every workaround falls into one of three buckets. That is 