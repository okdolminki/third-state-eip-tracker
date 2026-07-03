---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Proposing a family of candidate ERC interfaces for titled asset infrastructure — architecture review"
author: ""
pub_date: "Thu, 02 Jul 2026 19:56:31 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-03
sources:
  - "https://ethereum-magicians.org/t/proposing-a-family-of-candidate-erc-interfaces-for-titled-asset-infrastructure-architecture-review/28913"
---
# Proposing a family of candidate ERC interfaces for titled asset infrastructure — architecture review

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/proposing-a-family-of-candidate-erc-interfaces-for-titled-asset-infrastructure-architecture-review/28913)  |  Thu, 02 Jul 2026 19:56:31 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 기존 ERC 표준으로는 다루기 어려운 소유권 자산(titled-asset) 계층을 위한 6가지 새로운 ERC 인터페이스 후보군이 제안되었다.

**리서치 앵글:** RWA 테마와 관련하여 소유권 자산의 온체인 표현 및 규제 준수를 위한 새로운 ERC 표준 제안을 검토한다.

## 원문 미리보기
<p><strong>Thesis:</strong> No composition of existing ERC standards appears to cover the full titled-asset layer: structural asset-to-token binding, deterministic document-bundle commitments, directional transfer-domain rules, compliance event recording, impact snapshots with optional attestation, and standardised NAV reporting. We have split that layer into six candidate ERC interfaces. Each is designed to deploy and add value on its own; composition is optional, and the split itself is part of what we want feedback on.</p>
<p><em>See <strong>Materials</strong> below. Prior-art corrections a