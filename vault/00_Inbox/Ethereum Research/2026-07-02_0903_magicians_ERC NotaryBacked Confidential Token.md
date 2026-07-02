---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC: Notary-Backed Confidential Token"
author: ""
pub_date: "Wed, 01 Jul 2026 12:36:50 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-02
sources:
  - "https://ethereum-magicians.org/t/erc-notary-backed-confidential-token/28908"
---
# ERC: Notary-Backed Confidential Token

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-notary-backed-confidential-token/28908)  |  Wed, 01 Jul 2026 12:36:50 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 공증인 기반의 기밀 UTXO 토큰 표준(ERC)에 대한 논의가 시작되었으며, 이는 오프체인에서 개인 상태 전환을 검증하는 모델을 제안합니다.

**리서치 앵글:** 기관 DeFi 도입 및 RWA 토큰화에 필요한 기밀성 및 규제 준수 가능성을 탐색합니다.

## 원문 미리보기
<p>I’m preparing an ERC titled “Notary-Backed Confidential Token” and wanted to open a discussion thread here before submitting the PR.</p>
<h2><a name="p-71550-context-1" class="anchor" href="https://ethereum-magicians.org#p-71550-context-1" aria-label="Heading link"></a>Context</h2>
<p>The core model is a confidential UTXO token with transitions validated by a notary address. The notary address may represent a single party, a group, a smart contract submission gate, or another implementation-specific validation process.</p>
<p>The notary validates private state transitions off-chain, includi