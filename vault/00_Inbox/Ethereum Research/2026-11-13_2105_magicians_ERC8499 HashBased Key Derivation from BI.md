---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8499: Hash-Based Key Derivation from BIP-39"
author: ""
pub_date: "Fri, 13 Nov 2026 10:34:58 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-13
sources:
  - "https://ethereum-magicians.org/t/erc-8499-hash-based-key-derivation-from-bip-39/30375"
---
# ERC-8499: Hash-Based Key Derivation from BIP-39

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8499-hash-based-key-derivation-from-bip-39/30375)  |  Fri, 13 Nov 2026 10:34:58 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** BIP-39 니모닉 구문에서 해시 기반 양자 내성 키를 파생하는 방법에 대한 ERC 초안에 대한 피드백 요청.

**리서치 앵글:** 계정 추상화(EIP-7702)의 미래 보안 및 키 관리 방식에 대한 잠재적 영향.

## 원문 미리보기
<p>I’d like feedback on a draft ERC that says how a wallet derives hash-based post-quantum keys (leanSPHINCS, SLH-DSA, WOTS, FORS, XMSS) from a BIP-39 phrase.</p>
<p>Draft: <a href="https://github.com/ethereum/ERCs/pull/2172" class="inline-onebox" rel="noopener nofollow ugc">Add ERC: Hash-Based Key Derivation from BIP-39 by johba37 · Pull Request #2172 · ethereum/ERCs · GitHub</a></p>
<h2><a name="p-76573-why-1" class="anchor" href="https://ethereum-magicians.org#p-76573-why-1" aria-label="Heading link"></a>Why</h2>
<p>Contracts already verify hash-based signatures through ERC-1271 and account