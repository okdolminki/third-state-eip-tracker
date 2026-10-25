---
source: "Ethereum Research"
source_type: research
title: "A hash-only rollup: OP Stack L2 accounts as Lamport-style hash chains, no ECDSA inside the L2"
author: ""
pub_date: "Sat, 24 Oct 2026 23:24:10 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-25
sources:
  - "https://ethresear.ch/t/a-hash-only-rollup-op-stack-l2-accounts-as-lamport-style-hash-chains-no-ecdsa-inside-the-l2/26172"
---
# A hash-only rollup: OP Stack L2 accounts as Lamport-style hash chains, no ECDSA inside the L2

> 출처: [Ethereum Research](https://ethresear.ch/t/a-hash-only-rollup-op-stack-l2-accounts-as-lamport-style-hash-chains-no-ecdsa-inside-the-l2/26172)  |  Sat, 24 Oct 2026 23:24:10 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** OP Stack L2에서 ECDSA 서명 없이 해시 체인으로 계정을 관리하고 트랜잭션을 처리하는 새로운 방식을 제안한다.

**리서치 앵글:** OP Stack L2의 새로운 계정 모델이 L2 확장성과 계정 추상화(EIP-7702)에 미치는 영향을 연구한다.

## 원문 미리보기
<p><em>Disclosure: I’m the founder of bb84, the payments app that runs on this chain. Feedback, especially critical feedback, is very welcome.</em></p>
<h2><a name="p-62870-tldr-1" class="anchor" href="https://ethresear.ch#p-62870-tldr-1" aria-label="Heading link"></a>TL;DR</h2>
<p>We run an OP Stack rollup on Ethereum mainnet (chain ID 42069000, live since 2026-09-30) where L2 transactions carry <strong>no signatures at all</strong>. An account is the tip of a keccak-256 hash chain. Spending reveals the next preimage. A commit–reveal step binds each preimage to one transaction before the prei