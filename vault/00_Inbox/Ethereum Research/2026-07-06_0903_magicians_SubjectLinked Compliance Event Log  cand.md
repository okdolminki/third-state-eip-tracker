---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Subject-Linked Compliance Event Log - candidate ERC"
author: ""
pub_date: "Sun, 05 Jul 2026 21:33:00 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-06
sources:
  - "https://ethereum-magicians.org/t/subject-linked-compliance-event-log-candidate-erc/28937"
---
# Subject-Linked Compliance Event Log - candidate ERC

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/subject-linked-compliance-event-log-candidate-erc/28937)  |  Sun, 05 Jul 2026 21:33:00 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 기존 토큰 및 컴플라이언스 표준의 한계를 극복하고, 온체인 컴플라이언스 이벤트 기록을 표준화하기 위한 ERC 후보 제안.

**리서치 앵글:** RWA 및 기관 DeFi 도입을 위한 온체인 컴플라이언스 기록 표준화 방안 연구에 활용.

## 원문 미리보기
<p>We would like feedback on a candidate ERC for append-only, subject-linked compliance-event records with attribution, evidence commitments, typed parties, versioned payloads, indexing, and correction provenance.</p>
<p>Existing token and compliance standards primarily define behavior: transfer eligibility, holder identity, freezes, forced transfers, and other lifecycle operations. Applications still represent the resulting records through custom events, token-local state, generic attestations, or off-chain databases. That makes it difficult for contracts, indexers, auditors, and reporting sy