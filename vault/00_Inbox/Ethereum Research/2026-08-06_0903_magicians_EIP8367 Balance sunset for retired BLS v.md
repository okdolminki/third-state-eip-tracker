---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8367: Balance sunset for retired BLS validators"
author: ""
pub_date: "Wed, 05 Aug 2026 18:52:20 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-06
sources:
  - "https://ethereum-magicians.org/t/eip-8367-balance-sunset-for-retired-bls-validators/29299"
---
# EIP-8367: Balance sunset for retired BLS validators

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8367-balance-sunset-for-retired-bls-validators/29299)  |  Wed, 05 Aug 2026 18:52:20 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8367은 EIP-8365에 따라 직무에서 은퇴하고 잔액이 동결된 0x00 BLS 검증자들의 잔액을 최종적으로 처리하는 방안을 논의합니다.

**리서치 앵글:** 이더리움 검증자 메커니즘 변경이 LST/LRT 프로토콜의 운영 및 유동성 관리에 미칠 영향을 분석합니다.

## 원문 미리보기
<p>Discussion topic for EIP-8367: <a href="https://github.com/ethereum/EIPs/pull/12099" class="inline-onebox" rel="noopener nofollow ugc">Add EIP: Balance sunset for retired BLS validators by ensi321 · Pull Request #12099 · ethereum/EIPs · GitHub</a></p>
<p>Companion to EIP-8365 ( <a href="https://ethereum-magicians.org/t/eip-8365-bls-withdrawal-credential-retirement/29284" class="inline-onebox">EIP-8365: BLS withdrawal credential retirement</a> ). Where 8365 retires <code>0x00</code> validators from duties and freezes their balances, this EIP proposes the second stage: each retired <code>0x00