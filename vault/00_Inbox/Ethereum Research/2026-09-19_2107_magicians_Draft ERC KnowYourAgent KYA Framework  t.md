---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "[Draft ERC] Know-Your-Agent (KYA) Framework — trust assertions for agents, ZK-KYA profile, ERC-8004 binding"
author: ""
pub_date: "Sat, 19 Sep 2026 02:23:13 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-09-19
sources:
  - "https://ethereum-magicians.org/t/draft-erc-know-your-agent-kya-framework-trust-assertions-for-agents-zk-kya-profile-erc-8004-binding/29735"
---
# [Draft ERC] Know-Your-Agent (KYA) Framework — trust assertions for agents, ZK-KYA profile, ERC-8004 binding

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/draft-erc-know-your-agent-kya-framework-trust-assertions-for-agents-zk-kya-profile-erc-8004-binding/29735)  |  Sat, 19 Sep 2026 02:23:13 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** ERC-8004 기반의 에이전트 신원 및 신뢰 증명 프레임워크인 KYA(Know-Your-Agent)를 제안하는 초안 ERC.

**리서치 앵글:** 기관 DeFi 도입 및 계정 추상화와 연관된 에이전트 신원 및 신뢰 증명 표준 제안.

## 원문 미리보기
<p><strong>PR:</strong> <a href="https://github.com/ethereum/ERCs/pull/2012" rel="noopener nofollow ugc">ethereum/ERCs#2012</a>  ·  <strong>Repo / reference implementation:</strong> <a href="https://github.com/garyyang-finchip/kya-standard" rel="noopener nofollow ugc">garyyang-finchip/kya-standard</a>  ·  <strong>Status:</strong> Draft, number not yet assigned</p>
<h2><a name="p-74368-what-this-proposes-1" class="anchor" href="https://ethereum-magicians.org#p-74368-what-this-proposes-1" aria-label="Heading link"></a>What this proposes</h2>
<p>ERC-8004 gives agents portable identity and a place