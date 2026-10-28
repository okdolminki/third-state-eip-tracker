---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8455: RESERVOIR Opcode"
author: ""
pub_date: "Wed, 28 Oct 2026 09:17:58 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-28
sources:
  - "https://ethereum-magicians.org/t/eip-8455-reservoir-opcode/30116"
---
# EIP-8455: RESERVOIR Opcode

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8455-reservoir-opcode/30116)  |  Wed, 28 Oct 2026 09:17:58 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8455는 EIP-8037의 가스 분리(실행 가스 및 상태 가스) 및 EIP-8141의 프레임 트랜잭션 개념을 확장하는 RESERVOIR Opcode에 대한 논의입니다.

**리서치 앵글:** 가스 비용 구조 변경을 통해 L2 확장성 및 계정 추상화의 효율성에 영향을 미칠 수 있습니다.

## 원문 미리보기
<p>Discussion topic <a href="https://eips.ethereum.org/EIPS/eip-8455" rel="noopener nofollow ugc">EIP-8455</a></p>
<h2><a name="p-75809-summary-1" class="anchor" href="https://ethereum-magicians.org#p-75809-summary-1" aria-label="Heading link"></a>Summary</h2>
<p><a href="https://eips.ethereum.org/EIPS/eip-8037" rel="noopener nofollow ugc">EIP-8037</a> splits gas into execution gas and state gas, and lets state gas be paid from a reservoir that <code>GAS</code> does not report. <a href="https://eips.ethereum.org/EIPS/eip-8141" rel="noopener nofollow ugc">EIP-8141</a> frame transactions have a 