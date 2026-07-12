---
source: "Ethereum Research"
source_type: research
title: "Sybil Attacks on AUCIL"
author: ""
pub_date: "Sun, 12 Jul 2026 03:28:26 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-12
sources:
  - "https://ethresear.ch/t/sybil-attacks-on-aucil/25447"
---
# Sybil Attacks on AUCIL

> 출처: [Ethereum Research](https://ethresear.ch/t/sybil-attacks-on-aucil/25447)  |  Sun, 12 Jul 2026 03:28:26 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 이더리움 PBS 환경에서 검열 저항을 위한 인클루전 리스트(ILs) 디자인(FOCIL, AUCIL)과 AUCIL에 대한 시빌 공격 가능성을 다룬 연구.

**리서치 앵글:** MEV 및 이더리움의 검열 저항성 강화 방안과 관련된 연구로, 모든 DeFi 프로토콜의 기반 인프라에 영향을 미침.

## 원문 미리보기
<p>Inclusion lists (ILs) are the talk of the town as a censorship resistance primitive for Ethereum under proposer builder separation (PBS). Two major designs have been developed as per my understanding:</p>
<ol>
<li>
<p><strong>FOCIL</strong>, which relies on underlying consensus with fixed slot wise participants and no explicit pricing, and</p>
</li>
<li>
<p><strong>AUCIL</strong>, which is an auction based inclusion list design that relies on economic incentives with strategic participation and price formation.</p>
</li>
</ol>
<p>With FOCIL (EIP-7805) proposed to headline the forthcoming He