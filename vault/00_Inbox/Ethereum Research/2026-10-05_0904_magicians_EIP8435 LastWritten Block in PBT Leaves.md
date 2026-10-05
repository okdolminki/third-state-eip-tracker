---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8435: Last-Written Block in PBT Leaves"
author: ""
pub_date: "Sun, 04 Oct 2026 18:20:38 +0000"

importance: medium
action: weekly_review
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-10-05
sources:
  - "https://ethereum-magicians.org/t/eip-8435-last-written-block-in-pbt-leaves/29860"
---
# EIP-8435: Last-Written Block in PBT Leaves

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8435-last-written-block-in-pbt-leaves/29860)  |  Sun, 04 Oct 2026 18:20:38 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review

**요약:** EIP-8188의 최근 쓰기 블록 기록 기능을 분할 바이너리 트리(PBT) 리프에 적용하여 상태 만료 및 스토리지 관리를 최적화하려는 제안입니다.

**리서치 앵글:** 이더리움의 장기 상태 만료(State Expiry) 구조 변화는 L1/L2 스토리지 접근 비용 및 인프라 확장성에 중장기적 영향을 미칠 수 있습니다.

## 원문 미리보기
<h1><a name="p-74842-carrying-eip-8188s-write-age-signal-into-the-partitioned-binary-tree-1" class="anchor" href="https://ethereum-magicians.org#p-74842-carrying-eip-8188s-write-age-signal-into-the-partitioned-binary-tree-1" aria-label="Heading link"></a>Carrying EIP-8188’s write-age signal into the Partitioned Binary Tree</h1>
<p><a href="https://eips.ethereum.org/EIPS/eip-8188" rel="noopener nofollow ugc">EIP-8188</a> records, for every account and storage slot, the block at which it was last written. That gives clients a consensus-level signal for separating recently written state from stat