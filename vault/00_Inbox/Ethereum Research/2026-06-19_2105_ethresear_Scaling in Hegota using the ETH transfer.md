---
source: "Ethereum Research"
source_type: research
title: "Scaling in Hegota: using the ETH transfer to anchor execution and bandwidth"
author: ""
pub_date: "Fri, 19 Jun 2026 08:19:35 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-19
sources:
  - "https://ethresear.ch/t/scaling-in-hegota-using-the-eth-transfer-to-anchor-execution-and-bandwidth/25232"
---
# Scaling in Hegota: using the ETH transfer to anchor execution and bandwidth

> 출처: [Ethereum Research](https://ethresear.ch/t/scaling-in-hegota-using-the-eth-transfer-to-anchor-execution-and-bandwidth/25232)  |  Fri, 19 Jun 2026 08:19:35 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 이더리움의 가스 한도 확장을 위해 ETH 전송의 21,000 가스 비용이 실행 및 대역폭의 두 가지 측면을 모두 제한한다는 점을 활용하는 방안을 모색합니다.

**리서치 앵글:** 이더리움의 가스 한도 확장 논의는 L2 확장성 테마와 직접적으로 연관됩니다.

## 원문 미리보기
<blockquote>
<p>I would like to thank Toni Wahrstaetter, Marius Vanderwijden and Parithosh Jayanthi for the discussion that led to this report</p>
</blockquote>
<p>This post works out what Hegota needs to change to keep scaling the gas limit after Glamsterdam. The starting point is a single observation: the 21,000-gas ETH transfer bounds <em>both</em> dimensions of the slot.</p>
<ul>
<li>On the execution side, the Glamsterdam repricings pushed costs as far as the transfer cap permits, fixing worst-case execution at 100 Mgas/s.</li>
<li>On the bandwidth side, a block full of transfers is itself