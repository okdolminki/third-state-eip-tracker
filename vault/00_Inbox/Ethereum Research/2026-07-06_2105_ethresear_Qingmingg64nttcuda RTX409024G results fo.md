---
source: "Ethereum Research"
source_type: research
title: "Qingming-g64-ntt-cuda: RTX4090-24G results for native Goldilocks/G64 STARK-LDE NTT"
author: ""
pub_date: "Mon, 06 Jul 2026 11:56:25 +0000"

importance: medium
action: weekly_review
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-07-06
sources:
  - "https://ethresear.ch/t/qingming-g64-ntt-cuda-rtx4090-24g-results-for-native-goldilocks-g64-stark-lde-ntt/25373"
---
# Qingming-g64-ntt-cuda: RTX4090-24G results for native Goldilocks/G64 STARK-LDE NTT

> 출처: [Ethereum Research](https://ethresear.ch/t/qingming-g64-ntt-cuda-rtx4090-24g-results-for-native-goldilocks-g64-stark-lde-ntt/25373)  |  Mon, 06 Jul 2026 11:56:25 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review

**요약:** RTX4090-24G GPU에서 Goldilocks/G64 STARK-LDE NTT의 CUDA 성능 측정 결과를 보고하는 리포트가 공개되었습니다.

**리서치 앵글:** ZK-STARK 성능 최적화는 L2 확장성 연구 테마와 직접적으로 연관됩니다.

## 원문 미리보기
<p>I am releasing a CUDA / RTX4090-24G result report for native Goldilocks/G64 STARK-LDE NTT.</p>
<p>Repository:</p>
<pre><code class="lang-auto">https://github.com/uulong950/qingming-g64-ntt-cuda
</code></pre>
<p>This is the CUDA-side follow-up to my previous <code>qingming-g64-ntt</code> work on AMD HIP / ROCm.</p>
<p>The purpose of this release is to report reproducible RTX4090-24G results with clear interface definitions, validation checks, and supported-size boundaries.</p>
<h2><a name="p-61103-status-1" class="anchor" href="https://ethresear.ch#p-61103-status-1"></a>Status</h2>
<pre><cod