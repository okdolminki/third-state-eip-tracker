---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Providing protocol interaction knowledge in machine readable files (translating intent into transactions)"
author: ""
pub_date: "Fri, 29 May 2026 14:45:43 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-05-31
sources:
  - "https://ethereum-magicians.org/t/providing-protocol-interaction-knowledge-in-machine-readable-files-translating-intent-into-transactions/28663"
---
# Providing protocol interaction knowledge in machine readable files (translating intent into transactions)

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/providing-protocol-interaction-knowledge-in-machine-readable-files-translating-intent-into-transactions/28663)  |  Fri, 29 May 2026 14:45:43 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 프로토콜 상호작용 지식이 온체인에 없고 웹사이트와 SDK에 의존하여 중앙화 위험을 초래하며, 이를 기계 판독 가능한 형식으로 제공하여 의도를 트랜잭션으로 변환하는 필요성을 제기한다.

**리서치 앵글:** 사용자 의도를 트랜잭션으로 변환하는 기계 판독 가능한 프로토콜 상호작용 지식의 필요성은 계정 추상화(EIP-7702) 및 기관 DeFi 도입과 밀접하게 연관된다.

## 원문 미리보기
<h2><a name="p-70442-the-problem-1" class="anchor" href="https://ethereum-magicians.org#p-70442-the-problem-1" aria-label="Heading link"></a>The Problem</h2>
<p>Protocol interaction knowledge exists primarily in websites and SDKs and not on-chain or in a portable machine-readable format. The websites set up to support dApps are a centralisation risk that depend upon developer team availability for regular maintenance.</p>
<p>Every DeFi protocol exposes functionality through smart contract ABIs. While an ABI can tell you the function names, parameter types and returned values, it does not tell 