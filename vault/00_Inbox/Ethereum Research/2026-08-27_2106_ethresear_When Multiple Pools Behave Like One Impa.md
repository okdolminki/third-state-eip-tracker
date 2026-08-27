---
source: "Ethereum Research"
source_type: research
title: "When Multiple Pools Behave Like One: Impact-Constrained Capacity Concentration in Uniswap v3"
author: ""
pub_date: "Thu, 27 Aug 2026 01:32:59 +0000"

importance: high
action: read_now
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-08-27
sources:
  - "https://ethresear.ch/t/when-multiple-pools-behave-like-one-impact-constrained-capacity-concentration-in-uniswap-v3/25823"
---
# When Multiple Pools Behave Like One: Impact-Constrained Capacity Concentration in Uniswap v3

> 출처: [Ethereum Research](https://ethresear.ch/t/when-multiple-pools-behave-like-one-impact-constrained-capacity-concentration-in-uniswap-v3/25823)  |  Thu, 27 Aug 2026 01:32:59 +0000

## AI 분석
**중요도:** high | **액션:** read_now

**요약:** 유니스왑 v3에서 여러 풀이 존재하더라도, 실제 유동성 공급은 극히 소수의 풀에 집중되어 사실상 하나의 풀처럼 작동함을 분석.

**리서치 앵글:** 유니스왑 v3의 유동성 집중 현상 분석을 통해 DEX 경쟁구도 및 효율성 연구에 기여.

## 원문 미리보기
<h3><a name="p-62112-tldr-1" class="anchor" href="https://ethresear.ch#p-62112-tldr-1"></a>TL;DR</h3>
<ul>
<li><strong>293,273</strong> reconstructed <code>family × day × direction × impact_bps</code> cells across <strong>78</strong> Ethereum Uniswap v3 token–quote families.</li>
<li><strong>Nominal multiplicity <span class="math">\neq</span> diffuse effective capacity</strong>: The <strong>cell-weighted</strong> median capacity-effective pool count is <strong>1.076</strong> (<span class="math">N_{\mathrm{eff}}=1/\mathrm{HHI}</span>), with a median top-1 capacity share of <strong>96.3%</strong