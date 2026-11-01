---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Pre-ERC: Agent Pre-Sign Risk Report"
author: ""
pub_date: "Sat, 31 Oct 2026 13:56:39 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-01
sources:
  - "https://ethereum-magicians.org/t/pre-erc-agent-pre-sign-risk-report/30145"
---
# Pre-ERC: Agent Pre-Sign Risk Report

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/pre-erc-agent-pre-sign-risk-report/30145)  |  Sat, 31 Oct 2026 13:56:39 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 자율형 AI 에이전트의 트랜잭션 자동 서명 시 발생하는 무제한 승인, 가짜 토큰 매수, 주소 포이즈닝 등의 리스크를 사전 탐지·보고하기 위한 표준 제안이다.

**리서치 앵글:** 계정 추상화 환경에서 DeFi 프로토콜과 상호작용하는 자율형 AI 에이전트의 온체인 실행 보안 및 스마트 월렛 연계 분석에 활용 가능하다.

## 원문 미리보기
<p>AI agents now prepare and sign transactions with no person reading each one. the losses that follow are mostly not exotic, and each is visible before signing to anyone who reads the chain and the request:</p>
<p>· an unlimited approval to a spender that is a plain wallet or a week-old contract<br>
· a transfer to an address that shares its first and last characters with one the signer used before<br>
· a buy of a copy of a real token (on robinhood chain there are 3,148 copies of robinhood’s own stock tokens) or through a pool priced far from its oracle<br>
· an x402 payment to a payTo that 