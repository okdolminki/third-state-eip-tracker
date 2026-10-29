---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Draft ERC: AI Dispute Resolution Framework (ADRF) — admitting, resolving and ruling on claims about bound objects within pre-committed authority"
author: ""
pub_date: "Wed, 28 Oct 2026 18:50:29 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-29
sources:
  - "https://ethereum-magicians.org/t/draft-erc-ai-dispute-resolution-framework-adrf-admitting-resolving-and-ruling-on-claims-about-bound-objects-within-pre-committed-authority/30121"
---
# Draft ERC: AI Dispute Resolution Framework (ADRF) — admitting, resolving and ruling on claims about bound objects within pre-committed authority

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/draft-erc-ai-dispute-resolution-framework-adrf-admitting-resolving-and-ruling-on-claims-about-bound-objects-within-pre-committed-authority/30121)  |  Wed, 28 Oct 2026 18:50:29 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** AI 시스템 및 서비스 관련 분쟁 발생 시, 참여자, 분쟁 대상, 해결 방식 등을 정의하는 분쟁 해결 프레임워크 ERC 초안입니다.

**리서치 앵글:** 기관 DeFi 도입 시 AI 기반 서비스 및 데이터 관련 분쟁 해결 표준화에 기여할 수 있습니다.

## 원문 미리보기
<p>This is a draft ERC for the step that the standards around AI systems, resources and services have been leaving to “the parties’ contract”: what happens when someone objects to a record. Participants may be people, organizations, agents or contracts; what a dispute is about (which model, service, output, dataset, evaluation or promise) and how it is resolved (verifier, evidence, human or AI-assisted judgment) are kept apart, and nothing requires that AI be judged by AI or that a party be an agent.</p>
<p><strong>The claim is the object.</strong> A dispute is a specific claim about a specifi