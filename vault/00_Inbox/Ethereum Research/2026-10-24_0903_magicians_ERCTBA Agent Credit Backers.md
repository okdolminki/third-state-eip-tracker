---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-TBA: Agent Credit Backers"
author: ""
pub_date: "Fri, 23 Oct 2026 14:32:17 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-24
sources:
  - "https://ethereum-magicians.org/t/erc-tba-agent-credit-backers/30062"
---
# ERC-TBA: Agent Credit Backers

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-tba-agent-credit-backers/30062)  |  Fri, 23 Oct 2026 14:32:17 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 이 EIP 초안은 에이전트의 신용 대출에 대해 제3자(스테이커, 담보 볼트, 보험사)가 보증을 서서 채무 불이행 위험을 흡수하고, EIP-712 동의를 통해 대출을 지원하는 메커니즘을 제안한다.

**리서치 앵글:** 에이전트 신용 보증 메커니즘은 계정 추상화(EIP-7702)를 활용한 기관 DeFi 도입 및 새로운 신용 모델 구축과 연관된다.

## 원문 미리보기
<p>A line of credit to an agent is a bet on whoever stands behind the agent. This draft lets a third party (a staker, a collateral vault, an insurer) stand behind a lender’s line to an agent identity and absorb its defaults, with the identity owner’s EIP-712 consent. The lender asks the backer before each draw (<code>canBorrow</code>), tells it of each draw (<code>onBorrow</code>), and on a default takes the principal from the backer and tells it (<code>onDefault</code>, with what was paid); lowered, removed or replaced lines are told once each (<code>onRelease</code>). Neither a backer nor th