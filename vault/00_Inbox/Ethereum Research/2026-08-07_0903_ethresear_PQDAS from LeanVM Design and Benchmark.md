---
source: "Ethereum Research"
source_type: research
title: "PQ-DAS from LeanVM: Design and Benchmark"
author: ""
pub_date: "Thu, 06 Aug 2026 14:32:28 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-07
sources:
  - "https://ethresear.ch/t/pq-das-from-leanvm-design-and-benchmark/25642"
---
# PQ-DAS from LeanVM: Design and Benchmark

> 출처: [Ethereum Research](https://ethresear.ch/t/pq-das-from-leanvm-design-and-benchmark/25642)  |  Thu, 06 Aug 2026 14:32:28 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 양자 컴퓨팅 시대에 대비해 LeanVM 기반의 양자 내성 데이터 가용성 샘플링(PQ-DAS) 구조를 설계하고 벤치마킹하여 블롭 데이터 검증 성능을 평가한 연구입니다.

**리서치 앵글:** L2 확장성의 핵심인 데이터 가용성(DA) 레이어의 장기적인 양자 내성 보안 및 효율성 개선과 연관되어 있습니다.

## 원문 미리보기
<p><em>Authors.</em> Long Meng, Benedikt Wagner, George Kadianakis, Francesco Risitano</p>
<p><em>Thanks to Tom Wambsgans, Thomas Coratger, Arantxa Zapico, and others for insightful discussions</em>.</p>
<h2><a name="p-61753-h-1-motivation-1" class="anchor" href="https://ethresear.ch#p-61753-h-1-motivation-1"></a>1. Motivation</h2>
<p>Ethereum uses data availability sampling (DAS) to let validators check the availability of large blob data by sampling a small number of random positions from an erasure-coded object, rather than downloading the whole payload. As Ethereum moves toward post-quantu