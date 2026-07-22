---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-XXXX: Cento Proxy – Index-Based Multi-Facet Proxy"
author: ""
pub_date: "Tue, 21 Jul 2026 19:30:42 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-22
sources:
  - "https://ethereum-magicians.org/t/erc-xxxx-cento-proxy-index-based-multi-facet-proxy/29054"
---
# ERC-XXXX: Cento Proxy – Index-Based Multi-Facet Proxy

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-xxxx-cento-proxy-index-based-multi-facet-proxy/29054)  |  Tue, 21 Jul 2026 19:30:42 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 새로운 ERC-XXXX 제안인 Cento Proxy는 ERC-2535와 같은 기존 모듈형 프록시 아키텍처를 기반으로 하는 인덱스 기반 다면 프록시 표준을 다룹니다.

**리서치 앵글:** 스마트 컨트랙트 모듈화 및 업그레이드 가능성 개선을 통해 L2 확장성 및 계정 추상화(EIP-7702) 구현에 영향을 미칠 수 있습니다.

## 원문 미리보기
<h2><a name="p-72001-motivation-1" class="anchor" href="https://ethereum-magicians.org#p-72001-motivation-1" aria-label="Heading link"></a>Motivation</h2>
<p>Over the past several years, the Ethereum ecosystem has shown sustained interest in modular proxy architectures. <a href="https://eips.ethereum.org/EIPS/eip-2535" rel="noopener nofollow ugc">ERC-2535</a> (Diamonds) established the first widely adopted standard, and subsequent proposals such as <a href="https://eips.ethereum.org/EIPS/eip-8109" rel="noopener nofollow ugc">ERC-8109</a> and <a href="https://eips.ethereum.org/EIPS/eip-8153" re