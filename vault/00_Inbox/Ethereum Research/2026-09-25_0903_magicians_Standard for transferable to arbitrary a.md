---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Standard for 'transferable to arbitrary addresses' on tokenized RWAs? (locked v4 pools quoted in tokenized stocks)"
author: ""
pub_date: "Thu, 24 Sep 2026 16:18:01 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-09-25
sources:
  - "https://ethereum-magicians.org/t/standard-for-transferable-to-arbitrary-addresses-on-tokenized-rwas-locked-v4-pools-quoted-in-tokenized-stocks/29769"
---
# Standard for "transferable to arbitrary addresses" on tokenized RWAs? (locked v4 pools quoted in tokenized stocks)

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/standard-for-transferable-to-arbitrary-addresses-on-tokenized-rwas-locked-v4-pools-quoted-in-tokenized-stocks/29769)  |  Thu, 24 Sep 2026 16:18:01 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 이더리움 매지션스에서 Uniswap v4와 Ondo 토큰화 주식을 활용하여 거래 수수료를 지급하는 RWA 기반 토큰 모델의 표준화 논의가 진행되고 있다.

**리서치 앵글:** RWA 테마와 Ondo 프로토콜의 토큰화된 주식을 활용한 새로운 DEX 수익 모델 및 표준화 가능성을 분석한다.

## 원문 미리보기
<p>Been looking at a launchpad on mainnet (sender.family) that does something I haven’t seen elsewhere and I’m not sure it’s safe.</p>
<p>Instead of a bonding curve + migration, it puts the whole supply into a single one-sided Uniswap v4 position and locks it forever. Fine, clanker/zora do similar on base. The new part: the quote asset can be anything on their allowlist, including Ondo tokenized stocks (NVDA, TSLA, AAPL). And the creator can route 70% of the swap fee to holders, paid in the stock token. So a coin whose holders earn tokenized nvidia from trading volume. It’s announced today, an