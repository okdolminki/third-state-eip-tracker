---
source: "Ethereum Research"
source_type: research
title: "A privacy pool on frame transactions: what works, and the case that does not yet"
author: ""
pub_date: "Fri, 06 Nov 2026 13:00:55 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-07
sources:
  - "https://ethresear.ch/t/a-privacy-pool-on-frame-transactions-what-works-and-the-case-that-does-not-yet/26223"
---
# A privacy pool on frame transactions: what works, and the case that does not yet

> 출처: [Ethereum Research](https://ethresear.ch/t/a-privacy-pool-on-frame-transactions-what-works-and-the-case-that-does-not-yet/26223)  |  Fri, 06 Nov 2026 13:00:55 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 이 연구는 프레임 트랜잭션과 EIP-8250을 활용한 프라이버시 풀 구현을 탐구하며, 릴레이어 없는 프라이빗 인출의 가능성을 보여주지만, 높은 증명 검증 가스 비용과 풀이 사용자 주소의 호출 비용을 지불할 수 없는 한계를 지적합니다.

**리서치 앵글:** 프레임 트랜잭션 기반 프라이버시 풀의 구현 가능성과 한계를 분석하여 기관 DeFi 도입을 위한 프라이버시 요구사항 및 계정 추상화(EIP-8250)의 기술적 과제를 탐구합니다.

## 원문 미리보기
<p><em>Daniil Ankushin, Nethermind. Verify-budget figures: method by Daniil Ankushin, benchmark and measurements by Manuel Arto.</em></p>
<p>On frame transactions a shielded pool pays its own gas, so a private withdrawal needs no relayer. We ran a real BN254 Groth16 pool this way on current Nethermind master: a withdrawal costs 679,322 gas. With EIP-8250 nonce keys, many withdrawals can come from the one pool address at once. Two things do not work yet. The proof check is over the spec cap on validation gas, and a pool cannot pay for a call from the user’s own address.</p>
<p>The pool we ran i