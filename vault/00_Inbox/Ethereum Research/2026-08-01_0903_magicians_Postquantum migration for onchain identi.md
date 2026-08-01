---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Post-quantum migration for on-chain identity: an anchored key-binding + a cutoff, verified by recompute (not a second signature)"
author: ""
pub_date: "Fri, 31 Jul 2026 22:52:13 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-01
sources:
  - "https://ethereum-magicians.org/t/post-quantum-migration-for-on-chain-identity-an-anchored-key-binding-a-cutoff-verified-by-recompute-not-a-second-signature/29225"
---
# Post-quantum migration for on-chain identity: an anchored key-binding + a cutoff, verified by recompute (not a second signature)

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/post-quantum-migration-for-on-chain-identity-an-anchored-key-binding-a-cutoff-verified-by-recompute-not-a-second-signature/29225)  |  Fri, 31 Jul 2026 22:52:13 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 온체인 신원/에이전트의 서명 계층을 양자 내성으로 마이그레이션하는 문제에 대한 접근 방식을 공유하며, 재계산을 통해 신뢰 대신 검증하는 방식을 제안합니다.

**리서치 앵글:** 계정 추상화(EIP-7702)의 장기적인 보안 및 온체인 신원 시스템의 양자 내성 확보와 관련됩니다.

## 원문 미리보기
<p>Sharing an approach we’ve been building and would like scrutiny on. It’s aimed at the narrow but real problem of migrating the <strong>signature layer</strong> of on-chain / agent identity to post-quantum, and it leans on recomputation rather than trust.</p>
<p><strong>The problem.</strong> Shor breaks the ECDSA/Schnorr signatures under most of Web3 and most AI-attestation identity. Hashes survive (Grover only halves them). The usual reflex “add a post-quantum signature alongside the classical one” doesn’t actually close it: a forger who derives the classical key just <em>omits</em> the ext