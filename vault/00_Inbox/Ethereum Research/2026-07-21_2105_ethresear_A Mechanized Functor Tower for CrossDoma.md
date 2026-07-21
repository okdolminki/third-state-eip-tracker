---
source: "Ethereum Research"
source_type: research
title: "A Mechanized Functor Tower for Cross-Domain State Preservation"
author: ""
pub_date: "Tue, 21 Jul 2026 10:36:52 +0000"

importance: medium
action: weekly_review
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-07-21
sources:
  - "https://ethresear.ch/t/a-mechanized-functor-tower-for-cross-domain-state-preservation/25491"
---
# A Mechanized Functor Tower for Cross-Domain State Preservation

> 출처: [Ethereum Research](https://ethresear.ch/t/a-mechanized-functor-tower-for-cross-domain-state-preservation/25491)  |  Tue, 21 Jul 2026 10:36:52 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review

**요약:** 이더리움 리서치 포스트는 크로스-도메인 상태 보존을 위한 재사용 가능한 검증 기반을 제공하며, 브릿지 및 롤업 출구와 같은 시스템에 적용 가능한 기계 검증된 정리를 제시합니다.

**리서치 앵글:** L2 확장성 및 크로스-체인 브릿지의 상태 보존 및 검증 기반 연구와 연관됩니다.

## 원문 미리보기
<p>This post adds two machine-checked results to <strong>a reusable verification basis for cross-domain state</strong>. State-preserving maps between synchronization domains are closed under identity and composition, with associative composition, all as mechanized theorems. And coupling breadth forms a stratified tower of functors in which forgetting a coupled chain is a natural transformation. The mechanization is a set of generic Isabelle/HOL locales over arbitrary state machines, so the laws are directly reusable by any domain that discharges the locale obligations: a bridge, a rollup exit,