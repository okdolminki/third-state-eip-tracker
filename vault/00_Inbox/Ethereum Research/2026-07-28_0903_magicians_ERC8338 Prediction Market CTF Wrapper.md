---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8338: Prediction Market CTF Wrapper"
author: ""
pub_date: "Mon, 27 Jul 2026 14:29:28 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-28
sources:
  - "https://ethereum-magicians.org/t/erc-8338-prediction-market-ctf-wrapper/29106"
---
# ERC-8338: Prediction Market CTF Wrapper

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8338-prediction-market-ctf-wrapper/29106)  |  Mon, 27 Jul 2026 14:29:28 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 이 제안은 조건부 토큰 프레임워크(CTF) 포지션(ERC-1155 예측 시장 결과 지분)을 ERC-20 토큰으로 표준화하는 것을 목표로 합니다.

**리서치 앵글:** DeFi 자산의 표준화 및 상호운용성 개선에 기여하여 DeFi 생태계 확장에 영향을 줄 수 있습니다.

## 원문 미리보기
<h2><a name="p-72158-abstract-1" class="anchor" href="https://ethereum-magicians.org#p-72158-abstract-1" aria-label="Heading link"></a>Abstract</h2>
<p>This proposal standardizes the representation of Conditional Tokens Framework (CTF) positions — <a>ERC-1155</a> prediction-market outcome shares — as <a>ERC-20</a> tokens.</p>
<p>Two interfaces are defined. A contract conforming to <code>ICTFWrapper</code> is an ERC-20 token that wraps a single CTF position one-to-one, exposing <code>wrap</code>, <code>unwrap</code>, and a pointer to its factory. A contract conforming to <code>ICTFWrapperFactor