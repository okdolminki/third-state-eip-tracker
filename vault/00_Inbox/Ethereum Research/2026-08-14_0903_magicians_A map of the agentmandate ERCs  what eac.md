---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "A map of the agent-mandate ERCs — what each one actually does"
author: ""
pub_date: "Thu, 13 Aug 2026 16:14:23 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-14
sources:
  - "https://ethereum-magicians.org/t/a-map-of-the-agent-mandate-ercs-what-each-one-actually-does/29421"
---
# A map of the agent-mandate ERCs — what each one actually does

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/a-map-of-the-agent-mandate-ercs-what-each-one-actually-does/29421)  |  Thu, 13 Aug 2026 16:14:23 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 온체인 자율 에이전트의 활동 범위를 정의하는 다양한 ERC 표준들의 실제 기능을 명확히 구분하고 설명하는 글입니다.

**리서치 앵글:** 계정 추상화(EIP-7702)와 관련된 에이전트 권한 및 위임 표준 논의에 대한 이해를 심화합니다.

## 원문 미리보기
<p>If you are trying to work out how to bound what an autonomous agent may do on-chain, you<br>
will find a dozen ERCs that sound like they answer the question. Most of them answer a<br>
different one. Working out which is which took me a week, so here is the map, with the<br>
method attached so you can check it rather than trust it.</p>
<p>This is not a critique of anyone’s work. Several of the standards below deliberately<br>
exclude what I was looking for, and say so.</p>
<h3><a name="p-73252-method-1" class="anchor" href="https://ethereum-magicians.org#p-73252-method-1" aria-label="Heading