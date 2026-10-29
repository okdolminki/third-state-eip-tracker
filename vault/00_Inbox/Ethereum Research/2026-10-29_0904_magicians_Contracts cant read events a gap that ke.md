---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Contracts can't read events: a gap that keeps coming up in ERC drafts"
author: ""
pub_date: "Wed, 28 Oct 2026 18:28:53 +0000"

importance: medium
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-29
sources:
  - "https://ethereum-magicians.org/t/contracts-cant-read-events-a-gap-that-keeps-coming-up-in-erc-drafts/30120"
---
# Contracts can't read events: a gap that keeps coming up in ERC drafts

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/contracts-cant-read-events-a-gap-that-keeps-coming-up-in-erc-drafts/30120)  |  Wed, 28 Oct 2026 18:28:53 +0000

## AI 분석
**중요도:** medium | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 컨트랙트가 이벤트를 직접 읽을 수 없어 ERC 초안에서 반복적으로 발생하는 설계상의 문제점을 지적하는 글.

**리서치 앵글:** L2 확장성 및 계정 추상화를 포함한 미래 DeFi 프로토콜 설계에 미치는 근본적인 영향 분석.

## 원문 미리보기
<p>Since mid-September the same gap has come up in at least four ERC threads, raised by different people. It shows up in two directions, so I wanted to put it in one place for anyone writing a draft right now.</p>
<h3><a name="p-75839-the-two-directions-1" class="anchor" href="https://ethereum-magicians.org#p-75839-the-two-directions-1" aria-label="Heading link"></a>The two directions</h3>
<p><strong>1. A fact lives only in an event, and a contract needs it.</strong></p>
<p>In the <a href="https://ethereum-magicians.org/t/erc-8467-agent-credit-backers/30062">ERC-8467</a> (Agent Credit Backers)