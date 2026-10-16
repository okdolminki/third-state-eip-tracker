---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8442: 64-bit Opcodes for the EVM"
author: ""
pub_date: "Thu, 15 Oct 2026 22:25:30 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-16
sources:
  - "https://ethereum-magicians.org/t/eip-8442-64-bit-opcodes-for-the-evm/29982"
---
# EIP-8442: 64-bit Opcodes for the EVM

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8442-64-bit-opcodes-for-the-evm/29982)  |  Thu, 15 Oct 2026 22:25:30 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8442는 EVM의 256비트 연산 비용을 줄이기 위해 64비트 연산을 위한 새로운 28개 명령어 세트를 도입하여 효율성을 높이는 것을 제안합니다.

**리서치 앵글:** EVM의 연산 효율성 개선은 L2 확장성 향상 및 전반적인 DeFi 프로토콜의 가스 비용 절감에 기여할 수 있습니다.

## 원문 미리보기
<p><a href="https://eips.ethereum.org/EIPS/eip-8442">EIP-8442: 64-bit Opcodes for the EVM</a></p>
<p>Not every computation needs 256 bits.  Counters, offsets, lengths, and the inner loops of hashes and big-number arithmetic fit in 64, and the EVM makes them pay for 256 at every step.  This proposal adds twenty-eight instructions that compute on the low 64 bits of their operands: the EVM64 instruction set of <a href="https://eips.ethereum.org/EIPS/eip-7937">EIP-7937</a> — the same operations at the same costs — encoded as ordinary single-byte opcodes rather than behind a prefix byte.  Each is t