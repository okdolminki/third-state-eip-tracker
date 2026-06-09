---
source: "Ethereum Research"
source_type: research
title: "Trustless payments and relays"
author: ""
pub_date: "Mon, 08 Jun 2026 15:01:40 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-09
sources:
  - "https://ethresear.ch/t/trustless-payments-and-relays/25125"
---
# Trustless payments and relays

> 출처: [Ethereum Research](https://ethresear.ch/t/trustless-payments-and-relays/25125)  |  Mon, 08 Jun 2026 15:01:40 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** ePBS 도입이 프로토콜 내 무신뢰 결제 채널을 구축하여 블록 경매를 비공개 입찰 방식으로 변화시키고 기존 릴레이의 역할을 재조정할 것이라는 분석입니다.

**리서치 앵글:** ePBS로 인한 MEV 및 블록 구축 메커니즘의 변화는 당사 커버리지인 Lido의 검증인 수익 구조 및 MEV 분배 전략에 직접적인 영향을 미치므로 MEV 연구 테마와 깊이 연관되어 있습니다.

## 원문 미리보기
<p>TL;DR: <em>ePBS adds an in-protocol, sealed-by-default first-price channel for builder–proposer payments. We expect relays to survive, but the in-protocol channel reshapes what they can offer. We predict that trustless payments in-protocol will ossify a first-price block auction. Whether and how bids are shared publicly post-Glamsterdam is more subtle: the trustless payment channel generally pushes the block auction to a sealed-bid format, but there are scenarios where proposers may want to publicly share (possibly through a relay) bids they have received. Two factors matter: 1) how many “f