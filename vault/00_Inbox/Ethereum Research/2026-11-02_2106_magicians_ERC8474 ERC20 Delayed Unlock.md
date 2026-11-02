---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8474: ERC-20 Delayed Unlock"
author: ""
pub_date: "Mon, 02 Nov 2026 08:55:11 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-02
sources:
  - "https://ethereum-magicians.org/t/erc-8474-erc-20-delayed-unlock/30177"
---
# ERC-8474: ERC-20 Delayed Unlock

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8474-erc-20-delayed-unlock/30177)  |  Mon, 02 Nov 2026 08:55:11 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** ERC-8474는 토큰 보유자가 출금 잠금 기능을 제어하고 블록 기반의 지연 해제 및 독립적인 잠금 관리자를 포함하는 ERC-20 확장 제안입니다.

**리서치 앵글:** 기관 DeFi 도입 시 토큰 보안 강화 및 자산 관리 리스크 감소에 기여할 수 있는 잠재적 요소입니다.

## 원문 미리보기
<p>I would like feedback on ERC-8474, an opt-in ERC-20 extension for holder-controlled outgoing transfer locks with a block-based unlock delay and an independent locking guardian.</p>
<p>Proposal and specification: <a href="https://github.com/ethereum/ERCs/pull/2129" class="inline-onebox" rel="noopener nofollow ugc">Add ERC: ERC-20 Delayed Unlock by shargon · Pull Request #2129 · ethereum/ERCs · GitHub</a></p>
<h2><a name="p-76063-motivation-1" class="anchor" href="https://ethereum-magicians.org#p-76063-motivation-1" aria-label="Heading link"></a>Motivation</h2>
<p>Cold storage protects keys a