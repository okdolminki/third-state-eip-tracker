---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "How Arbitrum's freezes send transactions from an address without its key"
author: ""
pub_date: "Mon, 02 Nov 2026 06:48:04 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-02
sources:
  - "https://ethereum-magicians.org/t/how-arbitrums-freezes-send-transactions-from-an-address-without-its-key/30175"
---
# How Arbitrum's freezes send transactions from an address without its key

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/how-arbitrums-freezes-send-transactions-from-an-address-without-its-key/30175)  |  Mon, 02 Nov 2026 06:48:04 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** Arbitrum Security Council이 바이낸스 및 KelpDAO 익스플로잇 관련 주소의 자산을 키 없이 동결한 사례를 다루며, L2의 보안 모델과 중앙화 이슈를 제기합니다.

**리서치 앵글:** L2의 보안 및 거버넌스 모델, 기관 DeFi 도입 시 중앙화 리스크, 그리고 계정 추상화(EIP-7702)와 관련된 주소 제어 방식의 근본적 논의와 연관됩니다.

## 원문 미리보기
<p>On 30 October the Arbitrum Security Council froze 8,425 ETH and 74,559,805.2 ARB that an address tied to the Binance exploit held on Arbitrum One (<a href="https://forum.arbitrum.foundation/t/31625" rel="noopener nofollow ugc">notice</a>). It was the second time this year. On 21 April they did the same with 30,765 ETH from the KelpDAO exploiter (<a href="https://forum.arbitrum.foundation/t/30803" rel="noopener nofollow ugc">notice</a>).</p>
<p>When we review drafts here we usually take it as given that an address only moves when its key signs. A few drafts this month come from teams buildin