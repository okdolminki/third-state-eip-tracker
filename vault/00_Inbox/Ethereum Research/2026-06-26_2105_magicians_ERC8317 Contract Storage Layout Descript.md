---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8317: Contract Storage Layout Descriptor Format"
author: ""
pub_date: "Fri, 26 Jun 2026 09:42:20 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-26
sources:
  - "https://ethereum-magicians.org/t/erc-8317-contract-storage-layout-descriptor-format/28864"
---
# ERC-8317: Contract Storage Layout Descriptor Format

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8317-contract-storage-layout-descriptor-format/28864)  |  Fri, 26 Jun 2026 09:42:20 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 이 ERC는 EVM 컨트랙트의 저장소 레이아웃 메타데이터를 JSON 형식으로 표준화하여 하드웨어 지갑의 트랜잭션 시뮬레이션 및 명확한 서명 기능을 개선하는 것을 목표로 합니다.

**리서치 앵글:** 표준화된 저장소 레이아웃을 통한 트랜잭션 투명성 및 보안 강화는 기관 DeFi 도입에 필수적입니다.

## 원문 미리보기
<p>This ERC is an attempt to standardize the description of any EVM contract’s storage layout metadata using a JSON format, to be used with transaction simulation and transaction assertion features by the hardware wallets that implement Clear Signing (<a href="https://ethereum-magicians.org/t/eip-7730-proposal-for-a-clear-signing-standard-format-for-wallets/20403">ERC-7730</a>).</p>
<p>Knowing the storage layout of the contract being interacted with allows the hardware wallet to trace a transaction locally and display information like:<br>
<code>"This transaction sets USDC::balanceOf[vitalik.e