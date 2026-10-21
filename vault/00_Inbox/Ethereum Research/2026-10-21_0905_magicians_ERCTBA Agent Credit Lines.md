---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-TBA: Agent Credit Lines"
author: ""
pub_date: "Tue, 20 Oct 2026 15:22:51 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-21
sources:
  - "https://ethereum-magicians.org/t/erc-tba-agent-credit-lines/30023"
---
# ERC-TBA: Agent Credit Lines

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-tba-agent-credit-lines/30023)  |  Tue, 20 Oct 2026 15:22:51 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** ERC-8004 기반 자율 에이전트를 위한 표준화된 온체인 회전 신용 공통 인터페이스 초안을 제안한다.

**리서치 앵글:** 계정 추상화 및 자율 에이전트 도입에 따른 온체인 무담보·신용 대출 시장의 발전 방향과 Morpho, Maple 등 대출 프로토콜 연계 가능성을 분석할 수 있다.

## 원문 미리보기
<p>Lenders to ERC-8004 agents are appearing, and each has its own ABI, so every wallet, payment client and MCP server integrates every lender separately. This draft is one lender-neutral interface for revolving credit to agent identities: how much an identity can borrow now (<code>availableCredit</code>), what a draw would cost (<code>quote</code>), draw it with a fee cap (<code>borrow</code>), what closes it (<code>amountDue</code>), repay it (anyone may), and mark it defaulted once overdue (anyone may). Three events, <code>Borrowed</code>, <code>Repaid</code> and <code>Defaulted</code>, reco