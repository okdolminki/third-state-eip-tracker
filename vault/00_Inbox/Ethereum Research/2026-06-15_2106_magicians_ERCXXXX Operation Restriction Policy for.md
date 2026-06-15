---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-XXXX: Operation Restriction Policy for Tiered Permissions"
author: ""
pub_date: "Mon, 15 Jun 2026 06:19:07 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-15
sources:
  - "https://ethereum-magicians.org/t/erc-xxxx-operation-restriction-policy-for-tiered-permissions/28793"
---
# ERC-XXXX: Operation Restriction Policy for Tiered Permissions

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-xxxx-operation-restriction-policy-for-tiered-permissions/28793)  |  Mon, 15 Jun 2026 06:19:07 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 스마트 계약 내에서 계층화된 작업 제한 정책을 표준화하여, 기존의 신원 기반 권한 관리를 보완하고 세분화된 접근 제어를 가능하게 하는 제안입니다.

**리서치 앵글:** 기관용 DeFi(RWA, Maple, Ondo) 도입에 필수적인 세분화된 권한 제어 및 계정 추상화(EIP-7702) 환경에서의 정교한 보안 정책 수립과의 연관성을 분석할 수 있습니다.

## 원문 미리보기
<h2><a name="p-71044-abstract-1" class="anchor" href="https://ethereum-magicians.org#p-71044-abstract-1" aria-label="Heading link"></a><strong>Abstract</strong></h2>
<p>This proposal defines a standardized interface for tiered operation restriction policies in smart contracts. The existing EIP ecosystem has a fundamental asymmetry: multiple standards address identity-based permissions (“who can act”), including ERC-5982 (role-based access control), ERC-6366 (permission tokens), ERC-7820 (access control registries), and ERC-8063 (group-member tokens); as well as verification infrastructure (“ho