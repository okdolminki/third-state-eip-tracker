---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8369: VOPS Profiles for FOCIL Eligibility"
author: ""
pub_date: "Wed, 05 Aug 2026 18:23:53 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-06
sources:
  - "https://ethereum-magicians.org/t/eip-8369-vops-profiles-for-focil-eligibility/29298"
---
# EIP-8369: VOPS Profiles for FOCIL Eligibility

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8369-vops-profiles-for-focil-eligibility/29298)  |  Wed, 05 Aug 2026 18:23:53 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8369는 FOCIL(fork-choice enforced inclusion list) 적격성을 위한 두 가지 VOPS(validity-only partial statelessness) 프로필을 설명합니다.

**리서치 앵글:** 이더리움 프로토콜의 트랜잭션 처리 및 상태 관리 개선을 통해 L2 확장성 및 MEV에 미칠 잠재적 영향을 분석합니다.

## 원문 미리보기
<p>Discussion topic for <a href="https://github.com/ethereum/EIPs/pull/12110/" rel="noopener nofollow ugc">EIP-8369: VOPS Profiles for FOCIL Eligibility · Pull Request #12110 · ethereum/EIPs · GitHub</a></p>
<h2><a name="p-72709-abstract-1" class="anchor" href="https://ethereum-magicians.org#p-72709-abstract-1" aria-label="Heading link"></a>Abstract</h2>
<p>This EIP describes two validity-only partial statelessness (VOPS) profiles for fork-choice enforced inclusion list (FOCIL) eligibility. Profile 1 covers regular transactions, every non-frame type without blobs, and keeps <a>EIP-7805</a>’s e