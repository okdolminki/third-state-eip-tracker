---
source: "Ethereum Research"
source_type: research
title: "Native Randomness Sourcing with Looser Guarantees"
author: ""
pub_date: "Tue, 28 Jul 2026 16:05:16 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-29
sources:
  - "https://ethresear.ch/t/native-randomness-sourcing-with-looser-guarantees/25556"
---
# Native Randomness Sourcing with Looser Guarantees

> 출처: [Ethereum Research](https://ethresear.ch/t/native-randomness-sourcing-with-looser-guarantees/25556)  |  Tue, 28 Jul 2026 16:05:16 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 이더리움 온체인 게임을 위한 네이티브 난수 생성 방식을 다루며, 사용자 경험을 위해 빠른 처리 시간(1-2 블록)을 우선시하는 난수 보장 완화 방안을 탐구한다.

**리서치 앵글:** DeFi 프로토콜이 MEV 완화 및 공정한 온체인 메커니즘 설계를 위해 난수를 활용할 때, 온체인 난수 생성 방식과 보장 수준에 대한 이해가 필요하다.

## 원문 미리보기
<h2><a name="p-61565-background-1" class="anchor" href="https://ethresear.ch#p-61565-background-1"></a>Background</h2>
<p>Asphodel’s Prologue is an onchain game on Ethereum. One with state logic actually processed end-to-end onchain. It demands randomness sourcing throughout its core flows, as most modern game flows centered around PvP mechanics do. These systems also require a turnaround time of 1-2 blocks rather than whole epochs for the sake of UX, so the question of economic security is one that’s reasoned about on a Pareto front.</p>
<p>I won’t go too deep into the game itself to keep the