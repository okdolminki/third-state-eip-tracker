---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-XXXX: Holding-Time Auto Staking for NFTs"
author: ""
pub_date: "Mon, 28 Sep 2026 05:38:19 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-09-28
sources:
  - "https://ethereum-magicians.org/t/erc-xxxx-holding-time-auto-staking-for-nfts/29787"
---
# ERC-XXXX: Holding-Time Auto Staking for NFTs

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-xxxx-holding-time-auto-staking-for-nfts/29787)  |  Mon, 28 Sep 2026 05:38:19 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** NFT를 보유하는 것만으로 스테이킹 시간이 자동으로 적립되는 ERC-721 확장 제안으로, 가스비, 토큰 이동, 커스터디 위험 문제를 해결합니다.

**리서치 앵글:** NFT 스테이킹의 간소화 및 커스터디 위험 감소는 기관의 DeFi 도입을 촉진할 수 있습니다.

## 원문 미리보기
<p>We propose an ERC-721 extension in which tokens accrue staking time simply by being held, without staking transactions or custody transfers.</p>
<p><strong>The problem:</strong><br>
Many NFT projects reward long-term holders, but the usual staking pattern asks holders to call a staking function, move the token into a separate staking contract, and later withdraw it. Every step costs gas, the token leaves the holder’s wallet (breaking token-gated access, profile pictures and other wallet-based utilities), and a separate contract adds its own custody risk. What these systems actually measure 