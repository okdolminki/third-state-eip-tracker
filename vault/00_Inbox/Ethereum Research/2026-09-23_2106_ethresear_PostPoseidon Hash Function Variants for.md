---
source: "Ethereum Research"
source_type: research
title: "Post-Poseidon: Hash Function Variants for Ethereum"
author: ""
pub_date: "Wed, 23 Sep 2026 09:50:36 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-09-23
sources:
  - "https://ethresear.ch/t/post-poseidon-hash-function-variants-for-ethereum/26071"
---
# Post-Poseidon: Hash Function Variants for Ethereum

> 출처: [Ethereum Research](https://ethresear.ch/t/post-poseidon-hash-function-variants-for-ethereum/26071)  |  Wed, 23 Sep 2026 09:50:36 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 이더리움 프로토콜을 위한 해시 함수 선택의 중요성과 다양한 변형의 장단점을 논의하며, 새로운 증명 시스템(Flock)의 등장에 따른 변화를 다룬다.

**리서치 앵글:** 이더리움의 핵심 해시 함수 변경 논의는 L2 확장성 및 전반적인 프로토콜 효율성에 중장기적 영향을 미칠 수 있다.

## 원문 미리보기
<h2><a name="p-62615-introduction-1" class="anchor" href="https://ethresear.ch#p-62615-introduction-1" aria-label="Heading link"></a>Introduction</h2>
<p>With the emergence of Flock as a PQ proof system for binary circuits (esp. hashes),   Ethereum   no longer requires specific circuit-friendly hashes for protocols whose computation would be proven. Still, the question of which hash function to choose is non-trivial, as they all have advantages and disadvantages in the context of the Ethereum protocol.</p>
<h2><a name="p-62615-usage-2" class="anchor" href="https://ethresear.ch#p-62615-usage-2"