---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8445: Common Computational Gas Scaling Factor"
author: ""
pub_date: "Mon, 19 Oct 2026 04:26:09 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-19
sources:
  - "https://ethereum-magicians.org/t/eip-8445-common-computational-gas-scaling-factor/30002"
---
# EIP-8445: Common Computational Gas Scaling Factor

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8445-common-computational-gas-scaling-factor/30002)  |  Mon, 19 Oct 2026 04:26:09 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 이 EIP는 EVM 내 연산 오피코드의 가스 비용을 책정하는 공통 스케일링 팩터인 CPCU를 도입하여, 연산 작업의 상대적 가스 비용과 절대적 가스 가격을 분리하고 후자를 일괄적으로 조정할 수 있도록 합니다.

**리서치 앵글:** EVM 가스 비용 구조 변경은 L2 확장성 및 전반적인 DeFi 프로토콜의 경제성에 중대한 영향을 미칠 수 있습니다.

## 원문 미리보기
<p>Discussion topic for <a href="https://github.com/ethereum/EIPs/pull/12527" rel="noopener nofollow ugc">EIP-8445</a></p>
<h2><a name="p-75387-abstract-1" class="anchor" href="https://ethereum-magicians.org#p-75387-abstract-1" aria-label="Heading link"></a>Abstract</h2>
<p>This EIP introduces a common scaling factor, <code>CPCU</code> (cost per computational unit), for pricing computational opcodes in the Ethereum Virtual Machine (EVM). The factor decouples the relative gas costs of computational operations from their absolute gas prices, allowing the latter to be adjusted collectively at har