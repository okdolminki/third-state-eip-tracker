---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8392: Asset Status Interface for Tokenized Assets"
author: ""
pub_date: "Mon, 24 Aug 2026 02:09:15 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-24
sources:
  - "https://ethereum-magicians.org/t/erc-8392-asset-status-interface-for-tokenized-assets/29489"
---
# ERC-8392: Asset Status Interface for Tokenized Assets

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8392-asset-status-interface-for-tokenized-assets/29489)  |  Mon, 24 Aug 2026 02:09:15 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 토큰화된 자산(예: 토큰화 주식)의 상태 정보(시장 개장 여부, 거래 중단 등)가 표준화되어 있지 않아 담보 가치 평가 및 활용에 어려움이 있으며, 이를 해결하기 위한 ERC-8392 인터페이스가 제안되었다.

**리서치 앵글:** RWA 테마와 관련하여 토큰화된 자산의 표준화된 상태 인터페이스 부재가 기관 DeFi 도입의 걸림돌임을 지적하고 해결책을 제시한다.

## 원문 미리보기
<p>Tokenized stocks now transfer onchain 24/7 while NYSE is open 32.5 hours a week. The<br>
state that determines whether one of these tokens can be safely valued or used as<br>
collateral — is the reference market open, is it halted, is the valuation feed stale<br>
because it’s Sunday or stale because it’s broken, can anyone actually redeem right<br>
now — is not observable through ERC-20, and today every issuer exposes it differently:<br>
Ondo has an offchain HTTP status API, Robinhood Chain tokens have a proprietary<br>
<code>oraclePaused()</code>, most others have a bare <code>paused()</co