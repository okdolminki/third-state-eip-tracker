---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "RPC Standards # 38, November 16, 2026"
author: ""
pub_date: "Tue, 10 Nov 2026 15:43:08 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-11
sources:
  - "https://ethereum-magicians.org/t/rpc-standards-38-november-16-2026/30331"
---
# RPC Standards # 38, November 16, 2026

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/rpc-standards-38-november-16-2026/30331)  |  Tue, 10 Nov 2026 15:43:08 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 이더리움 RPC 표준 논의에서 비활성 포크의 트랜잭션 필드 처리 및 `maxFeePerBlobGas` 관련 실행 API 변경 사항이 다루어집니다.

**리서치 앵글:** L2 확장성: `maxFeePerBlobGas` 관련 논의는 EIP-4844와 직결되어 L2 데이터 가용성 및 확장성에 중대한 영향을 미칩니다.

## 원문 미리보기
<h3><a name="p-76432-agenda-1" class="anchor" href="https://ethereum-magicians.org#p-76432-agenda-1" aria-label="Heading link"></a>Agenda</h3>
<p>Agenda</p>
<ul>
<li><a href="https://github.com/ethereum/execution-apis/pull/938#issuecomment-6770341261" class="inline-onebox">eth: reject transaction fields whose fork is not active at the target block by MysticRyuujin · Pull Request #938 · ethereum/execution-apis · GitHub</a></li>
<li><a href="https://github.com/ethereum/execution-apis/pull/939#issuecomment-6770341941" class="inline-onebox">eth: ignore type in calls and reject maxFeePerBlobGas wit