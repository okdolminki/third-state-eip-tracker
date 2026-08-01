---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8357: EVM Verification Key Registry"
author: ""
pub_date: "Fri, 31 Jul 2026 14:14:10 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-01
sources:
  - "https://ethereum-magicians.org/t/eip-8357-evm-verification-key-registry/29222"
---
# EIP-8357: EVM Verification Key Registry

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8357-evm-verification-key-registry/29222)  |  Fri, 31 Jul 2026 14:14:10 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8357은 L1 기능 포크별 EVM 검증 키를 포함하는 고정 주소 시스템 컨트랙트를 생성하여, 각 검증 키를 해당 포크의 활성화 타임스탬프에 매핑합니다.


## 원문 미리보기
<p>Discussion topic for <a href="https://github.com/ethereum/EIPs/pull/12055" rel="noopener nofollow ugc">EIP-8357</a>.</p>
<h2><a name="p-72447-abstract-1" class="anchor" href="https://ethereum-magicians.org#p-72447-abstract-1" aria-label="Heading link"></a><strong>Abstract</strong></h2>
<p>This EIP creates a fixed-address system contract containing the canonical EVM verification key for each registered L1 feature fork. Each entry maps one exact verification key to the activation timestamp of the fork-specific EVM program bound by that key.</p>
<p>The contract stores one <code>current_verific