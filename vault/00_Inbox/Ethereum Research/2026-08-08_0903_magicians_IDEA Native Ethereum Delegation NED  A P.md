---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "[IDEA] Native Ethereum Delegation (NED) — A Protocol-Level Delegation Market With Diminishing Concentration Economics"
author: ""
pub_date: "Fri, 07 Aug 2026 20:34:02 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-08
sources:
  - "https://ethereum-magicians.org/t/idea-native-ethereum-delegation-ned-a-protocol-level-delegation-market-with-diminishing-concentration-economics/29356"
---
# [IDEA] Native Ethereum Delegation (NED) — A Protocol-Level Delegation Market With Diminishing Concentration Economics

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/idea-native-ethereum-delegation-ned-a-protocol-level-delegation-market-with-diminishing-concentration-economics/29356)  |  Fri, 07 Aug 2026 20:34:02 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 프로토콜 레이어에서 위임 시장을 구축하여 스테이킹 중앙집중화를 방지하는 '네이티브 이더리움 위임(NED)' 경제 모델에 대한 아이디어 제안입니다.

**리서치 앵글:** Lido, Ether.fi, EigenLayer 등 LST/LRT 생태계의 위임 구조 및 이더리움 스테이킹 경제학 테마와 밀접하게 연관됩니다.

## 원문 미리보기
<p>Discussion topic for <strong>Native Ethereum Delegation (NED)</strong>.</p>
<p>This is an idea-stage proposal, not yet an EIP. I’m posting it to get feedback on the underlying direction and, if there is enough merit, hopefully develop a stronger community-driven specification before anything formal is proposed.</p>
<p>I’m approaching this mostly from the staking incentive and economic design side rather than as a consensus-layer researcher, so I’m particularly interested in corrections where my assumptions about the protocol are wrong.</p>
<h4><a name="p-72919-update-log-1" class="anchor" h