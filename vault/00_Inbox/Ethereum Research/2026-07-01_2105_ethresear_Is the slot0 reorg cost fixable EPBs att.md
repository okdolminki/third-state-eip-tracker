---
source: "Ethereum Research"
source_type: research
title: "Is the slot-0 reorg cost fixable? EPBs attestation deadline study"
author: ""
pub_date: "Wed, 01 Jul 2026 07:57:48 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-01
sources:
  - "https://ethresear.ch/t/is-the-slot-0-reorg-cost-fixable-epbs-attestation-deadline-study/25338"
---
# Is the slot-0 reorg cost fixable? EPBs attestation deadline study

> 출처: [Ethereum Research](https://ethresear.ch/t/is-the-slot-0-reorg-cost-fixable-epbs-attestation-deadline-study/25338)  |  Wed, 01 Jul 2026 07:57:48 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 슬롯-0 리오그 비용 문제 해결 가능성 및 EPB(Epoch Boundary)의 증명 마감 기한 선택에 대한 연구.

**리서치 앵글:** L2 확장성 및 기관 DeFi 도입에 필수적인 이더리움 L1의 안정성과 보안에 대한 연구.

## 원문 미리보기
<blockquote>
<p>Thanks to <a class="mention" href="https://ethresear.ch/u/potuz">@potuz</a> <a class="mention" href="https://ethresear.ch/u/misilva73">@misilva73</a> and <a class="mention" href="https://ethresear.ch/u/nero_eth">@Nero_eth</a> for the discussions and motivation to elaborate this brief research as well as for the reviews.</p>
</blockquote>
<p><em>Glamsterdam has to pick where the attestation deadline sits — second 2, 3, or 4 of the slot — and the epoch boundary is the reason that choice is hard. Twenty-one months of mainnet data point to fixable production engineering rather than