---
source: "Ethereum Research"
source_type: research
title: "Ashlar: an AO hash from a squaring degree engine, and a request for cryptanalysis"
author: ""
pub_date: "Thu, 06 Aug 2026 07:57:13 +0000"

importance: high
action: read_now
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-08-06
sources:
  - "https://ethresear.ch/t/ashlar-an-ao-hash-from-a-squaring-degree-engine-and-a-request-for-cryptanalysis/25634"
---
# Ashlar: an AO hash from a squaring degree engine, and a request for cryptanalysis

> 출처: [Ethereum Research](https://ethresear.ch/t/ashlar-an-ao-hash-from-a-squaring-degree-engine-and-a-request-for-cryptanalysis/25634)  |  Thu, 06 Aug 2026 07:57:13 +0000

## AI 분석
**중요도:** high | **액션:** read_now

**요약:** 새로운 산술 지향 해시 함수 Ashlar는 필드 제곱을 기반으로 하며, 기존 Poseidon 계열 해시보다 R1CS 제약 조건과 EVM 가스 비용 면에서 더 효율적이다.

**리서치 앵글:** L2 확장성 및 계정 추상화의 핵심 기반 기술인 ZK-SNARK 효율성 개선에 기여.

## 원문 미리보기
<p><strong>TL;DR.</strong> I have a new arithmetization-oriented hash, <strong>Ashlar</strong>, built around a different degree engine: a Feistel chain of field <em>squarings</em> instead of a power map. Under the accounting metric that the FreeLunch-era attacks make natural — bits of CICO ideal degree per R1CS constraint — squaring buys 1.0 and I prove 1.0 is a ceiling. The width-3 BN254 hash costs <strong>191 measured R1CS constraints</strong> against derived counts of 243 for Poseidon and 240 for Poseidon2, and <strong>14,232 EVM gas</strong> against Poseidon’s measured 18,229. It also lose