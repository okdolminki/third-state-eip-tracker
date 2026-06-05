---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "[Post-Quantum ERC-4337] WOTS-39: Winternitz One Time Signature Wallet For Ethereum"
author: ""
pub_date: "Fri, 05 Jun 2026 04:50:52 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-05
sources:
  - "https://ethereum-magicians.org/t/post-quantum-erc-4337-wots-39-winternitz-one-time-signature-wallet-for-ethereum/28715"
---
# [Post-Quantum ERC-4337] WOTS-39: Winternitz One Time Signature Wallet For Ethereum

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/post-quantum-erc-4337-wots-39-winternitz-one-time-signature-wallet-for-ethereum/28715)  |  Fri, 05 Jun 2026 04:50:52 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 양자 컴퓨터 위협에 대비하여 ERC-4337 지갑에 적용할 수 있는 WOTS-39 기반의 양자 내성 서명 방안을 제안하는 글.

**리서치 앵글:** 계정 추상화(ERC-4337)의 장기적인 보안 강화를 위한 양자 내성 서명 기술 도입 가능성 분석.

## 원문 미리보기
<p><strong>WOTS-39: A Live Post-Quantum Signature Wallet Across Bitcoin and Ethereum</strong></p>
<hr>
<p><strong>The Core Problem</strong></p>
<p>Every signature scheme securing crypto today (ECDSA, Schnorr, Ed25519) derives its security from the hardness of the elliptic curve discrete logarithm problem. Shor’s algorithm solves that in polynomial time on a sufficiently powerful quantum computer. This is not a theoretical future concern: NIST finalized its first post-quantum standards in 2024 precisely because the timeline is real. Every address that has ever broadcast a transaction has an exp