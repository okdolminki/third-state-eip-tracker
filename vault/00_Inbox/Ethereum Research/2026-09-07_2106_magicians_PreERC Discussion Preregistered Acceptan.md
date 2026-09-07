---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "[Pre-ERC Discussion] Preregistered Acceptance Criteria"
author: ""
pub_date: "Mon, 07 Sep 2026 06:24:25 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-09-07
sources:
  - "https://ethereum-magicians.org/t/pre-erc-discussion-preregistered-acceptance-criteria/29609"
---
# [Pre-ERC Discussion] Preregistered Acceptance Criteria

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/pre-erc-discussion-preregistered-acceptance-criteria/29609)  |  Mon, 07 Sep 2026 06:24:25 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 에이전트 스택 내 다양한 검증 프리미티브(ERC-8274, ERC-8404 등)가 결과 재계산 및 다이제스트 비교라는 동일한 형태로 귀결됨을 논의합니다.

**리서치 앵글:** 새로운 ERC 및 검증 프리미티브 논의는 L2 확장성 및 계정 추상화와 연관되어 미래 온체인 에이전트 및 복잡한 연산 검증에 영향을 미칠 수 있습니다.

## 원문 미리보기
<p>Topic title: [Pre-ERC Discussion] Preregistered Acceptance Criteria<br>
Category: ERCs</p>
<hr>
<p>Every verification primitive in the agent stack reduces to the same shape:<br>
recompute the result, compare digests. <a href="https://ethereum-magicians.org/t/erc-8274-ai-inference-proof-verification/28083">ERC-8274</a> verifies an<br>
<code>(inputHash, outputHash, proof)</code> triple. ERC-8404 issues a receipt over<br>
<code>REPRODUCED | DIVERGED | CANNOT_RECOMPUTE</code>. ERC-8263 anchors a digest.<br>
Inclusion-proof designs confirm a commitment made earlier. Every one of them<br>
assumes