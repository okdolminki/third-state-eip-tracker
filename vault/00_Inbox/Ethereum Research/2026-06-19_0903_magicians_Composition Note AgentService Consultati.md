---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Composition Note: Agent-Service Consultation Flow composing the agent ERCs (8004 · 8263 · 8274 · 8275 · 8281 · 8299 · 8301) [Informational]"
author: ""
pub_date: "Thu, 18 Jun 2026 21:26:44 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-19
sources:
  - "https://ethereum-magicians.org/t/composition-note-agent-service-consultation-flow-composing-the-agent-ercs-8004-8263-8274-8275-8281-8299-8301-informational/28833"
---
# Composition Note: Agent-Service Consultation Flow composing the agent ERCs (8004 · 8263 · 8274 · 8275 · 8281 · 8299 · 8301) [Informational]

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/composition-note-agent-service-consultation-flow-composing-the-agent-ercs-8004-8263-8274-8275-8281-8299-8301-informational/28833)  |  Thu, 18 Jun 2026 21:26:44 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 여러 에이전트 관련 ERC들을 조합하여 에이전트가 전문 서비스를 이용하고 검증 가능한 결과를 얻으며 신뢰 없이 비용을 지불하는 종단 간 흐름을 설명하는 글.

**리서치 앵글:** 여러 에이전트 ERC의 조합을 통한 신뢰 없는 서비스 이용 및 결제 흐름은 계정 추상화(EIP-7702)의 실제 적용 및 확장 가능성과 밀접하게 연관됨.

## 원문 미리보기
<p>Several of the agent-layer standards now in flight each define one layer of an agent interaction, identity, input provenance, verification, anchoring, eligibility, settlement, orchestration. What hasn’t existed is a <em>canonical end-to-end flow</em> showing how they compose into one real interaction: an agent (or human) consulting another agent’s specialised service, getting a <strong>verifiable</strong> result, and <strong>paying</strong> for it without trusting the provider.</p>
<p>This note documents that composition pattern. <strong>The contribution is the pattern and the per-step inva