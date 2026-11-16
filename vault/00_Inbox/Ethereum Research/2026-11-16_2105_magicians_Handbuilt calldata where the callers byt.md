---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Hand-built calldata where the caller's bytes become the selector (Scroll's 10 Nov fix)"
author: ""
pub_date: "Mon, 16 Nov 2026 06:45:41 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-16
sources:
  - "https://ethereum-magicians.org/t/hand-built-calldata-where-the-callers-bytes-become-the-selector-scrolls-10-nov-fix/30405"
---
# Hand-built calldata where the caller's bytes become the selector (Scroll's 10 Nov fix)

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/hand-built-calldata-where-the-callers-bytes-become-the-selector-scrolls-10-nov-fix/30405)  |  Mon, 16 Nov 2026 06:45:41 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 스크롤 메인넷에서 계약 간 호출 방식의 버그로 인해 긴급 업그레이드가 발생했으며, 이는 calldata 처리의 취약성을 보여줍니다.

**리서치 앵글:** L2 확장성 및 보안, 특히 L2 상의 스마트 컨트랙트 상호작용의 취약성 분석에 중요합니다.

## 원문 미리보기
<p>On 10 November Scroll registered a new bundle proof verifier on mainnet after a bug bounty report, and posted a report the next day (<a href="https://forum.scroll.io/t/report-scroll-mainnet-emergency-upgrade-on-2026-11-10/1586" rel="noopener nofollow ugc">Scroll Mainnet Emergency Upgrade on 2026-11-10</a>). Nothing was wrong with the proof system. The bug was in how one contract called another, and I’ve been grepping for the same shape since I read it.</p>
<h3><a name="p-76698-what-the-old-code-did-1" class="anchor" href="https://ethereum-magicians.org#p-76698-what-the-old-code-did-1" aria-