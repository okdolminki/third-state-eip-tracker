---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8472: Stock Locates"
author: ""
pub_date: "Thu, 29 Oct 2026 15:07:09 +0000"

importance: medium
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-30
sources:
  - "https://ethereum-magicians.org/t/erc-8472-stock-locates/30128"
---
# ERC-8472: Stock Locates

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8472-stock-locates/30128)  |  Thu, 29 Oct 2026 15:07:09 +0000

## AI 분석
**중요도:** medium | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 토큰 대출 시장에서 특정 토큰의 대출 가능 여부, 수량, 이자율 등을 조회하는 표준 인터페이스인 ERC-8472 초안이 제안되었다.

**리서치 앵글:** DeFi 대출 시장의 표준화된 정보 조회를 통해 기관 DeFi 도입을 촉진하고, 커버리지 프로토콜(Aave, Morpho, Maple)의 상호운용성 및 효율성에 영향을 미칠 수 있다.

## 원문 미리보기
<p>Ask a lending venue whether, how much and at what rate a token can be borrowed now, and against what.</p>
<p>This is a draft ERC from Borro, a stock lending market on Robinhood Chain. It has no number yet; we will open the pull request to ethereum/ERCs with this thread as its <code>discussions-to</code>. The reference implementation is deployed and its source is verified: <a href="https://robinhoodchain.blockscout.com/address/0xd86522162EBFc75bc3f959174be878FeD09dFc1f?tab=contract" rel="noopener nofollow ugc">0xd86522162EBFc75bc3f959174be878FeD09dFc1f</a>. Feedback on the interface, units a