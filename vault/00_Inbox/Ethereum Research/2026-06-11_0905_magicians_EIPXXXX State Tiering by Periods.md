---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-XXXX: State Tiering by Periods"
author: ""
pub_date: "Wed, 10 Jun 2026 16:40:21 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-11
sources:
  - "https://ethereum-magicians.org/t/eip-xxxx-state-tiering-by-periods/28763"
---
# EIP-XXXX: State Tiering by Periods

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-xxxx-state-tiering-by-periods/28763)  |  Wed, 10 Jun 2026 16:40:21 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 이 제안은 이더리움 상태 쓰기 작업에 '갱신 연령 가격'을 도입하여, 상태의 마지막 쓰기 시점에 따라 활성/비활성 계층으로 구분하고 비활성 상태 쓰기에 더 높은 가스 비용을 부과합니다.

**리서치 앵글:** 이더리움 L1의 상태 관리 및 가스 비용 변경은 L2 확장성과 커버리지 프로토콜의 운영 효율성에 직접적인 영향을 미칩니다.

## 원문 미리보기
<p><strong>## Abstract</strong></p>
<p>This proposal introduces <em>_renewal-age pricing_</em> for Ethereum state writes. It builds on the `last_written_block` write-age metadata defined in [EIP-8188](./eip-8188.md), deriving a coarse `period` from each item’s last-write block number. The gas cost of state-writing operations depends on whether the target state is in the <strong>**Active**</strong> or <strong>**Inactive**</strong> tier, determined by how many periods have elapsed since its last write. Writing to Inactive state is more expensive than writing to Active state. Read costs are uncha