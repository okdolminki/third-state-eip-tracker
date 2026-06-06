---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8283: On-Chain Registry for ERC-7730 Clear Signing Descriptors"
author: ""
pub_date: "Fri, 05 Jun 2026 14:37:31 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-06
sources:
  - "https://ethereum-magicians.org/t/erc-8283-on-chain-registry-for-erc-7730-clear-signing-descriptors/28717"
---
# ERC-8283: On-Chain Registry for ERC-7730 Clear Signing Descriptors

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8283-on-chain-registry-for-erc-7730-clear-signing-descriptors/28717)  |  Fri, 05 Jun 2026 14:37:31 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** ERC-7730이 해결하지 못한 블라인드 사이닝 디스크립터의 온체인 레지스트리, 신뢰 네트워크, 장기 저장 메커니즘 부재 문제를 ERC-8283이 제안한다.

**리서치 앵글:** 블라인드 사이닝 문제 해결을 통한 기관 DeFi 도입 촉진 및 계정 추상화(EIP-7702) 관련 사용자 경험 개선.

## 원문 미리보기
<p>ERC-7730 is a wonderful standard that finally addresses the issue of blind signing, a huge problem that has not been addressed properly for many years and has lead to large financial loses and loads of stress literally for everyone who has ever interacted with smart contracts on Ethereum.</p>
<p>However, ERC-7730 does not specify a mechanism for the Ethereum community to permissionlessly maintain and update the registry of the Clear Signing descriptors, to establish a network of trust between the creators and consumers of these descriptors, and does not address the long-term storage and ret