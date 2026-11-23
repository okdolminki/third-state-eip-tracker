---
source: "Ethereum Research"
source_type: research
title: "EthCLLib: a Lean 4 framework for the Ethereum consensus specs"
author: ""
pub_date: "Mon, 23 Nov 2026 11:17:01 +0000"

importance: high
action: read_now
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-11-23
sources:
  - "https://ethresear.ch/t/ethcllib-a-lean-4-framework-for-the-ethereum-consensus-specs/26283"
---
# EthCLLib: a Lean 4 framework for the Ethereum consensus specs

> 출처: [Ethereum Research](https://ethresear.ch/t/ethcllib-a-lean-4-framework-for-the-ethereum-consensus-specs/26283)  |  Mon, 23 Nov 2026 11:17:01 +0000

## AI 분석
**중요도:** high | **액션:** read_now

**요약:** 이더리움 합의 사양을 Lean 4로 구현하고 pyspec 벡터를 통과하는 EthCLLib 프레임워크에 대한 연구.

**리서치 앵글:** 이더리움 합의 레이어의 안정성과 검증 가능성을 높여 L2 확장성 및 기관 DeFi 도입의 기반을 강화.

## 원문 미리보기
<p>Thanks to <a class="mention" href="https://ethresear.ch/u/alexanderlhicks">@alexanderlhicks</a> for inspiring this post.</p>
<p>In the <a href="https://ethresear.ch/t/etheorem-update-the-complete-executable-consensus-specs-written-in-lean-4/26063">previous update</a> we showed the Etheorem consensus specs in Lean 4, Fulu, Gloas and Heze, passing the pyspec vectors. We write the three forks with one package, EthCLLib, which we started in June 2026. That post showed how the specs look. This one is about the framework under them: what it gives to the people who write a fork, what it gives to t