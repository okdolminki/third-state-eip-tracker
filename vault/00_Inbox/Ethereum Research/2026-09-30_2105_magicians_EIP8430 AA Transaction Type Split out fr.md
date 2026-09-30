---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8430: AA Transaction Type (Split out from 8130)"
author: ""
pub_date: "Wed, 30 Sep 2026 12:00:45 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-09-30
sources:
  - "https://ethereum-magicians.org/t/eip-8430-aa-transaction-type-split-out-from-8130/29810"
---
# EIP-8430: AA Transaction Type (Split out from 8130)

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8430-aa-transaction-type-split-out-from-8130/29810)  |  Wed, 30 Sep 2026 12:00:45 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8430은 EIP-8130에서 트랜잭션 타입을 분리하여 키스토어 의존성 없이 독립적인 EIP로 제안합니다.

**리서치 앵글:** 계정 추상화(AA)의 핵심 구성 요소인 트랜잭션 타입 표준화 논의로, EIP-7702와 연관된 계정 추상화 연구에 중요합니다.

## 원문 미리보기
<p>EIP-8430 splits the transaction type out of [EIP-8130]( <a href="https://eips.ethereum.org/EIPS/eip-8130" class="inline-onebox" rel="noopener nofollow ugc">EIP-8130: Keystore Accounts</a> ) into its own EIP, with no Keystore dependency. EIP-8130 keeps the Keystore.</p>
<p>- EIP-8430 PR: <a href="https://github.com/ethereum/EIPs/pull/12385" class="inline-onebox" rel="noopener nofollow ugc">Add EIP: AA Transaction Type by chunter-cb · Pull Request #12385 · ethereum/EIPs · GitHub</a></p>
<p>- EIP-8130 update PR: <a href="https://github.com/ethereum/EIPs/pull/12386" class="inline-onebox" rel="n