---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Vantage-Authority Resolution Profiles — public companion to ERC-8309's divergence boundary (#1826)"
author: ""
pub_date: "Thu, 10 Sep 2026 13:46:45 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-09-11
sources:
  - "https://ethereum-magicians.org/t/vantage-authority-resolution-profiles-public-companion-to-erc-8309s-divergence-boundary-1826/29637"
---
# Vantage-Authority Resolution Profiles — public companion to ERC-8309's divergence boundary (#1826)

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/vantage-authority-resolution-profiles-public-companion-to-erc-8309s-divergence-boundary-1826/29637)  |  Thu, 10 Sep 2026 13:46:45 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** ERC-8309는 충돌하는 관측값을 묵묵히 중복 제거하는 대신, 이를 일급 저장 상태로 보존하고 선언된 해결 정책을 첨부할 수 있는 확장 지점을 제공하며, 이 동반 사양은 해당 정책을 정의한다.

**리서치 앵글:** 이더리움 프로토콜의 상태 불일치 처리 방식 변경은 L2 확장성 및 계정 추상화(EIP-7702)와 같은 미래 이더리움 아키텍처에 근본적인 영향을 미칠 수 있다.

## 원문 미리보기
<p>ERC-8309, under the §Deduplication amendment proposed in ethereum/ERCs#1826, changes what a mesh does when two vantages disagree about the same observation: instead of silently deduplicating, it preserves the divergence as a first-class store state — single | divergent(committed observation set) | absent — and names an extension point, resolveDivergence, where a declared resolution policy may attach. It deliberately prescribes none.</p>
<p>This companion specification defines what attaches there. It is now public</p>
<aside class="onebox githubrepo" data-onebox-src="https://github.com/damon