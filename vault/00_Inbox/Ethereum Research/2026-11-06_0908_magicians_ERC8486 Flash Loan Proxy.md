---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8486: Flash Loan Proxy"
author: ""
pub_date: "Thu, 05 Nov 2026 13:13:39 +0000"

importance: medium
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-06
sources:
  - "https://ethereum-magicians.org/t/erc-8486-flash-loan-proxy/30289"
---
# ERC-8486: Flash Loan Proxy

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8486-flash-loan-proxy/30289)  |  Thu, 05 Nov 2026 13:13:39 +0000

## AI 분석
**중요도:** medium | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 이 표준은 임시 저장소에 프로그램과 캘데이터를 캐싱하여 실행 세션을 조정하고, DELEGATECALL을 통해 고정된 구현으로 전달하며, 핸들러 플래그로 재진입 호출을 제어하는 프록시를 정의합니다.

**리서치 앵글:** DeFi 프로토콜의 복잡한 상호작용 및 플래시 론 활용 방식에 영향을 미쳐 DeFi 기관 도입 및 DEX 경쟁구도에 연관됩니다.

## 원문 미리보기
<h2><a name="p-76280-abstract-1" class="anchor" href="https://ethereum-magicians.org#p-76280-abstract-1" aria-label="Heading link"></a>Abstract</h2>
<p>This standard defines a proxy that coordinates execution sessions by temporarily caching a program and its associated calldata in transient storage. The proxy forwards the cached program to a fixed implementation through <code>DELEGATECALL</code> and uses a handler flag to control whether subsequent reentrant invocations are dispatched.</p>
<p>The program remains unchanged throughout an execution session, while the cached calldata is replaced o