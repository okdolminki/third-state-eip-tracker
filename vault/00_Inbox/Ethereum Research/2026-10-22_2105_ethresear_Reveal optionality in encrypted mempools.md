---
source: "Ethereum Research"
source_type: research
title: "Reveal optionality in encrypted mempools: how big is the sender’s free option, and a post-quantum way to remove it"
author: ""
pub_date: "Thu, 22 Oct 2026 05:07:16 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-22
sources:
  - "https://ethresear.ch/t/reveal-optionality-in-encrypted-mempools-how-big-is-the-sender-s-free-option-and-a-post-quantum-way-to-remove-it/26169"
---
# Reveal optionality in encrypted mempools: how big is the sender’s free option, and a post-quantum way to remove it

> 출처: [Ethereum Research](https://ethresear.ch/t/reveal-optionality-in-encrypted-mempools-how-big-is-the-sender-s-free-option-and-a-post-quantum-way-to-remove-it/26169)  |  Thu, 22 Oct 2026 05:07:16 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 암호화된 멤풀에서 발신자의 '자유 옵션' 가치를 분석하고, 이를 제거하기 위한 양자 내성 방안을 탐구하는 연구입니다.

**리서치 앵글:** 이더리움의 MEV 문제와 L2 확장성에 영향을 미치는 암호화된 멤풀 및 트랜잭션 순서화 메커니즘에 대한 연구입니다.

## 원문 미리보기
<p>Hi all,</p>
<p>Thanks to <a class="mention" href="https://ethresear.ch/u/aelowsson">@aelowsson</a> <a class="mention" href="https://ethresear.ch/u/julian">@julian</a> <a class="mention" href="https://ethresear.ch/u/b-wagn">@b-wagn</a> <a class="mention" href="https://ethresear.ch/u/gottfriedherold">@GottfriedHerold</a>, since this builds directly on LUCID and the criticism thread. Also a kind request for review on this work.</p>
<p>I’ve been wondering how much the “free option” in encrypted mempools is actually worth, and what happens if you try to take it away. The short version is in the 