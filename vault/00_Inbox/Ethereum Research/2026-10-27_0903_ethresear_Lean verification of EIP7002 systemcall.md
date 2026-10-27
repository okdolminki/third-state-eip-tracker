---
source: "Ethereum Research"
source_type: research
title: "Lean verification of EIP-7002: system-call success and FIFO requests"
author: ""
pub_date: "Mon, 26 Oct 2026 16:46:40 +0000"

importance: high
action: read_now
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-10-27
sources:
  - "https://ethresear.ch/t/lean-verification-of-eip-7002-system-call-success-and-fifo-requests/26180"
---
# Lean verification of EIP-7002: system-call success and FIFO requests

> 출처: [Ethereum Research](https://ethresear.ch/t/lean-verification-of-eip-7002-system-call-success-and-fifo-requests/26180)  |  Mon, 26 Oct 2026 16:46:40 +0000

## AI 분석
**중요도:** high | **액션:** read_now

**요약:** EIP-7002의 검증자 출금 및 부분 인출 시스템 호출이 항상 성공함을 Lean 4를 통해 검증한 연구.

**리서치 앵글:** EIP-7002의 검증자 출금 메커니즘 검증은 LST/LRT 구조의 근간이 되는 이더리움 스테이킹 안정성과 직결됨.

## 원문 미리보기
<p>Since Prague, execution-layer requests for validator exits and partial withdrawals go through a 504-byte contract at <code>0x00000961Ef480Eb55e80D19ad83579A64c007002</code>, hand-written for the geas assembler. At the end of every block the protocol makes a system call to it, and that call is consensus-critical: <a href="https://eips.ethereum.org/EIPS/eip-7002#system-call" rel="noopener nofollow ugc">EIP-7002</a> requires a block whose call fails to be invalidated.</p>
<p>We proved two properties of the deployed runtime bytes in Lean 4:</p>
<ol>
<li><strong>The system call always succeeds,<