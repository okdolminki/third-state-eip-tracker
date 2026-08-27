---
source: "Ethereum Research"
source_type: research
title: "AMM Yield Maximization: Convergence of the Liquidity Provider and Arbitrageur Roles"
author: ""
pub_date: "Thu, 27 Aug 2026 10:32:59 +0000"

importance: medium
action: weekly_review
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-08-27
sources:
  - "https://ethresear.ch/t/amm-yield-maximization-convergence-of-the-liquidity-provider-and-arbitrageur-roles/25826"
---
# AMM Yield Maximization: Convergence of the Liquidity Provider and Arbitrageur Roles

> 출처: [Ethereum Research](https://ethresear.ch/t/amm-yield-maximization-convergence-of-the-liquidity-provider-and-arbitrageur-roles/25826)  |  Thu, 27 Aug 2026 10:32:59 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review

**요약:** DeFi 시장의 미시적 비효율성으로 발생하는 유동성 공급자 수수료 수익과 차익거래자 이익을 합산한 'dislocation value'를 측정하여 AMM 수익 극대화 방안을 연구하는 글입니다.

**리서치 앵글:** DEX 경쟁구도와 MEV 테마에 직접적으로 연관되며, AMM의 근본적인 수익 메커니즘과 차익거래의 역할을 이해하는 데 중요합니다.

## 원문 미리보기
<p><em>This essay is authored by the <a href="https://www.mev-x.com/" rel="noopener nofollow ugc">MEV-X</a> research team together with academic collaborators from HSE University.</em></p>
<h4><a name="p-62116-abstract-1" class="anchor" href="https://ethresear.ch#p-62116-abstract-1"></a>Abstract</h4>
<p>DeFi markets are efficient at the macro scale but constantly dislocated at the micro level: almost every swap moves a pool away from the market price and opens an arbitrage opportunity. We measure the <strong>dislocation value</strong> — the pool’s fee revenue plus the arbitrageur’s profit — an