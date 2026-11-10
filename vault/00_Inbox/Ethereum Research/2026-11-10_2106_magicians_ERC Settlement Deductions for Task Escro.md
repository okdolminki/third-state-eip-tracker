---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC: Settlement Deductions for Task Escrows"
author: ""
pub_date: "Tue, 10 Nov 2026 04:18:12 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-10
sources:
  - "https://ethereum-magicians.org/t/erc-settlement-deductions-for-task-escrows/30323"
---
# ERC: Settlement Deductions for Task Escrows

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-settlement-deductions-for-task-escrows/30323)  |  Tue, 10 Nov 2026 04:18:12 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 온체인 AI 에이전트의 작업 보상 지급 시 세금, 수수료, 대출 상환 등 다양한 공제액을 에스크로가 자동으로 처리할 수 있도록 하는 ERC 제안.

**리서치 앵글:** 온체인 결제 시 다양한 공제액 처리를 표준화하여 기관의 DeFi 도입 및 복잡한 금융 거래 지원 가능성 연구.

## 원문 미리보기
<p>Hi everyone,</p>
<p>AI agents now take on paid work on-chain. The client locks the pay in an escrow, and the escrow pays the agent when the work is accepted. As this grows, each payment also has to cover others: a tax that funds public services, a fee to whoever referred the job, or the repayment of a loan the agent took to do the job.</p>
<p>This is a draft ERC for <strong>Settlement Deductions</strong>. It lets an escrow withhold these amounts from each payout. The escrow does not need to know the rules behind them. None of them can stall the payout. It works for any task escrow, not only