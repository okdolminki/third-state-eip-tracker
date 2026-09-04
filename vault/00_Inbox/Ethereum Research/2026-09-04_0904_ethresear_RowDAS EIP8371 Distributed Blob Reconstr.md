---
source: "Ethereum Research"
source_type: research
title: "RowDAS (EIP-8371): Distributed Blob Reconstruction, measured"
author: ""
pub_date: "Thu, 03 Sep 2026 12:28:44 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-09-04
sources:
  - "https://ethresear.ch/t/rowdas-eip-8371-distributed-blob-reconstruction-measured/25897"
---
# RowDAS (EIP-8371): Distributed Blob Reconstruction, measured

> 출처: [Ethereum Research](https://ethresear.ch/t/rowdas-eip-8371-distributed-blob-reconstruction-measured/25897)  |  Thu, 03 Sep 2026 12:28:44 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EF 네트워킹 팀이 제안한 RowDAS(EIP-8371) 기반의 분산 블롭 재구성(Distributed Blob Reconstruction) 성능을 실측하고 분석한 연구이다.

**리서치 앵글:** 데이터 가용성 샘플링(PeerDAS/RowDAS) 고도화는 Arbitrum을 비롯한 L2의 Blob 수용량 확대 및 롤업 수수료 절감과 직결되는 L2 확장성 핵심 이슈이다.

## 원문 미리보기
<p><em>Note: this document is a result of a collaborative effort. It would not had been possible without the contribution and ideas of <a class="mention" href="https://ethresear.ch/u/marcopolo">@MarcoPolo</a> , <a class="mention" href="https://ethresear.ch/u/leobago">@leobago</a>, <a class="mention" href="https://ethresear.ch/u/kamilsa">@kamilsa</a> , <a class="mention" href="https://ethresear.ch/u/fradamt">@fradamt</a> , and the whole EF networking team.</em></p>
<p><strong>TL;DR</strong></p>
<ul>
<li>
<p><strong><a href="https://eips.ethereum.org/EIPS/eip-8371" rel="noopener nofollow ugc">Ro