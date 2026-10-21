---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-TBA: Credit history for ERC-8004 agents"
author: ""
pub_date: "Tue, 20 Oct 2026 15:22:18 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-21
sources:
  - "https://ethereum-magicians.org/t/erc-tba-credit-history-for-erc-8004-agents/30022"
---
# ERC-TBA: Credit history for ERC-8004 agents

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-tba-credit-history-for-erc-8004-agents/30022)  |  Tue, 20 Oct 2026 15:22:18 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** ERC-8004 에이전트의 대출 상환 및 연체 이력을 온체인에 기록하여 신용 평판을 관리하는 레지스트리 제안입니다.

**리서치 앵글:** 기관 DeFi 도입 및 계정 추상화 테마와 연관, 온체인 신용 기록을 통해 DeFi 대출 시장의 효율성 및 기관 참여 증진 가능성을 탐색합니다.

## 원문 미리보기
<p>This is a profile of the ERC-8004 Reputation Registry for loan outcomes: loans opened, repaid on time, repaid late, defaulted. It adds no core contract. A lender posts ordinary <code>giveFeedback</code> entries with two tags, <code>credit.statement</code> and <code>credit.defaulted</code>, whose files travel inside the entry as <code>data:</code> URIs.</p>
<p>A statement commits, with a Merkle root, to every loan of an agent that closed in a block window at the lender’s contracts. Each leaf names the lender’s own log that closed the loan, so a reader with only an RPC endpoint can rebuild ev