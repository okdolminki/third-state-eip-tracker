---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC: Wallet-Scoped NFT Pull Execution"
author: ""
pub_date: "Wed, 03 Jun 2026 09:29:08 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-03
sources:
  - "https://ethereum-magicians.org/t/erc-wallet-scoped-nft-pull-execution/28692"
---
# ERC: Wallet-Scoped NFT Pull Execution

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-wallet-scoped-nft-pull-execution/28692)  |  Wed, 03 Jun 2026 09:29:08 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 이 제안은 단일 외부 호출 동안 임시 NFT 풀 권한을 위한 지갑 네이티브 기본 기능을 정의합니다.

**리서치 앵글:** 계정 추상화(EIP-7702)와 연관된 지갑의 NFT 상호작용 방식 개선 제안입니다.

## 원문 미리보기
<p>This proposal defines a wallet-native primitive for temporary NFT pull authorization during one external call.</p>
<p>A compliant account exposes <code>executeWithNftPull</code>, which opens a transient pull context for one target, one <code>ERC-721</code> asset, and one token id. During that call, the bound target may pull the NFT from the account by calling <code>nftPullToCaller</code>. Outside the active call window, pull attempts fail.</p>
<p>The intended implementation model is execution-local state, for example transient storage. The account records the active <code>(target, asset, to