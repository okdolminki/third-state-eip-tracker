---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8477: Recent Block Bound Delegation Authorizations"
author: ""
pub_date: "Tue, 03 Nov 2026 17:39:43 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-04
sources:
  - "https://ethereum-magicians.org/t/eip-8477-recent-block-bound-delegation-authorizations/30269"
---
# EIP-8477: Recent Block Bound Delegation Authorizations

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8477-recent-block-bound-delegation-authorizations/30269)  |  Tue, 03 Nov 2026 17:39:43 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8477은 EIP-7702 서명의 장기 저장 및 재사용을 방지하기 위해 최근 블록 정보를 포함하도록 위임 권한을 제한하는 제안입니다.

**리서치 앵글:** EIP-7702의 보안 취약점을 개선하여 계정 추상화의 안정적인 도입 및 활용에 기여합니다.

## 원문 미리보기
<p>Discussion topic for <a href="https://github.com/ethereum/EIPs/pull/12601" rel="noopener nofollow ugc">EIP-8477: Recent Block Bound Delegation Authorizations</a>.</p>
<p>Motivated by the recent EIP-7702 sweeps that happened on <a href="https://x.com/XBToshi/status/2115989338345619794" rel="noopener nofollow ugc">Binance 16</a> this proposal in essence prevents long term storage of EIP-7702 signatures for later playback.</p>
<p>This proposal limits the delayed use of unused EIP-7702 authorizations. Each authorization signs a recent execution block number and its block header hash, in additio