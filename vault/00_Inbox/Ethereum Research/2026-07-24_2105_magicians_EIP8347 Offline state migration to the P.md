---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8347: Offline state migration to the PBT"
author: ""
pub_date: "Fri, 24 Jul 2026 11:10:43 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-24
sources:
  - "https://ethereum-magicians.org/t/eip-8347-offline-state-migration-to-the-pbt/29089"
---
# EIP-8347: Offline state migration to the PBT

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8347-offline-state-migration-to-the-pbt/29089)  |  Fri, 24 Jul 2026 11:10:43 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8347은 이더리움의 상태 저장 방식을 기존 MPT에서 PBT로 오프라인으로 전환하는 방안을 제안합니다.

**리서치 앵글:** 이더리움의 근본적인 상태 구조 변경은 L2 확장성 및 전반적인 네트워크 효율성에 중장기적인 영향을 미칠 것입니다.

## 원문 미리보기
<p>Discussion topic for EIP-8347</p>
<h4><a name="p-72092-abstract-1" class="anchor" href="https://ethereum-magicians.org#p-72092-abstract-1" aria-label="Heading link"></a>Abstract</h4>
<p>This EIP specifies an <strong>**offline**</strong> migration of Ethereum’s state from the hexary Merkle Patricia Trie (MPT) to the Partitioned Binary Tree (PBT) defined in EIP-8297 (the successor to the unified binary tree of EIP-7864).</p>
<p>The full state at a finalized <strong>**anchor block `ANCHOR_BLOCK`**</strong> is converted off the consensus-critical path. The result is distributed as a byte-canoni