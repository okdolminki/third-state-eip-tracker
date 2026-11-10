---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8487: Separate execution credits and billing credits"
author: ""
pub_date: "Mon, 09 Nov 2026 15:07:10 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-10
sources:
  - "https://ethereum-magicians.org/t/eip-8487-separate-execution-credits-and-billing-credits/30320"
---
# EIP-8487: Separate execution credits and billing credits

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8487-separate-execution-credits-and-billing-credits/30320)  |  Mon, 09 Nov 2026 15:07:10 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8487은 EVM이 사용하는 '실행 크레딧'과 실제 트랜잭션 비용을 결정하는 '청구 크레딧'을 분리하는 새로운 가스 스케줄을 제안합니다.

**리서치 앵글:** 가스 스케줄 변경은 L2 확장성 및 MEV 역학에 중대한 영향을 미칠 수 있습니다.

## 원문 미리보기
<p>This is the discussion thread for EIP-8487 (PR: <a href="https://github.com/ethereum/EIPs/pull/12637" class="inline-onebox" rel="noopener nofollow ugc">Add EIP: Separate execution credits and billing credits by Giulio2002 · Pull Request #12637 · ethereum/EIPs · GitHub</a>).</p>
<p>The proposal introduces two counters, both initialized from <code>tx.gasLimit</code>:</p>
<ul>
<li><strong>Credits</strong> follow the legacy gas schedule and are the only gas the EVM sees (GAS opcode, call forwarding, creation).</li>
<li><strong>Billing</strong> follows the new schedule and determines the transac