---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-1833: Bounded Agent Actions - a metering layer for agent authority"
author: ""
pub_date: "Tue, 23 Jun 2026 14:29:20 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-24
sources:
  - "https://ethereum-magicians.org/t/erc-1833-bounded-agent-actions-a-metering-layer-for-agent-authority/28851"
---
# ERC-1833: Bounded Agent Actions - a metering layer for agent authority

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-1833-bounded-agent-actions-a-metering-layer-for-agent-authority/28851)  |  Tue, 23 Jun 2026 14:29:20 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 이 ERC는 에이전트가 위임받은 권한 중 얼마나 사용했는지 추적하여, 남은 권한을 하위 컨트랙트가 조회할 수 있도록 하는 온체인 커서 객체를 제안합니다.

**리서치 앵글:** 계정 추상화(EIP-7702)와 연관되어, 에이전트의 위임된 권한 사용을 추적하는 메커니즘은 스마트 계정 및 기관 DeFi 도입에 중요한 영향을 미칠 수 있습니다.

## 원문 미리보기
<p><strong>ERC: Bounded Agent Actions - a metering layer for agent authority</strong></p>
<p>There are a lot of agent ERCs landing right now, so I want to be clear up front about what this one isn’t. It doesn’t enforce anything, it doesn’t run a workflow, and it doesn’t settle. What it does is narrow: <strong>it keeps a running count of how much of a bounded mandate an agent has already spent across its actions, so a downstream contract can look up how much room is left.</strong> That’s the whole idea: <strong>one small on-chain object, a cursor, with a single interface to read it and advance 