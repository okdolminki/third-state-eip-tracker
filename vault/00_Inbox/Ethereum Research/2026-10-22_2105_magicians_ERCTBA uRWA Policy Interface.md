---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-TBA: uRWA Policy Interface"
author: ""
pub_date: "Thu, 22 Oct 2026 11:24:49 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-22
sources:
  - "https://ethereum-magicians.org/t/erc-tba-urwa-policy-interface/30048"
---
# ERC-TBA: uRWA Policy Interface

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-tba-urwa-policy-interface/30048)  |  Thu, 22 Oct 2026 11:24:49 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** ERC-7943(uRWA) 허가형 토큰의 컴플라이언스 로직을 외부 정책 컨트랙트와 연결하는 표준 인터페이스를 제안하여 규제 변화에 유연하게 대응합니다.

**리서치 앵글:** RWA 및 기관 DeFi 도입 시 필수적인 허가형 토큰의 컴플라이언스 정책 관리 방안과 관련됩니다.

## 원문 미리보기
<p>ERC-7943 (uRWA) standardised what a permissioned token exposes: <code>canSend</code>, <code>canReceive</code>, <code>canTransfer</code>, frozen balances and <code>forcedTransfer</code>. It deliberately left open how the token reaches those decisions. This proposal standardises that other half: the interface between an ERC-7943 token and an external policy contract.</p>
<h2><a name="p-75545-why-1" class="anchor" href="https://ethereum-magicians.org#p-75545-why-1" aria-label="Heading link"></a>Why</h2>
<ul>
<li><strong>Compliance logic changes faster than the token.</strong> Identity, jurisdi