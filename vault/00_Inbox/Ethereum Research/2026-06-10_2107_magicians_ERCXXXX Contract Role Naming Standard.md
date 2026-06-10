---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-XXXX: Contract Role Naming Standard"
author: ""
pub_date: "Wed, 10 Jun 2026 02:52:59 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-10
sources:
  - "https://ethereum-magicians.org/t/erc-xxxx-contract-role-naming-standard/28756"
---
# ERC-XXXX: Contract Role Naming Standard

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-xxxx-contract-role-naming-standard/28756)  |  Wed, 10 Jun 2026 02:52:59 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 스마트 계약 내 권한이 있는 역할을 계층적 네임스페이스 패턴인 'role.{category}.{action}'과 keccak256 해시 유도를 통해 표준화하여 일관된 역할 명명 및 검색을 지원하는 제안입니다.

**리서치 앵글:** Aave, Morpho 등 커버리지 프로토콜의 복잡한 권한 제어 구조를 표준화함으로써, 기관 DeFi 도입 시 보안 감사 및 다중서명 거버넌스 운영의 투명성과 상호운용성을 제고할 수 있습니다.

## 원문 미리보기
<h2><a name="p-70770-abstract-1" class="anchor" href="https://ethereum-magicians.org#p-70770-abstract-1" aria-label="Heading link"></a><strong>Abstract</strong></h2>
<p>This proposal defines a hierarchical namespace pattern for naming privileged roles in smart contracts, enabling consistent role naming across protocols with support for incremental adoption. The pattern <code>role.{category}.{action}</code> combined with <code>keccak256</code> hash derivation provides semantically clear and hash-discoverable standardized naming. A core role set applies conditionally based on contract functional