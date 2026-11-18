---
source: "Ethereum Research"
source_type: research
title: "EIP-8288: the networking side of recursive aggregation"
author: ""
pub_date: "Wed, 18 Nov 2026 09:58:32 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-18
sources:
  - "https://ethresear.ch/t/eip-8288-the-networking-side-of-recursive-aggregation/26263"
---
# EIP-8288: the networking side of recursive aggregation

> 출처: [Ethereum Research](https://ethresear.ch/t/eip-8288-the-networking-side-of-recursive-aggregation/26263)  |  Wed, 18 Nov 2026 09:58:32 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** Vitalik Buterin이 공동 저술한 EIP-8288은 재귀적 STARK 기반의 대역폭 효율적인 멤풀을 정의하며, 트랜잭션의 의존성 처리 방식을 다룹니다.

**리서치 앵글:** 재귀적 STARK 기반 멤풀 효율성 개선은 L2 확장성 및 전반적인 이더리움 네트워크 성능에 긍정적인 영향을 미칠 수 있습니다.

## 원문 미리보기
<p>author: Csaba Kiraly <a class="mention" href="https://ethresear.ch/u/cskiraly">@cskiraly</a></p>
<p><a href="https://eips.ethereum.org/EIPS/eip-8288" rel="noopener nofollow ugc">EIP-8288</a>, by Vitalik Buterin and Thomas Coratger, specifies the <a href="https://ethresear.ch/t/recursive-stark-based-bandwidth-efficient-mempool/23838">Recursive-STARK-based bandwidth-efficient mempool</a> that Vitalik Buterin proposed in an earlier post on this forum. A transaction declares which post-quantum signatures and proofs it depends on. As transactions spread, mempool nodes fold those dependencies int