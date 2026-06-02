---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC Proposal: RWA Disclosure Interfaces"
author: ""
pub_date: "Tue, 02 Jun 2026 11:18:41 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-02
sources:
  - "https://ethereum-magicians.org/t/erc-proposal-rwa-disclosure-interfaces/28679"
---
# ERC Proposal: RWA Disclosure Interfaces

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-proposal-rwa-disclosure-interfaces/28679)  |  Tue, 02 Jun 2026 11:18:41 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** RWA 토큰의 오프체인 정보를 온체인에서 투명하게 공개하기 위한 새로운 ERC 인터페이스를 제안합니다.

**리서치 앵글:** RWA 토큰의 투명성 및 표준화는 Third State의 RWA 리서치 테마와 직접적으로 연관됩니다.

## 원문 미리보기
<h1><a name="p-70525-hi-everyone-1" class="anchor" href="https://ethereum-magicians.org#p-70525-hi-everyone-1" aria-label="Heading link"></a>Hi everyone,</h1>
<p>I would like to propose a new ERC for Real World Asset (RWA) disclosure interfaces.</p>
<h1><a name="p-70525-summary-2" class="anchor" href="https://ethereum-magicians.org#p-70525-summary-2" aria-label="Heading link"></a>Summary</h1>
<p>RWA tokens depend on off-chain facts that normal token interfaces do not expose: reserve reports, NAV statements, audit reports, backing status, global supply statements, and legal documents. Today, ev