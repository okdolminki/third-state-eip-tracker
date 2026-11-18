---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC: Onchain Announcements"
author: ""
pub_date: "Wed, 18 Nov 2026 06:33:26 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-18
sources:
  - "https://ethereum-magicians.org/t/erc-onchain-announcements/30428"
---
# ERC: Onchain Announcements

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-onchain-announcements/30428)  |  Wed, 18 Nov 2026 06:33:26 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 온체인 상태 변경과 관련된 인간이 읽을 수 있는 설명을 연결하는 표준화된 ERC 초안으로, `Announcement` 이벤트를 통해 상태 변경을 명확히 공개하는 메커니즘을 제안합니다.

**리서치 앵글:** 기관 DeFi 도입 시 필요한 온체인 투명성 및 감사 가능성을 높이는 표준화된 온체인 공시 메커니즘과 연관됩니다.

## 원문 미리보기
<p>This thread is for discussion of a draft ERC: <strong>Onchain Announcements</strong>.</p>
<p><strong>Summary.</strong> The ERC defines a convention for coupling a human-readable disclosure with the state changes it describes. An announcement is a bracket: an <code>Announcement</code> event opens it, zero or more self-targeted calls execute atomically inside it, and an <code>EndAnnouncement</code> event closes it. A caller-chosen <code>id</code> ties every effect in the bracket to its disclosure.</p>
<ul>
<li><code>announce(internalCalls, id, description, uri)</code> publishes a new announce