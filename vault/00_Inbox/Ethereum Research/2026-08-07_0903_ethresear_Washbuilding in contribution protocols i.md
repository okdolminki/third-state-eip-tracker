---
source: "Ethereum Research"
source_type: research
title: "Wash-building in contribution protocols is not a Sybil problem"
author: ""
pub_date: "Thu, 06 Aug 2026 16:27:20 +0000"

importance: medium
action: weekly_review
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-08-07
sources:
  - "https://ethresear.ch/t/wash-building-in-contribution-protocols-is-not-a-sybil-problem/25643"
---
# Wash-building in contribution protocols is not a Sybil problem

> 출처: [Ethereum Research](https://ethresear.ch/t/wash-building-in-contribution-protocols-is-not-a-sybil-problem/25643)  |  Thu, 06 Aug 2026 16:27:20 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review

**요약:** 기여 프로토콜에서 워시 빌딩은 시빌 문제가 아니며, 이 둘을 구분하는 것이 해결책을 더 어렵게 만든다는 내용의 연구.

**리서치 앵글:** 탈중앙화 거버넌스 및 펀딩 메커니즘의 공정성과 보안에 대한 연구로, DEX 경쟁 구도 및 L2 생태계의 지속 가능성에 간접적으로 영향을 미칠 수 있음.

## 원문 미리보기
<p>Wash-building is not a Sybil problem: an impossibility argument, and what a solution is then forced to look like</p>
<p>Contribution graphs (dependency graphs, quadratic funding, retro funding) face two attacks that are almost always conflated. Separating them makes one of them provably harder than most tooling assumes, and it also constrains the solution more than you would expect.</p>
<p><strong>Two axes.</strong> Sybil is fake identity: one actor wearing many masks. Wash is fake value: many genuinely distinct, real identities that build on each other’s worthless content and cross-endorse