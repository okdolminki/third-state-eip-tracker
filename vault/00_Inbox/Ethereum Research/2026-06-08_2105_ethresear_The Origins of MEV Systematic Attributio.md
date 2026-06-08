---
source: "Ethereum Research"
source_type: research
title: "The Origins of MEV: Systematic Attribution of Arbitrage Opportunity Creation at Scale"
author: ""
pub_date: "Mon, 08 Jun 2026 11:26:18 +0000"

importance: high
action: read_now
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-06-08
sources:
  - "https://ethresear.ch/t/the-origins-of-mev-systematic-attribution-of-arbitrage-opportunity-creation-at-scale/25124"
---
# The Origins of MEV: Systematic Attribution of Arbitrage Opportunity Creation at Scale

> 출처: [Ethereum Research](https://ethresear.ch/t/the-origins-of-mev-systematic-attribution-of-arbitrage-opportunity-creation-at-scale/25124)  |  Mon, 08 Jun 2026 11:26:18 +0000

## AI 분석
**중요도:** high | **액션:** read_now

**요약:** 이 논문은 MEV 기회 귀속 문제를 공식화하고, 특정 차익 거래 이익을 가능하게 한 선행 거래를 식별하기 위한 네 가지 귀속 방법을 설계 및 평가한다.

**리서치 앵글:** MEV의 근원을 체계적으로 분석하여 DEX 경쟁 구도 및 L2 확장성 맥락에서 MEV의 영향을 이해하는 데 기여한다.

## 원문 미리보기
<p><em>This paper is authored by the <a href="https://www.mev-x.com/" rel="noopener nofollow ugc">MEV-X</a> research team together with academic collaborators from MIPT, HSE University, and Skoltech.</em></p>
<p>This paper formalizes the MEV opportunity attribution problem: given an executed atomic arbitrage transaction <span class="math">T_{arb}</span> that extracts profit <span class="math">\Pi</span>, which preceding transaction created the price disbalance enabling that profit? We design and evaluate four attribution methods (bot-data-driven, simulation-based, coefficient-based, and Shaple