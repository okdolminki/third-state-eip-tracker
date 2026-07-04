---
source: "Ethereum Research"
source_type: research
title: "Qingming-g64-ntt: Native Goldilocks/G64 GPU NTT at 2^27 on RX 7900 XTX, and a reproducible benchmark plan"
author: ""
pub_date: "Sat, 04 Jul 2026 09:09:32 +0000"

importance: medium
action: weekly_review
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-07-04
sources:
  - "https://ethresear.ch/t/qingming-g64-ntt-native-goldilocks-g64-gpu-ntt-at-2-27-on-rx-7900-xtx-and-a-reproducible-benchmark-plan/25359"
---
# Qingming-g64-ntt: Native Goldilocks/G64 GPU NTT at 2^27 on RX 7900 XTX, and a reproducible benchmark plan

> 출처: [Ethereum Research](https://ethresear.ch/t/qingming-g64-ntt-native-goldilocks-g64-gpu-ntt-at-2-27-on-rx-7900-xtx-and-a-reproducible-benchmark-plan/25359)  |  Sat, 04 Jul 2026 09:09:32 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review

**요약:** STARK-LDE 워크로드를 위한 Goldilocks/G64 GPU NTT 구현을 공유하고 벤치마크 방법론에 대한 피드백을 요청하는 글입니다.

**리서치 앵글:** L2 확장성: STARK 기반 L2의 성능 향상 및 벤치마크 표준화에 기여할 수 있는 GPU NTT 구현 연구.

## 원문 미리보기
<p>I would like to share an open-source native Goldilocks/G64 GPU NTT implementation and ask for feedback on benchmark methodology for STARK-LDE workloads.</p>
<p>I am the author of <code>qingming-g64-ntt</code>, an original AMD HIP / ROCm implementation of native Goldilocks-field NTT for a STARK-style LDE workload. The goal of this post is not to claim a universal “fastest NTT”, but to make native G64 GPU NTT results more reproducible, better specified, and easier to compare across open implementations.</p>
<p>Repository: [<a href="https://github.com/uulong950/qingming-g64-ntt%5C" rel="noopen