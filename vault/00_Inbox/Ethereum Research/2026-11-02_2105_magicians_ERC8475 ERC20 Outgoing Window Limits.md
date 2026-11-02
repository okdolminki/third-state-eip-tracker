---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8475: ERC-20 Outgoing Window Limits"
author: ""
pub_date: "Mon, 02 Nov 2026 08:56:19 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-02
sources:
  - "https://ethereum-magicians.org/t/erc-8475-erc-20-outgoing-window-limits/30178"
---
# ERC-8475: ERC-20 Outgoing Window Limits

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8475-erc-20-outgoing-window-limits/30178)  |  Mon, 02 Nov 2026 08:56:19 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** ERC-8475는 전송당 한도와 고정 블록 기간당 총 출금 한도를 결합한 선택적 ERC-20 확장 기능으로, 자금 보안 강화를 목표로 합니다.

**리서치 앵글:** 이 ERC-20 확장은 기관 DeFi 도입 시 필요한 자금 보안 및 위험 관리 강화에 기여할 수 있습니다.

## 원문 미리보기
<p>I would like feedback on ERC-8475, an opt-in ERC-20 extension combining a per-transfer cap with an aggregate outgoing cap per fixed block window.</p>
<p>Proposal and specification: <a href="https://github.com/ethereum/ERCs/pull/2130" class="inline-onebox" rel="noopener nofollow ugc">Add ERC: ERC-20 Outgoing Window Limits by shargon · Pull Request #2130 · ethereum/ERCs · GitHub</a></p>
<h2><a name="p-76064-motivation-1" class="anchor" href="https://ethereum-magicians.org#p-76064-motivation-1" aria-label="Heading link"></a>Motivation</h2>
<p>A compromised signing or withdrawal workflow can di