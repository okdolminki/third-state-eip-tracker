---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Compose Whitepaper: A Composition Layer for On-Chain Applications"
author: ""
pub_date: "Wed, 08 Jul 2026 15:53:02 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-09
sources:
  - "https://ethereum-magicians.org/t/compose-whitepaper-a-composition-layer-for-on-chain-applications/28973"
---
# Compose Whitepaper: A Composition Layer for On-Chain Applications

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/compose-whitepaper-a-composition-layer-for-on-chain-applications/28973)  |  Wed, 08 Jul 2026 15:53:02 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** Compose는 온체인 애플리케이션을 위한 구성 레이어와 SCOP(Smart Contract Oriented Programming)를 도입하여 스마트 컨트랙트 코드 재사용을 촉진하고 중복 인프라로 인한 유지보수, 감사, 보안 부담을 줄이는 것을 목표로 한다.

**리서치 앵글:** 스마트 컨트랙트 재사용 및 구성 개선을 통해 L2 확장성 및 기관 DeFi 도입의 기반이 되는 온체인 애플리케이션의 보안과 효율성을 향상시킬 수 있음.

## 원문 미리보기
<h4><a name="p-71745-abstract-1" class="anchor" href="https://ethereum-magicians.org#p-71745-abstract-1" aria-label="Heading link"></a>Abstract</h4>
<p>The smart-contract ecosystem already depends heavily on code reuse, but that reuse has not yet become shared on-chain infrastructure. Similar logic is repeatedly redeployed across projects, creating duplicated infrastructure that increases long-term maintenance, audit, and security burdens for the ecosystem.</p>
<p><strong>Compose</strong> introduces <strong>Smart Contract Oriented Programming</strong>, or <strong>SCOP</strong>, to bring reuse 