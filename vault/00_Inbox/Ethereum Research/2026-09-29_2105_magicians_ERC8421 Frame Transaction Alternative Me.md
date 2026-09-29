---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8421: Frame Transaction Alternative Mempools"
author: ""
pub_date: "Tue, 29 Sep 2026 11:51:48 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-09-29
sources:
  - "https://ethereum-magicians.org/t/erc-8421-frame-transaction-alternative-mempools/29800"
---
# ERC-8421: Frame Transaction Alternative Mempools

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8421-frame-transaction-alternative-mempools/29800)  |  Tue, 29 Sep 2026 11:51:48 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** ERC-8421은 ERC-4337 UserOperation과 유사하게 Frame Transaction을 위한 대체 멤풀 규칙을 정의하며, EIP-8141의 맥락에서 평판 기반 시스템을 도입합니다.

**리서치 앵글:** ERC-4337 기반의 계정 추상화 트랜잭션 처리 방식 및 멤풀 경쟁 구도에 영향을 미칠 수 있습니다.

## 원문 미리보기
<p>A Frame Transaction specific definitions for alternative mempool rules, similar in structure and mostly backward compatible with the <a href="https://eips.ethereum.org/EIPS/eip-7562" rel="noopener nofollow ugc">ERC-7562</a> validation rules for <a href="https://eips.ethereum.org/EIPS/eip-4337" rel="noopener nofollow ugc">ERC-4337</a> UserOperations.</p>
<p>In the context of EIP-8141 serves as a more permissive, reputation-based system compared to the ‘canonical mempool’ defined as part of the core protocol.<br>
Conceptually, the “reputation” system of ERC-8421/ERC-7562 is similar to that pr