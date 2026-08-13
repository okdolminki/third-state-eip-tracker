---
source: "Ethereum Research"
source_type: research
title: "Designs for EVM gas accounting in EIP-7999"
author: ""
pub_date: "Wed, 12 Aug 2026 23:22:25 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-13
sources:
  - "https://ethresear.ch/t/designs-for-evm-gas-accounting-in-eip-7999/25696"
---
# Designs for EVM gas accounting in EIP-7999

> 출처: [Ethereum Research](https://ethresear.ch/t/designs-for-evm-gas-accounting-in-eip-7999/25696)  |  Wed, 12 Aug 2026 23:22:25 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-7999의 EVM 가스 회계 설계와 EIP-8037의 다차원 수수료 시장 도입을 통해 자원 소비를 정밀하게 제어하고 공정하게 가격을 책정하는 방안을 논의합니다.

**리서치 앵글:** EVM 가스 회계 및 다차원 수수료 시장 설계는 L2 확장성과 DeFi 프로토콜의 비용 효율성에 직접적인 영향을 미칩니다.

## 원문 미리보기
<h2><a name="p-61850-introduction-1" class="anchor" href="https://ethresear.ch#p-61850-introduction-1"></a>Introduction</h2>
<p>A multidimensional fee market enables precise control over resource consumption. It allows the market to fairly price resources according to targets and limits deemed safe by developers, and it allows resources to be consumed at maximum capacity within these limits. <a href="https://eips.ethereum.org/EIPS/eip-8037">EIP-8037</a> introduces state creation as a separately metered resource. Its resource-pricing design is kept simple so as not to delay Glamsterdam, but the