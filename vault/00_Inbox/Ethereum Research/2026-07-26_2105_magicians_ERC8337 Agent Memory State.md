---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8337: Agent Memory State"
author: ""
pub_date: "Sun, 26 Jul 2026 07:42:31 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-26
sources:
  - "https://ethereum-magicians.org/t/erc-8337-agent-memory-state/29098"
---
# ERC-8337: Agent Memory State

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8337-agent-memory-state/29098)  |  Sun, 26 Jul 2026 07:42:31 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 온체인에 메모리 내용을 저장하지 않고 자율 에이전트의 메모리 상태를 검증 가능한 방식으로 버전 관리하는 ERC-8337에 대한 논의가 진행 중입니다.

**리서치 앵글:** 계정 추상화(EIP-7702)와 연관하여 자율 에이전트의 복잡한 상태 관리 및 진화하는 로직 구현에 미칠 잠재적 영향을 분석합니다.

## 원문 미리보기
<p>Hi all — draft ERC for discussion: verifiable version control for autonomous-agent memory, without putting any memory content on chain.</p>
<p>Status: submitted upstream as ERC-8337 (ethereum/ERCs#1910) — all CI checks including eipw passing, awaiting editor review. A public Sepolia deployment is live (see Links and the Update Log).</p>
<p>The case, in plain terms<br>
An agent that has been running for a year is not the model it started as. It has accumulated preferences, distilled skills, revised policies, and a record of what it did and why. That accumulated state — its memory and its beh