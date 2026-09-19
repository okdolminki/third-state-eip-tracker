---
source: "Ethereum Research"
source_type: research
title: "Strict role alternation: reciprocal broadcast without relayers for EVM shielded pools (spec + population simulation, no code yet)"
author: ""
pub_date: "Sat, 19 Sep 2026 07:07:15 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-09-19
sources:
  - "https://ethresear.ch/t/strict-role-alternation-reciprocal-broadcast-without-relayers-for-evm-shielded-pools-spec-population-simulation-no-code-yet/26051"
---
# Strict role alternation: reciprocal broadcast without relayers for EVM shielded pools (spec + population simulation, no code yet)

> 출처: [Ethereum Research](https://ethresear.ch/t/strict-role-alternation-reciprocal-broadcast-without-relayers-for-evm-shielded-pools-spec-population-simulation-no-code-yet/26051)  |  Sat, 19 Sep 2026 07:07:15 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** EVM 쉴드 풀의 릴레이어 의존성 문제를 해결하기 위해, 릴레이어 시장을 노트 자체에 내재된 상호성으로 대체하는 방안을 제안한다.

**리서치 앵글:** EVM 쉴드 풀의 릴레이어 의존성 문제를 해결하는 방안으로, 계정 추상화(EIP-7702)와 연관된 가스 지불 및 트랜잭션 모델 개선에 기여할 수 있음.

## 원문 미리보기
<p>Shielded pools on the EVM depend on relayers because <code>msg.sender</code> has to pay gas from a funded transparent account. The June 2026 Railgun measurement (arXiv:2606.25926) shows both exits of that dependency: 1,049 self-broadcast withdrawals linked to their depositor through the gas payer, and 124 relayer-like addresses serving 89% of relayed volume. Zcash never had this problem; it is an artefact of the account model, not of ZK.</p>
<p>This is a proposal to replace the relayer <em>market</em> with reciprocity embedded in the note itself. Each shielded note carries a role bit inside