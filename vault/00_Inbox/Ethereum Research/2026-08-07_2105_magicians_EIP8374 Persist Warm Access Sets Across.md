---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8374: Persist Warm Access Sets Across Reverts"
author: ""
pub_date: "Fri, 07 Aug 2026 09:00:43 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-07
sources:
  - "https://ethereum-magicians.org/t/eip-8374-persist-warm-access-sets-across-reverts/29341"
---
# EIP-8374: Persist Warm Access Sets Across Reverts

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8374-persist-warm-access-sets-across-reverts/29341)  |  Fri, 07 Aug 2026 09:00:43 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8374는 EIP-2929의 접근 세트(access set) 롤백 기능을 제거하여, 호출 프레임이 되돌려지더라도 한 번 접근된 주소나 저장 키가 '웜(warm)' 상태를 유지하도록 제안합니다.

**리서치 앵글:** 이 EIP는 이더리움의 가스 비용 계산 방식에 영향을 주어 L2 확장성 및 전반적인 DeFi 프로토콜의 효율성에 중기적인 영향을 미칠 수 있습니다.

## 원문 미리보기
<p>EIP PR: <a href="https://github.com/ethereum/EIPs/pull/12128/changes" class="inline-onebox" rel="noopener nofollow ugc">Add EIP: Persist Warm Access Sets Across Reverts by rakita · Pull Request #12128 · ethereum/EIPs · GitHub</a></p>
<p>Abstraction:</p>
<p><a>EIP-2929</a> tracks accessed addresses and storage keys in the transaction-scoped sets <code>accessed_addresses</code> and <code>accessed_storage_keys</code>, and rolls both sets back to their pre-call state when a call frame reverts or exceptionally halts. This EIP removes that rollback: once an address or storage key is added to an a