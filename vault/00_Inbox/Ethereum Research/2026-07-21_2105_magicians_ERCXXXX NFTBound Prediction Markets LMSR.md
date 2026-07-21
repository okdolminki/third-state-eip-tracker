---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-XXXX: NFT-Bound Prediction Markets (LMSR pricing, on-chain state)"
author: ""
pub_date: "Tue, 21 Jul 2026 04:25:11 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-21
sources:
  - "https://ethereum-magicians.org/t/erc-xxxx-nft-bound-prediction-markets-lmsr-pricing-on-chain-state/29046"
---
# ERC-XXXX: NFT-Bound Prediction Markets (LMSR pricing, on-chain state)

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-xxxx-nft-bound-prediction-markets-lmsr-pricing-on-chain-state/29046)  |  Tue, 21 Jul 2026 04:25:11 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** NFT에 1:1로 바인딩되어 시장 상태가 온체인에 저장되고 NFT 자체로 기능하는 예측 시장 표준을 제안합니다.

**리서치 앵글:** 새로운 DeFi 금융 상품으로서 예측 시장의 구조 및 DEX 경쟁 구도에 미칠 영향

## 원문 미리보기
<p>Abstract</p>
<p>This proposes a standard for prediction markets bound one-to-one to NFTs. Each ERC-721 token represents ownership of a single binary (YES/NO) market. The market’s state — question text, current odds, pool balance, resolution status — is stored on-chain and rendered as the token’s tokenURI SVG, so the NFT is not a receipt for a market elsewhere; the NFT is the market.</p>
<p>Pricing uses an on-chain Logarithmic Market Scoring Rule (LMSR) with fixed liquidity parameter b, settled in native chain currency. Market owners set the question once per cycle, earn a per-trade fee for 