---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "[Pre-ERC Discussion] Evolving SBT with Namespaced State Transitions"
author: ""
pub_date: "Thu, 12 Nov 2026 05:47:33 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-12
sources:
  - "https://ethereum-magicians.org/t/pre-erc-discussion-evolving-sbt-with-namespaced-state-transitions/30361"
---
# [Pre-ERC Discussion] Evolving SBT with Namespaced State Transitions

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/pre-erc-discussion-evolving-sbt-with-namespaced-state-transitions/30361)  |  Thu, 12 Nov 2026 05:47:33 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 과거 활동을 통해 검증된 경험을 축적하고 다양한 애플리케이션에서 활용할 수 있는 SBT 확장 방안에 대한 초기 논의.

**리서치 앵글:** 계정 추상화 및 기관 DeFi 도입을 위한 온체인 신원 및 평판 시스템 구축 가능성과 연관됨.

## 원문 미리보기
<p><em>This discussion is split across two posts because of the forum’s per-post character limit. This first post covers the core interface, growth, authority, and validity. The continuation below covers private presentations, one-time entitlements, recovery, the implementation example, and discussion questions.</em></p>
<p>I am exploring an extension for soulbound credentials that accumulate verified experiences over time and allow those experiences to support different applications.</p>
<p>The motivation is:</p>
<blockquote>
<p>Past activity scattered across different protocols should be reu