---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-XXXX: Parametric Token"
author: ""
pub_date: "Mon, 10 Aug 2026 16:56:32 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-11
sources:
  - "https://ethereum-magicians.org/t/erc-xxxx-parametric-token/29385"
---
# ERC-XXXX: Parametric Token

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-xxxx-parametric-token/29385)  |  Mon, 10 Aug 2026 16:56:32 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** DeFi의 유동성과 유틸리티 간의 상충 관계를 해결하기 위해, 계정별 파라미터를 가질 수 있으면서도 토큰의 대체 가능성을 유지하는 새로운 ERC-20 호환 'Parametric Token' 표준이 제안되었습니다.

**리서치 앵글:** 토큰의 유동성과 유틸리티 개선을 통해 기관 DeFi 도입 및 계정 추상화(EIP-7702) 관련 연구에 시사점을 제공합니다.

## 원문 미리보기
<p>Hi everyone,</p>
<p>DeFi today faces a trade‑off: you can have liquidity, or you can have utility. Tokens that are highly liquid (like ERC‑20) carry no state - they are just balances. Tokens that carry state (like ERC‑721 or ERC‑1155) fragment liquidity because each variant is a separate class. Respectively, agents and structured products cannot easily build on either without choosing between the two.</p>
<p>I’d like to propose a new ERC-20 compatible solution: Parametric Token. It keeps tokens fungible while allowing each account to hold its own set of parameters. The parameter travels wit