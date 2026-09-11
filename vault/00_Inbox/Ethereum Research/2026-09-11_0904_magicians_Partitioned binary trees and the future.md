---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Partitioned binary trees and the future of code delegation"
author: ""
pub_date: "Thu, 10 Sep 2026 15:51:55 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-09-11
sources:
  - "https://ethereum-magicians.org/t/partitioned-binary-trees-and-the-future-of-code-delegation/29638"
---
# Partitioned binary trees and the future of code delegation

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/partitioned-binary-trees-and-the-future-of-code-delegation/29638)  |  Thu, 10 Sep 2026 15:51:55 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 이더리움의 핵심 EIP인 EIP-8297(Partitioned Binary Tree)은 기존 MPT를 이진 트리 구조로 대체하고 새로운 코드 저장 형식을 도입하여 비용 절감 및 효율성 향상을 목표로 합니다.

**리서치 앵글:** 이더리움의 핵심 구조 변경은 L2 확장성 및 전반적인 프로토콜 효율성에 중장기적 영향을 미칠 수 있습니다.

## 원문 미리보기
<p>A major EIP being considered for I* is the partitioned binary tree (PBT): <a href="https://eips.ethereum.org/EIPS/eip-8297" class="inline-onebox">EIP-8297: Partitioned Binary Tree</a></p>
<p>This replaces the hexary MPT with a binary tree structure that is well-designed with a decade of lessons and thought of what is ideal for Ethereum, including cost savings for provers, adjacent access, VOPS syncing, and other goals.</p>
<p>One very recent feature addition of the PBT that has been under-discussed is the new code storage format. Essentially: <strong>contract code will be stored in a separa