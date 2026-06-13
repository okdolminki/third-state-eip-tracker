---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8298: SETCODEFROM Code Reuse Instruction"
author: ""
pub_date: "Fri, 12 Jun 2026 15:10:51 +0000"

importance: high
action: read_now
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-06-13
sources:
  - "https://ethereum-magicians.org/t/eip-8298-setcodefrom-code-reuse-instruction/28779"
---
# EIP-8298: SETCODEFROM Code Reuse Instruction

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8298-setcodefrom-code-reuse-instruction/28779)  |  Fri, 12 Jun 2026 15:10:51 +0000

## AI 분석
**중요도:** high | **액션:** read_now

**요약:** EIP-8298은 기존 컨트랙트의 코드를 재사용하여 배포 비용을 절감하는 새로운 EVM 명령어 `SETCODEFROM`을 제안합니다.

**리서치 앵글:** L2 확장성 및 DeFi 프로토콜의 배포 효율성 개선에 기여할 수 있는 EVM 변경 사항입니다.

## 원문 미리보기
<p>This proposal comes from an idea raised during an ACDE call: combine the goals of EIP-7851 and EIP-8058 into one lower-level code adoption primitive.</p>
<p>EIP-8298 introduces <code>SETCODEFROM</code>, an EVM instruction that lets the current account adopt the code hash of an existing deployed contract. The source is a live account address, rather than a raw code hash, so the adopted code is tied to the current consensus state.</p>
<p>The proposal has two main uses:</p>
<ul>
<li>Contract bytecode reuse and deployment economics: this addresses the deployment-cost problem targeted by EIP-805