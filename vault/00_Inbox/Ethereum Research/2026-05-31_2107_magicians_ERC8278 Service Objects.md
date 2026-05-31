---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8278: Service Objects"
author: ""
pub_date: "Thu, 28 May 2026 23:51:31 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-05-31
sources:
  - "https://ethereum-magicians.org/t/erc-8278-service-objects/28659"
---
# ERC-8278: Service Objects

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8278-service-objects/28659)  |  Thu, 28 May 2026 23:51:31 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 이 제안은 오프체인 서비스 제어를 나타내는 양도 가능한 토큰인 서비스 객체를 위한 최소한의 ERC-721 호환 인터페이스를 정의합니다.

**리서치 앵글:** 오프체인 서비스 제어를 토큰화하여 기관 DeFi 도입 및 L2 확장성 측면에서 활용될 가능성을 분석합니다.

## 원문 미리보기
<p>I’d like feedback on a small ERC-721 extension for service objects.</p>
<p>Abstract</p>
<p>This proposal defines a minimal ERC-721-compatible interface for service objects. A service object is a transferable token that represents control over an offchain service. The interface exposes a service manifest, service operator, and payment route so that wallets, indexers, marketplaces, and clients can resolve the current operational state of a service before interacting with it.</p>
<p>The proposal does not define service discovery, reputation, execution, payment settlement, smart-account behavio