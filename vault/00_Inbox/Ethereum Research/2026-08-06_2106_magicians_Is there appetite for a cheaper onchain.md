---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Is there appetite for a cheaper on-chain AO hash? (Ashlar, 14,232 gas vs Poseidon's 18,229)"
author: ""
pub_date: "Thu, 06 Aug 2026 08:05:44 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-06
sources:
  - "https://ethereum-magicians.org/t/is-there-appetite-for-a-cheaper-on-chain-ao-hash-ashlar-14-232-gas-vs-poseidons-18-229/29315"
---
# Is there appetite for a cheaper on-chain AO hash? (Ashlar, 14,232 gas vs Poseidon's 18,229)

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/is-there-appetite-for-a-cheaper-on-chain-ao-hash-ashlar-14-232-gas-vs-poseidons-18-229/29315)  |  Thu, 06 Aug 2026 08:05:44 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 온체인 ZK 증명 검증에 사용되는 AO 해시 함수 Ashlar가 기존 Poseidon보다 가스 비용을 크게 절감할 수 있어 롤업 및 ZK 친화적 애플리케이션의 효율성을 높일 수 있다는 내용.

**리서치 앵글:** L2 확장성: ZK 롤업의 온체인 증명 비용 절감으로 L2의 효율성 및 확장성 개선에 기여.

## 원문 미리보기
<h2><a name="p-72768-the-question-first-1" class="anchor" href="https://ethereum-magicians.org#p-72768-the-question-first-1" aria-label="Heading link"></a>The question, first</h2>
<p>On-chain verification of Merkle proofs over an arithmetization-oriented hash is a real cost centre; rollup withdrawal proofs, storage proofs, anything that verifies a ZK-friendly tree in Solidity. Poseidon is the de facto choice and costs ~18,229 gas per 2-to-1 hash at a saturated optimizer in the maintained <code>poseidon-solidity</code> implementation.</p>
<p>I have a design that measures <strong>14,232 gas</str