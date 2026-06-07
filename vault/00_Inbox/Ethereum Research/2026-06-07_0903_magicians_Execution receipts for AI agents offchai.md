---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Execution receipts for AI agents: off-chain evidence, on-chain roots, and verifiable session proofs"
author: ""
pub_date: "Sat, 06 Jun 2026 22:40:19 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-07
sources:
  - "https://ethereum-magicians.org/t/execution-receipts-for-ai-agents-off-chain-evidence-on-chain-roots-and-verifiable-session-proofs/28737"
---
# Execution receipts for AI agents: off-chain evidence, on-chain roots, and verifiable session proofs

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/execution-receipts-for-ai-agents-off-chain-evidence-on-chain-roots-and-verifiable-session-proofs/28737)  |  Sat, 06 Jun 2026 22:40:19 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** AI 에이전트의 신원 및 권한을 넘어, 에이전트가 실제로 수행한 작업을 검증 가능한 기록으로 남기는 '실행 영수증'에 대한 논의가 제안되었다.

**리서치 앵글:** AI 에이전트의 검증 가능한 실행 기록은 기관 DeFi 도입 및 계정 추상화 환경에서 필수적인 감사 및 신뢰 기반을 제공한다.

## 원문 미리보기
<p>Hi everyone,</p>
<p>I want to propose a discussion around execution receipts for AI agents.</p>
<p>A lot of current agent work focuses on identity, reputation, permissions, payment, and tool execution. Those are important, but I think there is another layer that production agent systems will need:</p>
<p>«a verifiable record of what the agent actually did.»</p>
<p>For coding agents and tool-using agents, the question is not only:</p>
<p>«Can this agent perform the task?»</p>
<p>It is also:</p>
<p>«Can a user, another agent, or a verifier later check what happened?»</p>
<p>Problem</p>
<p>AI 