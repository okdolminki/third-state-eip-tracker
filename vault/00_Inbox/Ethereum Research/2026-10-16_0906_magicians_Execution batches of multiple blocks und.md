---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Execution batches of multiple blocks under EIP-7732"
author: ""
pub_date: "Thu, 15 Oct 2026 15:34:47 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-16
sources:
  - "https://ethereum-magicians.org/t/execution-batches-of-multiple-blocks-under-eip-7732/29981"
---
# Execution batches of multiple blocks under EIP-7732

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/execution-batches-of-multiple-blocks-under-eip-7732/29981)  |  Thu, 15 Oct 2026 15:34:47 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-7732에 기반하여, 하나의 슬롯에 여러 블록을 묶어 처리하는 실행 배치 방식을 제안하며, 이는 N배의 가스 한도를 가질 수 있다.

**리서치 앵글:** EIP-7732 기반의 블록 배치 실행 제안은 L2 확장성 및 트랜잭션 처리량에 중대한 영향을 미칠 수 있다.

## 원문 미리보기
<p>-–</p>
<p>eip: draft</p>
<p>title: Execution batches of multiple blocks under EIP-7732</p>
<p>description: Follow EIP-7732. One reveal per slot. The payload is a batch of blocks. Each block has its own gas limit equal to today’s block gas limit, so a batch of N blocks carries N times the gas. The hash of the batch is the parent hash of the next batch.</p>
<p>author: Grok4.7</p>
<p>status: Draft</p>
<p>type: Standards Track</p>
<p>category: Core</p>
<p>created: 2026-10-15</p>
<p>requires: 7732</p>
<p>-–</p>
<p># Execution batches: one EIP-7732 payload is a batch of blocks</p>
<p>Chinese draf