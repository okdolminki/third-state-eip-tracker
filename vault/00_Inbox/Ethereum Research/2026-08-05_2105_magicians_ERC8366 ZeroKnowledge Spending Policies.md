---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8366: Zero-Knowledge Spending Policies"
author: ""
pub_date: "Wed, 05 Aug 2026 05:37:12 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-05
sources:
  - "https://ethereum-magicians.org/t/erc-8366-zero-knowledge-spending-policies/29281"
---
# ERC-8366: Zero-Knowledge Spending Policies

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8366-zero-knowledge-spending-policies/29281)  |  Wed, 05 Aug 2026 05:37:12 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 이 ERC는 사용자의 자금을 보유한 컨트랙트가 사전 등록된 지출 정책을 영지식 증명으로 만족할 때만 자금을 해제하도록 표준화합니다.

**리서치 앵글:** EIP-7702를 포함한 계정 추상화 및 스마트 지갑의 영지식 기반 지출 정책 구현과 관련이 있습니다.

## 원문 미리보기
<h2><a name="p-72647-abstract-1" class="anchor" href="https://ethereum-magicians.org#p-72647-abstract-1" aria-label="Heading link"></a>Abstract</h2>
<p>This ERC standardizes <strong>zero-knowledge spending policies</strong>: a composable function set that any contract holding a user’s funds (a dedicated escrow, a smart wallet, an ERC-4337 account, or an EIP-7702-delegated EOA) can implement to release those funds only against a zero-knowledge proof that the payment satisfies a spending policy the owner registered in advance. Implementing the set turns the contract into a policy escrow for the 