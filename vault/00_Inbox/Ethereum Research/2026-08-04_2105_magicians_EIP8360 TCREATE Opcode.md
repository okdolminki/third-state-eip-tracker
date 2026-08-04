---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8360: TCREATE Opcode"
author: ""
pub_date: "Tue, 04 Aug 2026 00:31:05 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-04
sources:
  - "https://ethereum-magicians.org/t/eip-8360-tcreate-opcode/29258"
---
# EIP-8360: TCREATE Opcode

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8360-tcreate-opcode/29258)  |  Tue, 04 Aug 2026 00:31:05 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 이 EIP는 임시 계약 배포를 위한 공식적이고 가스 효율적인 TCREATE EVM opcode를 도입합니다.

**리서치 앵글:** 임시 계약을 통한 L2 확장성 개선 및 DeFi 프로토콜의 효율적인 설계 가능성 모색

## 원문 미리보기
<p>Discussion topic for <a href="https://github.com/ethereum/EIPs/pull/12073" rel="noopener nofollow ugc">EIP-8360</a></p>
<h2><a name="p-72564-abstract-1" class="anchor" href="https://ethereum-magicians.org#p-72564-abstract-1" aria-label="Heading link"></a>Abstract</h2>
<p>This EIP introduces a new EVM opcode, <code>TCREATE</code>, where <code>T</code> stands for transient, providing an official, gas-efficient, and state-aware mechanism for deploying temporary contracts.</p>
            <p><small>3 posts - 2 participants</small></p>
            <p><a href="https://ethereum-magicians.org/t/eip