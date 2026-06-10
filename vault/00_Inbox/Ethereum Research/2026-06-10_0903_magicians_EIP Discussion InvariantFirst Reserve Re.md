---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP Discussion: Invariant-First Reserve Receipt Token (IFR-pETH)"
author: ""
pub_date: "Tue, 09 Jun 2026 20:30:09 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-10
sources:
  - "https://ethereum-magicians.org/t/eip-discussion-invariant-first-reserve-receipt-token-ifr-peth/28753"
---
# EIP Discussion: Invariant-First Reserve Receipt Token (IFR-pETH)

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-discussion-invariant-first-reserve-receipt-token-ifr-peth/28753)  |  Tue, 09 Jun 2026 20:30:09 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 외부 오프체인 증명 없이 트랜잭션 실행 단계에서 솔벤시(지급 능력)를 수학적 불변식으로 강제하는 ERC-20 호환 예치 자산 담보 토큰(IFR) 표준에 대한 제안입니다.

**리서치 앵글:** Lido, Ether.fi와 같은 LST/LRT 프로토콜 및 Ondo, Maple 등 RWA 프로토콜이 발행하는 예치 자산 담보 토큰의 온체인 솔벤시 검증 및 리스크 관리 프레임워크에 직접적인 영향을 미칠 수 있습니다.

## 원문 미리보기
<p>This thread is the discussion venue for a proposed EIP defining the<br>
Invariant-First Reserve Receipt Token (IFR) standard.</p>
<h2><a name="p-70748-summary-1" class="anchor" href="https://ethereum-magicians.org#p-70748-summary-1" aria-label="Heading link"></a>Summary</h2>
<p>IFR is an ERC-20-compatible primitive for reserve-backed tokens that<br>
enforces solvency as a transaction-validity condition rather than an<br>
external proof-of-reserves report.</p>
<p>Every state transition preserves:</p>
<p>T + F == R address(this).balance &gt;= R</p>
<p>Where:</p>
<ul>
<li>R = accounted reserve