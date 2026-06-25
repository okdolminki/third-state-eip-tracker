---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-XXXX: Scope Contestation Registry — permissionless observation-scope completeness contestability"
author: ""
pub_date: "Wed, 24 Jun 2026 13:18:28 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-25
sources:
  - "https://ethereum-magicians.org/t/erc-xxxx-scope-contestation-registry-permissionless-observation-scope-completeness-contestability/28856"
---
# ERC-XXXX: Scope Contestation Registry — permissionless observation-scope completeness contestability

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-xxxx-scope-contestation-registry-permissionless-observation-scope-completeness-contestability/28856)  |  Wed, 24 Jun 2026 13:18:28 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 이 표준은 행위자가 관찰한 데이터 범위의 완전성을 온체인에서 증명하여 이의를 제기할 수 있는 허가 없는 레지스트리 인터페이스를 정의합니다.

**리서치 앵글:** L2 확장성 및 데이터 무결성 검증 메커니즘과 관련하여 사기 증명 및 데이터 가용성 문제 해결에 기여할 수 있습니다.

## 원문 미리보기
<h2><a name="p-71326-abstract-1" class="anchor" href="https://ethereum-magicians.org#p-71326-abstract-1" aria-label="Heading link"></a>Abstract</h2>
<p>This standard defines an interface for a <em>scope contestation registry</em>: a<br>
permissionless mechanism by which an actor commits the set of coordinates it<br>
observed (its <strong>observation scope</strong>), bound to an external commitment, and any<br>
party may prove on-chain that a specific coordinate was <strong>absent</strong> from that<br>
committed set. The registry records such proofs permanently and recomputably. It<br>
<strong