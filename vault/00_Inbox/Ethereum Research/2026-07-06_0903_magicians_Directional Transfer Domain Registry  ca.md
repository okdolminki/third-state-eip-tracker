---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Directional Transfer Domain Registry - candidate ERC"
author: ""
pub_date: "Sun, 05 Jul 2026 21:32:04 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-06
sources:
  - "https://ethereum-magicians.org/t/directional-transfer-domain-registry-candidate-erc/28936"
---
# Directional Transfer Domain Registry - candidate ERC

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/directional-transfer-domain-registry-candidate-erc/28936)  |  Sun, 05 Jul 2026 21:32:04 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 토큰 종류와 무관하게 자산 클래스별로 불투명한 도메인 간의 전송 허용 여부를 등록하는 ERC 후보에 대한 피드백 요청.

**리서치 앵글:** RWA 및 기관 DeFi 도입을 위한 자산 전송 규제 및 컴플라이언스 프레임워크 구축에 기여할 수 있음.

## 원문 미리보기
<p>We would like feedback on a candidate ERC for a token-agnostic registry of directional transfer-route permissions between opaque domains by asset class.</p>
<p>Token standards and compliance modules commonly answer address-level or token-level questions. They do not provide a shared lookup surface for a separate policy question that can apply across many tokens:</p>
<blockquote>
<p>Is transfer from this source domain to this destination domain currently permitted for this asset class?</p>
</blockquote>
<p>A domain may represent a jurisdiction, regulated venue, enterprise network, game econo