---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8449: Engine API proposal lookahead"
author: ""
pub_date: "Tue, 20 Oct 2026 06:11:47 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-20
sources:
  - "https://ethereum-magicians.org/t/eip-8449-engine-api-proposal-lookahead/30016"
---
# EIP-8449: Engine API proposal lookahead

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8449-engine-api-proposal-lookahead/30016)  |  Tue, 20 Oct 2026 06:11:47 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8449는 합의 클라이언트가 실행 클라이언트에게 현재 및 다음 에포크의 검증자 블록 제안 정보를 미리 알려주는 Engine API 메서드를 추가합니다.

**리서치 앵글:** 블록 제안 정보 사전 공유를 통해 MEV 전략 최적화 및 블록 빌딩 효율성 증대에 기여할 수 있습니다.

## 원문 미리보기
<p>Discussion topic for <a href="https://github.com/ethereum/EIPs/pull/12547" rel="noopener nofollow ugc">EIP-8449</a></p>
<p>This EIP adds an Engine API method, <code>engine_proposalLookaheadUpdatedV1</code>, with which a consensus client tells its execution client the upcoming proposals of its validators in the current and next epoch: slot, timestamp, fee recipient and target gas limit. It is a notice, not a command: it starts no build, names no parent block and changes no consensus rule. The execution client decides whether, when and how to prepare.</p>
<p>Today an execution client learns o