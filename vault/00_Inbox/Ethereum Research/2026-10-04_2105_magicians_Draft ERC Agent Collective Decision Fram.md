---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "[Draft ERC] Agent Collective Decision Framework (ACDF) — authorized, composable collective decisions with procedural finality"
author: ""
pub_date: "Sun, 04 Oct 2026 00:55:45 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-04
sources:
  - "https://ethereum-magicians.org/t/draft-erc-agent-collective-decision-framework-acdf-authorized-composable-collective-decisions-with-procedural-finality/29850"
---
# [Draft ERC] Agent Collective Decision Framework (ACDF) — authorized, composable collective decisions with procedural finality

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/draft-erc-agent-collective-decision-framework-acdf-authorized-composable-collective-decisions-with-procedural-finality/29850)  |  Sun, 04 Oct 2026 00:55:45 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 자격을 갖춘 참여자(에이전트, 인간 또는 계약)가 명시된 권한 내에서 정의된 효과를 가진 집단적 결정을 내릴 수 있도록 하는 에이전트 집단 의사결정 프레임워크(ACDF)에 대한 ERC 초안입니다.

**리서치 앵글:** 이 프레임워크는 기관 DeFi 도입을 위한 온체인 집단 의사결정 및 프로토콜 거버넌스 방식에 영향을 미치며, 계정 추상화와 연관될 수 있습니다.

## 원문 미리보기
<p>Hi all,</p>
<p>This is a draft ERC for an <strong>Agent Collective Decision Framework (ACDF)</strong>: two co-deployable registries through which qualified participants — agents, humans or contracts — form collective decisions with a defined effect, within explicit authorization, under rules that are frozen as the very parameters the registry executes.</p>
<p>Repository (design memo, reference implementation, tests, vectors): <a href="https://github.com/garyyang-finchip/acd-framework" class="inline-onebox" rel="noopener nofollow ugc">GitHub - garyyang-finchip/acd-framework: Agent Collective