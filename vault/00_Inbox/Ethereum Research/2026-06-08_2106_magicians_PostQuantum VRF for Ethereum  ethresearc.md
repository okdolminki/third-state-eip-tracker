---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Post-Quantum VRF for Ethereum - ethresear.ch cross post"
author: ""
pub_date: "Mon, 08 Jun 2026 10:08:06 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-08
sources:
  - "https://ethereum-magicians.org/t/post-quantum-vrf-for-ethereum-ethresear-ch-cross-post/28743"
---
# Post-Quantum VRF for Ethereum - ethresear.ch cross post

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/post-quantum-vrf-for-ethereum-ethresear-ch-cross-post/28743)  |  Mon, 08 Jun 2026 10:08:06 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** L* 마일스톤에서 BLS 키 폐기로 인해 현재 RANDAO 메커니즘이 완전히 실패할 위험이 있어, 양자 저항성을 갖춘 해시 기반 VRF 수정안이 I*에서 활성화되도록 제안되었습니다.

**리서치 앵글:** 이더리움 핵심 프로토콜의 무작위성(RANDAO) 및 양자 저항성 강화는 LST/LRT 구조, MEV, L2 확장성 등 모든 DeFi 테마의 근간이 되는 L1 보안 및 안정성에 직접적인 영향을 미칩니다.

## 원문 미리보기
<h2><a name="p-70698-tldr-1" class="anchor" href="https://ethereum-magicians.org#p-70698-tldr-1" aria-label="Heading link"></a>TL;DR</h2>
<p>At the L* milestone, BLS keys are retired. The current <code>randao_reveal</code> mechanism fails entirely. This post proposes the minimal, hash-based fix: a PRF-commitment VRF derived from the leanSig seed, proved with a standalone WHIR proof included in the <code>BeaconBlockBody</code>. The construction activates at I*, so RANDAO gains quantum resistance before L* rather than at it.</p>
<p>A reference implementation is at <a href="https://github.com/ary