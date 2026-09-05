---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8410: Portable Execution Plan Artifact"
author: ""
pub_date: "Fri, 04 Sep 2026 15:25:46 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-09-05
sources:
  - "https://ethereum-magicians.org/t/erc-8410-portable-execution-plan-artifact/29587"
---
# ERC-8410: Portable Execution Plan Artifact

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8410-portable-execution-plan-artifact/29587)  |  Fri, 04 Sep 2026 15:25:46 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 키가 없는 소프트웨어에서 지갑으로 순서화된 호출 시퀀스와 검증용 해시를 안전하게 전달하기 위한 실행 계획 JSON 표준 규격 제안이다.

**리서치 앵글:** 계정 추상화(EIP-7702) 및 스마트 지갑 환경에서 복잡한 다단계 DeFi 트랜잭션 배치 실행 및 서명 UX 표준화와 연관된다.

## 원문 미리보기
<p>Discussion thread for <a href="https://github.com/ethereum/ERCs/pull/1992" rel="noopener nofollow ugc">ERC-8409</a>, a JSON document that carries an ordered call sequence for one sender on one chain from software that holds no keys to the wallet that does, together with a keccak256 digest over exactly the fields that determine what gets broadcast.</p>
            <p><small>1 post - 1 participant</small></p>
            <p><a href="https://ethereum-magicians.org/t/erc-8410-portable-execution-plan-artifact/29587">Read full topic</a></p>