---
source: "Ethereum Research"
source_type: research
title: "Substrate Incompleteness"
author: ""
pub_date: "Thu, 30 Jul 2026 01:15:09 +0000"

importance: medium
action: weekly_review
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-07-30
sources:
  - "https://ethresear.ch/t/substrate-incompleteness/25572"
---
# Substrate Incompleteness

> 출처: [Ethereum Research](https://ethresear.ch/t/substrate-incompleteness/25572)  |  Thu, 30 Jul 2026 01:15:09 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review

**요약:** 공정한 메커니즘을 구축하는 데 있어 끊임없이 발생하는 게임 패턴으로 인해 완벽한 설계가 어렵다는 'Substrate Incompleteness' 원칙을 다룬다.

**리서치 앵글:** MEV 및 DeFi 프로토콜의 경제적 보안 설계와 관련된 공정성 메커니즘의 한계점을 탐구한다.

## 원문 미리보기
<h1><a name="p-61602-substrate-incompleteness-1" class="anchor" href="https://ethresear.ch#p-61602-substrate-incompleteness-1"></a>Substrate Incompleteness</h1>
<p><strong>Status</strong>: Design humility principle with concrete walked-through surfaces.</p>
<hr>
<h2><a name="p-61602-a-humbling-observation-2" class="anchor" href="https://ethresear.ch#p-61602-a-humbling-observation-2"></a>A humbling observation</h2>
<p>You’re building a fairness mechanism. You work hard on it. You spot a gaming pattern and block it. Then you spot another. Then another.</p>
<p>Every mechanism you build catches so