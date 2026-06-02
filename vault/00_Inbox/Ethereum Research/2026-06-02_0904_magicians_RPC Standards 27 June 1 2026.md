---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "RPC Standards #27, June 1, 2026"
author: ""
pub_date: "Mon, 01 Jun 2026 14:11:20 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-02
sources:
  - "https://ethereum-magicians.org/t/rpc-standards-27-june-1-2026/28676"
---
# RPC Standards #27, June 1, 2026

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/rpc-standards-27-june-1-2026/28676)  |  Mon, 01 Jun 2026 14:11:20 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 이더리움 RPC 표준 논의에서 `eth_*` 상태 메서드의 블록 파라미터 필수 여부 및 기본값 설정에 대한 업데이트가 진행 중이며, 관련 실행 API 변경사항이 논의되고 있습니다.

**리서치 앵글:** RPC 표준은 L2 확장성 및 기관 DeFi 도입을 포함한 모든 DeFi 프로토콜의 이더리움 상호작용에 필수적인 기반 기술로, 개발자 경험과 시스템 안정성에 영향을 미칩니다.

## 원문 미리보기
<h3><a name="p-70492-agenda-1" class="anchor" href="https://ethereum-magicians.org#p-70492-agenda-1" aria-label="Heading link"></a>Agenda</h3>
<ul>
<li>ethereum/execution-apis#807, ethereum/execution-apis#808, &amp; <a href="https://closertools.github.io/execution-apis/">upcoming docs update</a></li>
<li><code>eth_*</code> state methods — block param required vs default-to-latest (ref: <a href="https://github.com/NethermindEth/nethermind/issues/11764">NethermindEth/nethermind#11764</a>) - see <a href="https://discord.com/channels/595666850260713488/804019759934078987/1509209722505658398">Disco