---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8292: PQ Attestation Aggregators"
author: ""
pub_date: "Fri, 12 Jun 2026 11:11:32 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-12
sources:
  - "https://ethereum-magicians.org/t/eip-8292-pq-attestation-aggregators/28778"
---
# EIP-8292: PQ Attestation Aggregators

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8292-pq-attestation-aggregators/28778)  |  Fri, 12 Jun 2026 11:11:32 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8292는 포스트 퀀텀 이더리움에서 BLS 서명을 대체하는 PQ 해시 기반 서명의 효율적인 집계를 위한 새로운 '어그리게이터' 역할을 도입합니다.

**리서치 앵글:** LST/LRT 구조와 관련하여, 이더리움의 핵심 합의 메커니즘 및 검증자 서명 방식의 변화는 LST/LRT 프로토콜의 기반 보안 및 운영 모델에 장기적인 영향을 미칠 수 있습니다.

## 원문 미리보기
<p>Discussion topic for EIP-8292: PQ Attestation Aggregators<br>
PR: <a href="https://github.com/ethereum/EIPs/pull/11777" class="inline-onebox" rel="noopener nofollow ugc">Add EIP: Post-Quantum(PQ) Attestation Aggregators by anshalshukla · Pull Request #11777 · ethereum/EIPs · GitHub</a></p>
<p><strong>Abstract</strong><br>
PQ Ethereum replaces BLS signatures with larger post-quantum hash-based signatures that cannot be cheaply aggregated directly. The <code>L*</code> hard fork introduces a new opt-in <strong>aggregator</strong> role: high-spec nodes that generate succinct proofs verifying ma