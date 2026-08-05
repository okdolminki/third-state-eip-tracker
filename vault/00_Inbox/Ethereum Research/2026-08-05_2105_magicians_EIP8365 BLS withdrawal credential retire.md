---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8365: BLS withdrawal credential retirement"
author: ""
pub_date: "Wed, 05 Aug 2026 07:24:31 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-05
sources:
  - "https://ethereum-magicians.org/t/eip-8365-bls-withdrawal-credential-retirement/29284"
---
# EIP-8365: BLS withdrawal credential retirement

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8365-bls-withdrawal-credential-retirement/29284)  |  Wed, 05 Aug 2026 07:24:31 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8365는 0x00 (BLS) 인출 자격 증명 유형을 폐지하고, 기존 BLS 검증자를 제한된 속도로 종료하며, 새로운 BLS 검증자 예치를 중단하지만, `BLSToExecutionChange`를 통해 잔액 회수를 보장한다.

**리서치 앵글:** 이 EIP는 이더리움의 스테이킹 메커니즘 변경을 통해 LST/LRT 구조의 안정성과 진화를 간접적으로 연구하는 데 연관된다.

## 원문 미리보기
<p>Discussion topic for EIP-8365: <a href="https://github.com/ethereum/EIPs/pull/12097" class="inline-onebox" rel="noopener nofollow ugc">Add EIP: BLS withdrawal credential retirement by ensi321 · Pull Request #12097 · ethereum/EIPs · GitHub</a></p>
<p>This proposal retires the <code>0x00</code> (BLS) withdrawal credential type: active <code>0x00</code> validators are exited at a capped rate per epoch, and deposits creating new <code>0x00</code> validators are no longer processed. <code>BLSToExecutionChange</code> stays open, so a retired validator’s full balance remains recoverable at any tim