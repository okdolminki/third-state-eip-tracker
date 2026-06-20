---
source: "Ethereum Research"
source_type: research
title: "Futarchy is insecure without a proposal gatekeeper"
author: ""
pub_date: "Fri, 19 Jun 2026 13:02:06 +0000"

importance: medium
action: weekly_review
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-06-20
sources:
  - "https://ethresear.ch/t/futarchy-is-insecure-without-a-proposal-gatekeeper/25235"
---
# Futarchy is insecure without a proposal gatekeeper

> 출처: [Ethereum Research](https://ethresear.ch/t/futarchy-is-insecure-without-a-proposal-gatekeeper/25235)  |  Fri, 19 Jun 2026 13:02:06 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review

**요약:** 자산 푸타키는 전략적 행동으로 인해 조건부 가격이 조작될 수 있어 제안의 실제 가치를 반영하지 못하므로, 제안 게이트키퍼 없이는 안전하지 않다.


## 원문 미리보기
<p>Asset futarchy is attractive because it lets markets compare a proposal’s expected effect on token value. That comparison is only reliable when conditional prices track the proposal’s causal effect rather than strategic behavior around the decision rule.</p>
<p>The attacks below describe ways a proposer can make PASS-ASSET trade above FAIL-ASSET without creating commensurate value for ASSET holders. They are defensive mechanism-design examples: each one identifies a coupling failure between the conditional market price and the proposal’s true expected effect.</p>
<p>The mitigations also imp