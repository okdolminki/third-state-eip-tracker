---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Lineage Registry: an ERC-721 extension for on-chain genealogical trees"
author: ""
pub_date: "Mon, 17 Aug 2026 07:19:12 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-17
sources:
  - "https://ethereum-magicians.org/t/lineage-registry-an-erc-721-extension-for-on-chain-genealogical-trees/29441"
---
# Lineage Registry: an ERC-721 extension for on-chain genealogical trees

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/lineage-registry-an-erc-721-extension-for-on-chain-genealogical-trees/29441)  |  Mon, 17 Aug 2026 07:19:12 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 온체인 족보(계보)를 위한 ERC-721 확장 표준을 제안하는 글입니다.

**리서치 앵글:** NFT의 온체인 계보를 추적하는 표준으로, 기관 DeFi 도입 시 자산의 투명한 이력 관리나 RWA 토큰화에 활용될 가능성이 있습니다.

## 원문 미리보기
<p>Author: Henrique L. Alvim (<a class="mention" href="https://ethereum-magicians.org/u/henriquelalvim">@henriquelalvim</a>)<br>
Reference implementation: <a href="https://github.com/henriquelalvim/genealogicalRegistryBlockchain/tree/v0.1.0" rel="noopener nofollow ugc">genealogicalRegistryBlockchain</a><br>
Base Sepolia deployment: <a href="https://base-sepolia.blockscout.com/address/0xcd64676020A0bbfaA35252E9A25eF7662463EdEC?tab=contract" rel="noopener nofollow ugc">Base Sepolia Blockscout</a></p>
<hr>
<blockquote>
<p><strong>TL;DR</strong> — I am proposing a standard for <strong>decentralize