---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC Discussion: ERC-20 Transferable Timelock"
author: ""
pub_date: "Tue, 24 Nov 2026 12:14:55 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-25
sources:
  - "https://ethereum-magicians.org/t/erc-discussion-erc-20-transferable-timelock/30493"
---
# ERC Discussion: ERC-20 Transferable Timelock

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-discussion-erc-20-transferable-timelock/30493)  |  Tue, 24 Nov 2026 12:14:55 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 새로 발행된 토큰이 발행 블록 내에서 소각되는 것을 방지하고, 전송 가능한 타임락 잔액을 추적하는 ERC-20 확장 제안.

**리서치 앵글:** 기관 DeFi 도입 시 토큰 발행 및 유통에 대한 통제 메커니즘으로 활용 가능성.

## 원문 미리보기
<p>I propose an ERC-20 extension that prevents fresh tokens from being burned in the block in which they were minted. The tokens stay transferable and remain compatible with normal DeFi operations.</p>
<p>I think the pattern is worth sharing, but I am not sure this deserves its own ERC, so I am posting it here for feedback on the concept, the implementation, and whether it belongs in a standard.</p>
<p>The extension tracks a timelocked balance for each account. A mint increases the timelocked balance, a transfer can move part or all of it to another account, and a burn can use only the unlocke