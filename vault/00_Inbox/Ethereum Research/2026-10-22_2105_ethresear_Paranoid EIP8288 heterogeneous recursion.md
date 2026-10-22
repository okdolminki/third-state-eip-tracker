---
source: "Ethereum Research"
source_type: research
title: "Paranoid EIP-8288: heterogeneous recursion with an authenticated class bank"
author: ""
pub_date: "Thu, 22 Oct 2026 08:29:09 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-22
sources:
  - "https://ethresear.ch/t/paranoid-eip-8288-heterogeneous-recursion-with-an-authenticated-class-bank/26170"
---
# Paranoid EIP-8288: heterogeneous recursion with an authenticated class bank

> 출처: [Ethereum Research](https://ethresear.ch/t/paranoid-eip-8288-heterogeneous-recursion-with-an-authenticated-class-bank/26170)  |  Thu, 22 Oct 2026 08:29:09 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8288이 제안하는 재귀적 집계에서 다양한 증명 크기를 지원하는 이종 재귀의 구현 가능성을 탐구하는 글이다.

**리서치 앵글:** EIP-8288의 재귀적 집계 및 이종 재귀 논의는 L2 확장성 개선에 직접적으로 기여할 수 있다.

## 원문 미리보기
<p><a href="https://eips.ethereum.org/EIPS/eip-8288" rel="noopener nofollow ugc">EIP-8288</a> proposes recursive aggregation under a fixed protocol-level verification key. One backend choice worth exploring is whether recursive steps should support several approved proof sizes, so that small aggregates can use a smaller proving relation.</p>
<p>I implemented this kind of heterogeneous recursion in Parano1d, where small and large recursive state-transition proofs already run on a public mainnet. The construction uses a finite authenticated bank of verifier classes. I recently published the <a h