---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Canonical Document Bundle Anchor - candidate ERC"
author: ""
pub_date: "Sun, 05 Jul 2026 21:30:30 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-06
sources:
  - "https://ethereum-magicians.org/t/canonical-document-bundle-anchor-candidate-erc/28935"
---
# Canonical Document Bundle Anchor - candidate ERC

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/canonical-document-bundle-anchor-candidate-erc/28935)  |  Sun, 05 Jul 2026 21:30:30 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 오프체인 문서 묶음에 대한 결정론적 커밋먼트를 도출하고 앵커링하기 위한 ERC 후보에 대한 피드백 요청으로, 문서 번들 상호운용성을 위한 표준화된 접근 방식을 제안합니다.

**리서치 앵글:** RWA 및 기관 DeFi 도입 시 오프체인 문서의 온체인 연동 및 상호운용성 표준화에 기여할 수 있습니다.

## 원문 미리보기
<p>We would like feedback on a candidate ERC for deriving and anchoring a deterministic commitment to a bundle of off-chain documents.</p>
<p>Applications frequently commit to agreements, certifications, evidence, amendments, and supporting records. Hashing each file is not enough to make a bundle interoperable: implementations can still disagree about entry fields, ordering, normalization identifiers, version separation, duplicate handling, and replacement history.</p>
<p>The proposal separates two layers:</p>
<ol>
<li>A normalization profile transforms a raw document into canonical bytes.</l