---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8429: Escalating gas for repeated calls"
author: ""
pub_date: "Tue, 29 Sep 2026 08:27:32 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-09-29
sources:
  - "https://ethereum-magicians.org/t/eip-8429-escalating-gas-for-repeated-calls/29798"
---
# EIP-8429: Escalating gas for repeated calls

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8429-escalating-gas-for-repeated-calls/29798)  |  Tue, 29 Sep 2026 08:27:32 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 동일 블록 내 옵트인된 컨트랙트에 대한 반복 호출에 대해 가스비를 점진적으로 인상하고, 추가 가스비는 스테이킹되는 EIP-8429 논의.

**리서치 앵글:** MEV 테마와 관련하여 블록 생산자의 이득을 제한하는 가스 메커니즘 변경 가능성.

## 원문 미리보기
<p>Discussion topic for <a href="https://github.com/ethereum/EIPs/pull/12384" rel="noopener nofollow ugc">EIP-8429</a></p>
<p>Repetition is underpriced. The k-th call into an opted-in contract within a block pays G_REF * k^2 extra gas.<br>
Half of that is deposited as stake with no withdrawer. Half is staked where the opted-in contract points.<br>
The block producer gets nothing, so nobody has a reason to farm it.</p>
<h4><a name="p-74656-update-log-1" class="anchor" href="https://ethereum-magicians.org#p-74656-update-log-1" aria-label="Heading link"></a>Update Log</h4>
<ul>
<li>2026-09-28: in