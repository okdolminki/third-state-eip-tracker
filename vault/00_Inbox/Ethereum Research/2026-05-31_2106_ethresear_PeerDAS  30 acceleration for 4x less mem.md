---
source: "Ethereum Research"
source_type: research
title: "PeerDAS - 30% acceleration for 4x less memory usage"
author: ""
pub_date: "Wed, 27 May 2026 15:47:27 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-05-31
sources:
  - "https://ethresear.ch/t/peerdas-30-acceleration-for-4x-less-memory-usage/24978"
---
# PeerDAS - 30% acceleration for 4x less memory usage

> 출처: [Ethereum Research](https://ethresear.ch/t/peerdas-30-acceleration-for-4x-less-memory-usage/24978)  |  Wed, 27 May 2026 15:47:27 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** PeerDAS는 c-kzg-4844 대비 30% 성능 향상과 4배 적은 메모리 사용으로 리소스 제약 장치에 큰 도움을 줄 수 있음을 보여주는 이더리움 재단 지원 연구 결과입니다.

**리서치 앵글:** PeerDAS의 성능 및 메모리 효율성 개선은 이더리움 L2 확장성 및 데이터 가용성 계층의 효율성을 직접적으로 향상시킵니다.

## 원문 미리보기
<p>Following a grant from the Ethereum Foundation I have recently added PeerDAS support to Constantine.</p>
<p>With careful engineering combined with state-of-the-art research, I managed to get a 30% acceleration over c-kzg-4844 while using 4x less memory for precomputation tables (and more memory → more acceleration), this should significantly help resource-constrained devices</p>
<div class="md-table">
<table>
<thead>
<tr>
<th style="text-align:left">Benchmark</th>
<th style="text-align:left">Precompute</th>
<th style="text-align:center">c-kzg-4844 (serial)</th>
<th style="text-align:center"