---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "(ERC Draft), Secure Transaction Verification and Authorization (STVA) – Stopping Blind Signing & Multisig UI Attacks"
author: ""
pub_date: "Tue, 27 Oct 2026 18:33:48 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-28
sources:
  - "https://ethereum-magicians.org/t/erc-draft-secure-transaction-verification-and-authorization-stva-stopping-blind-signing-multisig-ui-attacks/30106"
---
# (ERC Draft), Secure Transaction Verification and Authorization (STVA) – Stopping Blind Signing & Multisig UI Attacks

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-draft-secure-transaction-verification-and-authorization-stva-stopping-blind-signing-multisig-ui-attacks/30106)  |  Tue, 27 Oct 2026 18:33:48 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 이 ERC 초안은 블라인드 서명 및 멀티시그 UI 공격을 방지하기 위해 트랜잭션 서명을 독립적으로 검증 가능하고 사람이 이해할 수 있도록 표준화하는 것을 목표로 합니다.

**리서치 앵글:** 기관 DeFi 도입의 핵심 장애물인 트랜잭션 보안 및 검증 문제를 해결하며, 계정 추상화의 발전과도 밀접하게 연관됩니다.

## 원문 미리보기
<p>Hi everyone,</p>
<p>Following the wave of high-value signing-flow and supply-chain attacks (most notably the 2025 Bybit Safe incident and numerous access-control losses), I am proposing a new ERC focused on making transaction signing independently verifiable and human-meaningful.</p>
<p>Core idea:</p>
<p>Standardize a Verification Payload + independent simulation interface + scoped capabilities so that “what you see is what you sign” becomes enforceable rather than aspirational.</p>
<p>Motivation:</p>
<p>Analysis of major incidents (including the February 2025 Bybit ~$1.4–1.5B Safe multisig