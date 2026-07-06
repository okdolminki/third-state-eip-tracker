---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Subject-Linked NAV Snapshot Oracle - candidate ERC"
author: ""
pub_date: "Sun, 05 Jul 2026 21:34:51 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-06
sources:
  - "https://ethereum-magicians.org/t/subject-linked-nav-snapshot-oracle-candidate-erc/28939"
---
# Subject-Linked NAV Snapshot Oracle - candidate ERC

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/subject-linked-nav-snapshot-oracle-candidate-erc/28939)  |  Sun, 05 Jul 2026 21:34:51 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 제공자 귀속(provider-attributed) 유동성 낮은 자산의 NAV 스냅샷을 게시하고 조회하는 오라클을 위한 ERC 후보에 대한 피드백 요청.

**리서치 앵글:** RWA 자산의 온체인 가치 평가 및 오라클 인프라 구축에 필수적인 요소로, Third State의 RWA 리서치 테마와 직접적으로 연관됩니다.

## 원문 미리보기
<p>We would like feedback on a candidate ERC for publishing and querying provider-attributed Net Asset Value snapshots for application-defined subjects.</p>
<p>Periodic NAV for funds, private credit, real estate, infrastructure, commodities, and other illiquid or administratively priced assets differs from a continuous market-price feed. A consumer needs to know what the value represents, its denomination, when the valuation was measured, when it was published, who supplied it, which methodology was used, and whether either time is too old for the intended use.</p>
<p>Each stream is keyed by <