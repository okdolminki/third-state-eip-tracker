---
source: "Ethereum Research"
source_type: research
title: "Builders' Defection and Incentive Compatibility"
author: ""
pub_date: "Wed, 08 Jul 2026 11:22:20 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-08
sources:
  - "https://ethresear.ch/t/builders-defection-and-incentive-compatibility/25400"
---
# Builders' Defection and Incentive Compatibility

> 출처: [Ethereum Research](https://ethresear.ch/t/builders-defection-and-incentive-compatibility/25400)  |  Wed, 08 Jul 2026 11:22:20 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** PBS 환경에서 빌더는 서처의 입찰 정보를 활용해 수익성 있는 번들을 복제하여 경매 결과를 무시할 수 있는 불완전한 약속 문제를 야기한다.

**리서치 앵글:** MEV 테마와 직접적으로 연관되며, PBS 환경에서의 빌더 인센티브 및 블록 생산 메커니즘의 안정성에 대한 연구이다.

## 원문 미리보기
<p><code>team@nuconstruct.xyz</code></p>
<h2><a name="p-61174-tldr-1" class="anchor" href="https://ethresear.ch#p-61174-tldr-1"></a>TLDR</h2>
<ul>
<li>
<p>Under proposer-builder separation (PBS), a single builder observes every searcher’s bid and full payload before assembling the block, with no constraint on how it uses that information. It can therefore replicate a profitable bundle instead of honoring the auction it ran. This is an imperfect-commitment problem: the builder runs the auction but nothing binds it to the outcome it promised, summarized by a the share of opportunities on which i