---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "[Draft ERC] Swarm AI Framework — registry and charter model for purpose-bound agent swarms"
author: ""
pub_date: "Sun, 18 Oct 2026 05:22:46 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-18
sources:
  - "https://ethereum-magicians.org/t/draft-erc-swarm-ai-framework-registry-and-charter-model-for-purpose-bound-agent-swarms/29998"
---
# [Draft ERC] Swarm AI Framework — registry and charter model for purpose-bound agent swarms

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/draft-erc-swarm-ai-framework-registry-and-charter-model-for-purpose-bound-agent-swarms/29998)  |  Sun, 18 Oct 2026 05:22:46 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 자율 에이전트들이 목적 기반의 집단인 '스웜'을 온체인에서 형성, 운영, 해체할 수 있도록 하는 등록 및 헌장 모델을 제안한다.

**리서치 앵글:** 이 제안은 자율 에이전트 스웜이 온체인에서 활동하며 MEV 전략을 최적화하고 기관의 DeFi 도입을 촉진할 가능성과 연관된다.

## 원문 미리보기
<h2><a name="p-75359-summary-1" class="anchor" href="https://ethereum-magicians.org#p-75359-summary-1" aria-label="Heading link"></a>Summary</h2>
<p>We propose a registry and charter model through which autonomous agents — and any other account that qualifies — form, bound, run and dissolve <strong>swarms</strong>: purpose-bound collectives with an explicit membership boundary, an objective with attainment rules and a declared collaboration structure, recorded as one interoperable on-chain object.</p>
<p>Agent standards so far cover the individual (identity, reputation, validation), the act (o