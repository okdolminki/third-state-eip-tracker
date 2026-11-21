---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Draft ERC: Agent Whitelist Framework (AWF) - scoped allow and deny lists for agents, adopted per consumer, with stated grounds and uniform results"
author: ""
pub_date: "Fri, 20 Nov 2026 13:35:37 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-21
sources:
  - "https://ethereum-magicians.org/t/draft-erc-agent-whitelist-framework-awf-scoped-allow-and-deny-lists-for-agents-adopted-per-consumer-with-stated-grounds-and-uniform-results/30456"
---
# Draft ERC: Agent Whitelist Framework (AWF) - scoped allow and deny lists for agents, adopted per consumer, with stated grounds and uniform results

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/draft-erc-agent-whitelist-framework-awf-scoped-allow-and-deny-lists-for-agents-adopted-per-consumer-with-stated-grounds-and-uniform-results/30456)  |  Fri, 20 Nov 2026 13:35:37 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** AWF는 특정 활동 내에서 어떤 에이전트와 객체를 허용하거나 거부할지, 그 근거와 효과를 명시하는 화이트리스트 및 블랙리스트 프레임워크입니다.

**리서치 앵글:** 기관 DeFi 도입 시 필요한 접근 제어 및 규제 준수를 위한 표준화된 화이트리스트/블랙리스트 프레임워크로 활용될 수 있습니다.

## 원문 미리보기
<p>This topic is the discussion thread for a draft ERC, <strong>Agent Whitelist Framework (AWF)</strong>.</p>
<h2><a name="p-76991-summary-1" class="anchor" href="https://ethereum-magicians.org#p-76991-summary-1" aria-label="Heading link"></a>Summary</h2>
<p>AWF is a framework in which one or more parties state, within a declared activity, which agents and other objects they admit and which they refuse, on which grounds, and with what effect.</p>
<p>It defines whitelists and blacklists together: both are lists of one kind that differ only in polarity, <code>ALLOW</code> or <code>DENY</code>. A