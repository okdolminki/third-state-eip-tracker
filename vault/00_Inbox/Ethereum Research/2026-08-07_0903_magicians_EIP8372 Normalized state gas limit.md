---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8372: Normalized state gas limit"
author: ""
pub_date: "Thu, 06 Aug 2026 17:55:30 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-07
sources:
  - "https://ethereum-magicians.org/t/eip-8372-normalized-state-gas-limit/29332"
---
# EIP-8372: Normalized state gas limit

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8372-normalized-state-gas-limit/29332)  |  Thu, 06 Aug 2026 17:55:30 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8372는 스테이트 가스 한도를 조정하여 스테이트 가스와 실행 가스 사용량의 균형을 맞추는 것을 목표로 합니다.

**리서치 앵글:** 이 EIP는 이더리움의 가스 모델 변경을 통해 L2 확장성에 중대한 영향을 미칠 수 있습니다.

## 원문 미리보기
<p>Discussion topic for EIP-8372; <a href="https://github.com/ethereum/EIPs/pull/12119">PR</a>.</p>
<h4><a name="p-72809-description-1" class="anchor" href="https://ethereum-magicians.org#p-72809-description-1" aria-label="Heading link"></a>Description</h4>
<p>Scales and normalizes the state-gas limit to balance state-gas and execution-gas utilization.</p>
<h4><a name="p-72809-when-this-can-be-useful-2" class="anchor" href="https://ethereum-magicians.org#p-72809-when-this-can-be-useful-2" aria-label="Heading link"></a>When this can be useful</h4>
<p>This proposal is useful if observations afte