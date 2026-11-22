---
source: "Ethereum Research"
source_type: research
title: "What's a block, and how big can it get?"
author: ""
pub_date: "Sun, 22 Nov 2026 08:32:10 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-22
sources:
  - "https://ethresear.ch/t/whats-a-block-and-how-big-can-it-get/26281"
---
# What's a block, and how big can it get?

> 출처: [Ethereum Research](https://ethresear.ch/t/whats-a-block-and-how-big-can-it-get/26281)  |  Sun, 22 Nov 2026 08:32:10 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** Glamsterdam 하드포크 이후 이더리움 블록 크기 및 가스 한도의 최악의 시나리오와 그 영향에 대한 연구.

**리서치 앵글:** Glamsterdam 하드포크 이후 블록 크기 및 가스 변화가 L2 확장성에 미칠 영향 분석.

## 원문 미리보기
<h1><a name="p-63088-whats-a-block-and-how-big-can-it-get-1" class="anchor" href="https://ethresear.ch#p-63088-whats-a-block-and-how-big-can-it-get-1" aria-label="Heading link"></a>What’s a block, and how big can it get?</h1>
<p><em>Worst-case block size after <a href="https://eips.ethereum.org/EIPS/eip-7773">Glamsterdam</a>, why it matters for <a href="https://eips.ethereum.org/EIPS/eip-7805">FOCIL</a>, and what to make from block sizes and gas.</em></p>
<blockquote>
<p>All numbers here use Glamsterdam rules, with a 60M gas limit as the reference point.</p>
</blockquote>
<h2><a name="p-63088-