---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "SSZ Engine Api #1,June 26,2026"
author: ""
pub_date: "Thu, 18 Jun 2026 16:48:15 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-19
sources:
  - "https://ethereum-magicians.org/t/ssz-engine-api-1-june-26-2026/28832"
---
# SSZ Engine Api #1,June 26,2026

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/ssz-engine-api-1-june-26-2026/28832)  |  Thu, 18 Jun 2026 16:48:15 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 이더리움 실행-합의 레이어 간 핵심 인터페이스인 SSZ Engine API의 사양, 테스트, 구현을 위한 논의가 시작됩니다.

**리서치 앵글:** 이더리움 코어 프로토콜의 엔진 API 변경은 MEV 구조 및 L2 확장성에 간접적인 영향을 미칠 수 있습니다.

## 원문 미리보기
<h3><a name="p-71205-agenda-1" class="anchor" href="https://ethereum-magicians.org#p-71205-agenda-1" aria-label="Heading link"></a>Agenda</h3>
<p>This call will kick off the SSZ Engine API breakout sessions.</p>
<p>The primary focus will be on the specification, testing, and implementation of the REST-SSZ Engine API layer, as well as coordinating the work required to bring the feature to production readiness and eventual adoption across the clients.</p>
<ul>
<li>Pre-readings
<ul>
<li><a href="https://github.com/ethereum/execution-apis/pull/793">Specs</a></li>
</ul>
</li>
<li>Series intro
<ul>
