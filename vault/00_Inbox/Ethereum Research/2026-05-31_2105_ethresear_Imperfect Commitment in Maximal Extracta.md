---
source: "Ethereum Research"
source_type: research
title: "Imperfect Commitment in Maximal Extractable Value Auctions"
author: ""
pub_date: "Fri, 29 May 2026 14:50:27 +0000"

importance: high
action: read_now
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-05-31
sources:
  - "https://ethresear.ch/t/imperfect-commitment-in-maximal-extractable-value-auctions/25001"
---
# Imperfect Commitment in Maximal Extractable Value Auctions

> 출처: [Ethereum Research](https://ethresear.ch/t/imperfect-commitment-in-maximal-extractable-value-auctions/25001)  |  Fri, 29 May 2026 14:50:27 +0000

## AI 분석
**중요도:** high | **액션:** read_now

**요약:** 본 논문은 형식적으로 최적화된 MEV 경매조차도 빌더가 제출된 입찰 및 페이로드를 관찰한 후 이탈하여 승리 기회를 복제함으로써 훼손될 수 있음을 연구한다.

**리서치 앵글:** MEV 경매에서 빌더의 이탈 행위가 경매의 효율성과 공정성에 미치는 영향을 분석하여 Third State의 MEV 리서치 테마와 직접적으로 연관된다.

## 원문 미리보기
<p>This paper is a companion to <a href="https://ethresear.ch/t/open-vs-sealed-auction-format-choice-for-maximal-extractable-value/24454">Open vs. Sealed: Auction Format Choice for MEV</a> and studies a distinct but related problem: even a format-optimal auction can be undermined by builder defection ex post. We model a builder who, after observing submitted bids and payloads, defects from the honest auction outcome with probability <span class="math">\varepsilon</span> and replicates a type-specific fraction <span class="math">\gamma(\tau)</span> of the winning opportunity. Searchers respond 