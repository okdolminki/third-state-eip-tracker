---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8310: Post-Quantum Keystore for Stateful Keys"
author: ""
pub_date: "Tue, 23 Jun 2026 18:19:06 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-24
sources:
  - "https://ethereum-magicians.org/t/eip-8310-post-quantum-keystore-for-stateful-keys/28853"
---
# EIP-8310: Post-Quantum Keystore for Stateful Keys

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8310-post-quantum-keystore-for-stateful-keys/28853)  |  Tue, 23 Jun 2026 18:19:06 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8310은 이더리움 합의 계층의 상태 기반 해시 서명 키(XMSS)를 위한 양자 내성 키스토어 형식을 정의하고, ERC-2335를 확장하여 소모성 키를 지원하는 핵심 제안이다.

**리서치 앵글:** 이더리움의 근본적인 양자 내성 보안 강화는 기관 DeFi 도입의 장기적인 신뢰도를 높이고, L2 및 계정 추상화의 기반 보안을 강화한다.

## 원문 미리보기
<p>This thread is for discussion of <strong>EIP-8310: Post-Quantum Keystore for Stateful Keys</strong>, a Standards Track (Core) proposal defining a keystore format for <strong>stateful hash-based signing keys</strong> — XMSS as used by the lean Ethereum consensus layer (referred to as <code>leanxmss</code>).</p>
<p>It extends <a href="https://eips.ethereum.org/EIPS/eip-2335" rel="noopener nofollow ugc">ERC-2335</a> so the encrypted secret may be an XMSS seed, and adds the machinery a <em>consumable</em> key requires.</p>
<ul>
<li><strong>Draft PR:</strong> <a href="https://github.com/ethereum