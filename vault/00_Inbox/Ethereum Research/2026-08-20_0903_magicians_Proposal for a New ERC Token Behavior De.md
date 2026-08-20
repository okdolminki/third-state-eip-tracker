---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Proposal for a New ERC: Token Behavior Declaration"
author: ""
pub_date: "Wed, 19 Aug 2026 21:31:47 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-20
sources:
  - "https://ethereum-magicians.org/t/proposal-for-a-new-erc-token-behavior-declaration/29464"
---
# Proposal for a New ERC: Token Behavior Declaration

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/proposal-for-a-new-erc-token-behavior-declaration/29464)  |  Wed, 19 Aug 2026 21:31:47 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 토큰이 ERC-20 또는 ERC-721 표준과 다른 특성(수수료, 리베이스, 일시정지 등)을 선언하는 새로운 ERC 제안이 논의 중이다.

**리서치 앵글:** LST/LRT 및 RWA 토큰의 복잡한 행동(리베이스, 수수료, 블록리스트 등)을 표준화하여 DeFi 프로토콜의 통합 용이성과 리스크 관리를 개선할 수 있다.

## 원문 미리보기
<p>Short version: one view function, behaviorFlags, returning a uint256 in which each bit names a way the token departs from plain ERC-20 or ERC-721. Fee-on-transfer, rebasing, transfer hook, pausable, blocklist, non-transferable, upgradeable, mintable, seizable, and two that only mean anything for 721, operator-restricted and metadata-mutable.</p>
<p>The function is not the interesting part. Two rules hang off it, one of which I am confident about and one of which I am not, and there is a third problem underneath both that I have not solved and would mostly like help with.</p>
<p>The first ru