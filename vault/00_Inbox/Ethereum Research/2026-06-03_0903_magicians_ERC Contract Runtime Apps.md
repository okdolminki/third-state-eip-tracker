---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC: Contract Runtime Apps"
author: ""
pub_date: "Tue, 02 Jun 2026 15:37:43 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-03
sources:
  - "https://ethereum-magicians.org/t/erc-contract-runtime-apps/28685"
---
# ERC: Contract Runtime Apps

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-contract-runtime-apps/28685)  |  Tue, 02 Jun 2026 15:37:43 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 이 ERC는 스마트 컨트랙트가 서드파티 런타임 앱을 호스팅하기 위한 최소한의 인터페이스를 정의하며, 앱 실행은 호스트 컨텍스트 내에서 이루어져야 한다.

**리서치 앵글:** 이 ERC는 스마트 계정 내 서드파티 런타임 앱 호스팅을 위한 인터페이스를 정의하여 계정 추상화(EIP-7702)의 기능 확장 및 복잡한 로직 관리에 직접적인 영향을 미칠 수 있다.

## 원문 미리보기
<p>This ERC defines a minimal interface for smart contracts that host third-party runtime apps. A compliant host exposes local app enablement and a permissionless execution entry point for enabled apps.</p>
<p>Runtime app execution MUST occur in the host’s context rather than as a plain external call into app-owned state.</p>
<h2><a name="p-70536-motivation-1" class="anchor" href="https://ethereum-magicians.org#p-70536-motivation-1" aria-label="Heading link"></a>Motivation</h2>
<p>Smart contracts, especially smart accounts, increasingly host long-lived behavior such as inheritance rules, settl