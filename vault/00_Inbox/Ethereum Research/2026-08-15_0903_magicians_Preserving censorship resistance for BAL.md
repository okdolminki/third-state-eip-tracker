---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Preserving censorship resistance for BAL data in EIP-7999"
author: ""
pub_date: "Fri, 14 Aug 2026 13:05:41 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-15
sources:
  - "https://ethereum-magicians.org/t/preserving-censorship-resistance-for-bal-data-in-eip-7999/29427"
---
# Preserving censorship resistance for BAL data in EIP-7999

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/preserving-censorship-resistance-for-bal-data-in-eip-7999/29427)  |  Fri, 14 Aug 2026 13:05:41 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-7999는 데이터와 EVM 실행 가스를 분리하고 EIP-8279와 통합되어 데이터 자원을 무조건적으로 처리함으로써, 포함 목록(IL) 트랜잭션의 검열 저항성을 보존하는 방안을 논의합니다.

**리서치 앵글:** 이 EIP는 블록 빌딩 및 데이터 처리 방식의 변화를 통해 MEV와 L2 확장성에 미치는 영향을 분석하는 데 중요합니다.

## 원문 미리보기
<p><a href="https://eips.ethereum.org/EIPS/eip-7999">EIP-7999</a> separates data from EVM execution gas and treats data as an unconditional resource under <a href="https://eips.ethereum.org/EIPS/eip-7805">FOCIL</a>: a builder may not omit an inclusion-list transaction merely because the block’s data resource is full. This works because each IL is limited to 8 KiB of serialized transactions. <a href="https://eips.ethereum.org/EIPS/eip-8279">EIP-8279</a>, which can be <a href="https://github.com/ethereum/EIPs/pull/11835/changes">incorporated</a> in EIP-7999, specifies a single data resource cons