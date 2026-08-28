---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8391: Execution Delegation Framework"
author: ""
pub_date: "Thu, 27 Aug 2026 15:27:59 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-28
sources:
  - "https://ethereum-magicians.org/t/erc-8391-execution-delegation-framework/29527"
---
# ERC-8391: Execution Delegation Framework

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8391-execution-delegation-framework/29527)  |  Thu, 27 Aug 2026 15:27:59 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** ERC-8391은 콜드 월렛/멀티시그 소유자가 핫 키를 안전하게 관리하고 온체인 실행 권한을 위임할 수 있는 표준 프레임워크를 제안합니다.

**리서치 앵글:** 기관 DeFi 도입을 위한 안전한 온체인 실행 위임 및 계정 추상화 관련 잠재적 표준.

## 원문 미리보기
<h3><a name="p-73647-discussion-topic-for-erc-8391-1" class="anchor" href="https://ethereum-magicians.org#p-73647-discussion-topic-for-erc-8391-1" aria-label="Heading link"></a>Discussion topic for ERC-8391</h3>
<p>Summary</p>
<p>ERC-8391 defines a standard contract interface for delegating on-chain execution authority to a rotatable operational key. An integrator authorizes the delegation contract once, while its owner, ideally a cold wallet or multisig, can assign, rotate, or immediately revoke the active hot key without further integrator involvement. It supports both direct execution throu