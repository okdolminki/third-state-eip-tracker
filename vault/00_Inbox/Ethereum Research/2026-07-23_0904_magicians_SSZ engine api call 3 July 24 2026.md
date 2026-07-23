---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "SSZ engine api call 3, July 24, 2026"
author: ""
pub_date: "Wed, 22 Jul 2026 13:12:51 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-23
sources:
  - "https://ethereum-magicians.org/t/ssz-engine-api-call-3-july-24-2026/29060"
---
# SSZ engine api call 3, July 24, 2026

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/ssz-engine-api-call-3-july-24-2026/29060)  |  Wed, 22 Jul 2026 13:12:51 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 이더리움 핵심 개발자 회의(ACDE)에서 엔진 API의 누락된 비-엔진 메서드 최종 확정에 대한 논의가 진행 중입니다.

**리서치 앵글:** 이더리움 코어 프로토콜의 엔진 API 변경은 L2 확장성 및 MEV 구조에 근본적인 영향을 미칠 수 있습니다.

## 원문 미리보기
<h3><a name="p-72014-agenda-1" class="anchor" href="https://ethereum-magicians.org#p-72014-agenda-1" aria-label="Heading link"></a>Agenda</h3>
<ul>
<li><a href="https://hackmd.io/siEIwl9QTlODSZ6DYH3iqg" class="inline-onebox">Top-up sync - HackMD</a></li>
<li><a href="https://github.com/ethereum/pm/issues/2157#issuecomment-4981597977" class="inline-onebox">All Core Devs - Execution (ACDE) #241, July 16, 2026 · Issue #2157 · ethereum/pm · GitHub</a></li>
</ul>
<p>basicaly we would like to finalise the part about  missing non-engine methods that are exposed on the engine port and finalize that<br