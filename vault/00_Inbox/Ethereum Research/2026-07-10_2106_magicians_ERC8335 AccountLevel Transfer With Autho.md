---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8335: Account-Level Transfer With Authorization"
author: ""
pub_date: "Fri, 10 Jul 2026 03:12:14 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-10
sources:
  - "https://ethereum-magicians.org/t/erc-8335-account-level-transfer-with-authorization/28977"
---
# ERC-8335: Account-Level Transfer With Authorization

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8335-account-level-transfer-with-authorization/28977)  |  Fri, 10 Jul 2026 03:12:14 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 스마트 컨트랙트 계정에 ERC-20 및 네이티브 자산 전송을 위한 표준 인터페이스를 추가하여, 온체인 사전 승인 없이 오프체인 서명된 EIP-712 권한 부여를 통해 모든 토큰과 ETH에 대한 계정 수준의 전송 기능을 제공합니다.

**리서치 앵글:** 계정 추상화(EIP-7702)의 핵심 구성 요소로, L2 확장성 및 사용자 경험 개선에 기여합니다.

## 원문 미리보기
<p>Add a standard interface on smart contract accounts that executes ERC-20 and native asset transfers from an off-chain signed EIP-712 authorization, submittable by any relayer with no prior on-chain approval. The account verifies the authorization with its own signature validation logic, so any signature scheme the account supports can be used. Intended to offer similar functionality to ERC-3009, implemented at the account level instead of the token level so it works for any ERC-20 token and native ETH.</p>
<aside class="onebox githubpullrequest" data-onebox-src="https://github.com/ethereum/