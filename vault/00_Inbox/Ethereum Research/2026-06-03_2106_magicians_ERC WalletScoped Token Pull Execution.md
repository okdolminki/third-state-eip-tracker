---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC: Wallet-Scoped Token Pull Execution"
author: ""
pub_date: "Wed, 03 Jun 2026 09:22:45 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-03
sources:
  - "https://ethereum-magicians.org/t/erc-wallet-scoped-token-pull-execution/28691"
---
# ERC: Wallet-Scoped Token Pull Execution

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-wallet-scoped-token-pull-execution/28691)  |  Wed, 03 Jun 2026 09:22:45 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 이 제안은 지갑이 단일 외부 호출 동안 특정 ERC-20 토큰을 특정 대상에게 임시로 인출할 수 있도록 허용하는 새로운 원시 기능을 정의합니다.

**리서치 앵글:** 지갑의 토큰 인출 권한을 개선하여 계정 추상화(EIP-7702) 및 기관 DeFi 도입에 기여할 수 있습니다.

## 원문 미리보기
<p>This proposal defines a wallet-native primitive for temporary <code>ERC-20</code> pull authorization during one external call.</p>
<p>A compliant account exposes <code>executeWithTokenPull</code>, which opens a transient pull context for one target, one asset, and one maximum amount. During that call, the bound target may pull tokens from the account by calling <code>tokenPullToCaller</code>. Outside the active call window, pull attempts fail.</p>
<p>The intended implementation model is execution-local state, for example transient storage. The account records the active <code>(target, asset