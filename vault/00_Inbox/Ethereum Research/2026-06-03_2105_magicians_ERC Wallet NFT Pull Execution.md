---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC: Wallet NFT Pull Execution"
author: ""
pub_date: "Wed, 03 Jun 2026 09:47:05 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-03
sources:
  - "https://ethereum-magicians.org/t/erc-wallet-nft-pull-execution/28693"
---
# ERC: Wallet NFT Pull Execution

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-wallet-nft-pull-execution/28693)  |  Wed, 03 Jun 2026 09:47:05 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 이 제안은 외부 호출 중 일시적인 NFT 풀 권한을 위한 지갑 네이티브 기본 요소를 정의하며, 계정이 `executeWithNftPull`을 통해 특정 NFT를 일회성으로 풀할 수 있도록 합니다.

**리서치 앵글:** 계정 추상화(EIP-7702)와 관련하여 지갑의 NFT 권한 관리 및 사용자 경험 개선 가능성을 탐색합니다.

## 원문 미리보기
<p>This proposal defines a wallet-native primitive for temporary NFT pull authorization during one external call.</p>
<p>A compliant account exposes <code>executeWithNftPull</code>, which opens a transient pull context for one target, one <code>ERC-721</code> asset, and one token id. During that call, the bound target may pull the NFT from the account by calling <code>nftPullToCaller</code>. Outside the active call window, pull attempts fail.</p>
<p>The intended implementation model is execution-local state, for example transient storage. The account records the active <code>(target, asset, to