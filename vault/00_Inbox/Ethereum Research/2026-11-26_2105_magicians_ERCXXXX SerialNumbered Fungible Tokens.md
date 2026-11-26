---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-XXXX: Serial-Numbered Fungible Tokens"
author: ""
pub_date: "Thu, 26 Nov 2026 03:00:53 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-26
sources:
  - "https://ethereum-magicians.org/t/erc-xxxx-serial-numbered-fungible-tokens/30519"
---
# ERC-XXXX: Serial-Numbered Fungible Tokens

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-xxxx-serial-numbered-fungible-tokens/30519)  |  Thu, 26 Nov 2026 03:00:53 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 바이낸스 해킹 사례를 통해 현재 스테이블코인 동결 방식의 한계를 지적하며, 일련번호가 부여된 대체 가능 토큰(Serial-Numbered Fungible Tokens)을 제안하여 도난 자금에 대한 보다 세밀한 통제 가능성을 모색합니다.

**리서치 앵글:** 스테이블코인 동결 방식 개선 논의는 기관 DeFi 도입 시 요구되는 자산 통제 및 보안 강화와 관련이 있으며, 토큰의 대체 가능성 및 검열 저항성 측면에서 RWA와 같은 자산의 온체인 표현 방식에 영향을 줄 수 있습니다.

## 원문 미리보기
<p>When Binance’s hot wallets were drained on 29 October, the stablecoin issuers reacted fast: Tether froze the attackers’ main wallet 37 minutes after the stolen USDT arrived there, and Circle froze the USDC three minutes later (<a href="https://www.elliptic.co/insights/binance-largest-hack-in-history/" rel="noopener nofollow ugc">Elliptic</a>). <strong>It was still a race.</strong> Several hundred million dollars of stablecoins had been swapped, sold or pledged as collateral before a freeze reached them.</p>
<p><strong>A freeze by address stops only what is still at that address</strong>, an