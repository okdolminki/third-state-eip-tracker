---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8293: Counterfactual Rejection Event Log (CREL)"
author: ""
pub_date: "Mon, 15 Jun 2026 05:07:46 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-15
sources:
  - "https://ethereum-magicians.org/t/erc-8293-counterfactual-rejection-event-log-crel/28792"
---
# ERC-8293: Counterfactual Rejection Event Log (CREL)

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8293-counterfactual-rejection-event-log-crel/28792)  |  Mon, 15 Jun 2026 05:07:46 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** ERC-8293은 DEX 프로토콜이나 필터가 실행 전에 거부한 거래 후보에 대해 거부 시점과 사후 결과를 온체인 이벤트 로그로 기록하는 표준을 제안합니다.

**리서치 앵글:** Uniswap 등 DEX 프로토콜의 트랜잭션 필터링 및 MEV 방지 메커니즘 설계와 밀접한 연관이 있어, DEX 경쟁 구도 테마에서 분석할 가치가 있습니다.

## 원문 미리보기
<p>ERC-8293: Counterfactual Rejection Event Log (CREL)</p>
<p>PR: <a href="https://github.com/ethereum/ERCs/pull/1806" class="inline-onebox" rel="noopener nofollow ugc">Add ERC: Counterfactual Rejection Event Log (CREL) by aartikamat · Pull Request #1806 · ethereum/ERCs · GitHub</a></p>
<p>Abstract</p>
<p>ERC-8293 specifies an on-chain event log for trading candidates that a DEX protocol or filter rejects before execution. Two events: RejectionLogged at the moment of rejection, OutcomeSampled at fixed intervals afterward to record what the rejected token actually did. Protocols that emit these