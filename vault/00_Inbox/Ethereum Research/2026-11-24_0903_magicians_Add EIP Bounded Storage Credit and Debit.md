---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Add EIP: Bounded Storage Credit and Debit"
author: ""
pub_date: "Mon, 23 Nov 2026 12:15:21 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-24
sources:
  - "https://ethereum-magicians.org/t/add-eip-bounded-storage-credit-and-debit/30477"
---
# Add EIP: Bounded Storage Credit and Debit

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/add-eip-bounded-storage-credit-and-debit/30477)  |  Mon, 23 Nov 2026 12:15:21 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 스토리지 슬롯 값의 가감 연산을 상·하한선 범위 검증과 함께 원자적으로 수행하는 새로운 EVM 옵코드 SCREDIT 및 SDEBIT을 제안하는 EIP이다.

**리서치 앵글:** 토큰 잔액 갱신 등 DeFi 프로토콜 핵심 스토리지의 가스 비용 절감 및 병렬 실행 최적화 측면에서 중기적 모니터링이 유효하다.

## 원문 미리보기
<p>We propose <strong>Bounded Storage Credit and Debit</strong> (<a href="https://github.com/ethereum/EIPs/pull/12707" rel="noopener nofollow ugc">#12707</a>) as a successor to <a href="https://eips.ethereum.org/EIPS/eip-7519" rel="noopener nofollow ugc">EIP-7519</a>.</p>
<p><code>SCREDIT</code> adds an amount to a storage slot and <code>SDEBIT</code> subtracts an amount, each only if the slot’s value lies within a lower and an upper bound, given as operands, before and after the change. Both push a success flag, and neither pushes the slot’s value. A failed check leaves the slot unchanged and