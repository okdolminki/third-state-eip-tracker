---
source: "Ethereum Research"
source_type: research
title: "Same instruction count, 23x the wall clock: working-set effects in a deterministic RISC-V interpreter"
author: ""
pub_date: "Sun, 30 Aug 2026 03:30:44 +0000"

importance: medium
action: weekly_review
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-08-30
sources:
  - "https://ethresear.ch/t/same-instruction-count-23x-the-wall-clock-working-set-effects-in-a-deterministic-risc-v-interpreter/25856"
---
# Same instruction count, 23x the wall clock: working-set effects in a deterministic RISC-V interpreter

> 출처: [Ethereum Research](https://ethresear.ch/t/same-instruction-count-23x-the-wall-clock-working-set-effects-in-a-deterministic-risc-v-interpreter/25856)  |  Sun, 30 Aug 2026 03:30:44 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review

**요약:** 결정론적 RISC-V 인터프리터에서 프로토콜 수준의 실행 예산 책정을 위해 실행 비용을 측정했으며, 스텝 수와 실제 시간 간의 예상보다 느슨한 관계를 발견했다.

**리서치 앵글:** 결정론적 RISC-V 인터프리터의 실행 비용 측정은 L2 확장성 및 효율적인 프로토콜 운영에 대한 이해를 심화시킨다.

## 원문 미리보기
<p>I’ve been measuring execution cost in a deterministic RISC-V interpreter,</p>
<p>motivated by a narrow problem: assigning a protocol-level execution budget that</p>
<p>stays safe across heterogeneous machines. The budget is denominated in steps,</p>
<p>and the question I set out to answer is how tightly a step count bounds wall</p>
<p>clock. The answer I got is looser than I expected, so I’m posting the</p>
<p>measurements rather than a proposal.</p>
<p><strong>**Terminology, because this is the part that will otherwise be misread.**</strong> A</p>
<p><em>*step*</em> is one RV32IM instructi