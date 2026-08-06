---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8368: CPSB Recalibration for New Gas Limit"
author: ""
pub_date: "Wed, 05 Aug 2026 16:19:43 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-06
sources:
  - "https://ethereum-magicians.org/t/eip-8368-cpsb-recalibration-for-new-gas-limit/29293"
---
# EIP-8368: CPSB Recalibration for New Gas Limit

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8368-cpsb-recalibration-for-new-gas-limit/29293)  |  Wed, 05 Aug 2026 16:19:43 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8368은 EIP-8037에서 도입된 상태 바이트당 가스 비용(CPSB)을 새로운 블록 가스 한도에 맞춰 재조정하는 것을 제안합니다.

**리서치 앵글:** 이 EIP는 이더리움의 핵심 가스 비용 구조를 변경하여 L2 확장성 및 전반적인 DeFi 프로토콜의 비용 효율성에 직접적인 영향을 미칩니다.

## 원문 미리보기
<p>Discussion topic for EIP-8368</p>
<h4><a name="p-72689-abstract-1" class="anchor" href="https://ethereum-magicians.org#p-72689-abstract-1" aria-label="Heading link"></a>Abstract</h4>
<p>This proposal updates `CPSB` (cost per state byte), the unit gas cost per new state byte introduced in EIP-8037, by re-deriving it for a new reference block gas limit. All other parameters, mechanisms, and semantics defined in EIP-8037 are unaffected and remain unchanged.</p>
            <p><small>1 post - 1 participant</small></p>
            <p><a href="https://ethereum-magicians.org/t/eip-8368-cpsb-recali