---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Checking that a deployed contract still runs the audited commit"
author: ""
pub_date: "Mon, 09 Nov 2026 08:43:10 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-09
sources:
  - "https://ethereum-magicians.org/t/checking-that-a-deployed-contract-still-runs-the-audited-commit/30318"
---
# Checking that a deployed contract still runs the audited commit

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/checking-that-a-deployed-contract-still-runs-the-audited-commit/30318)  |  Mon, 09 Nov 2026 08:43:10 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 현재 익스플로러의 코드 검증은 배포된 컨트랙트가 감사받은 커밋을 실행하는지 보장하지 않으며, 특히 업그레이드 가능한 프록시의 경우 감사 이후 코드 무결성에 대한 불확실성이 존재한다.

**리서치 앵글:** 배포된 컨트랙트의 감사받은 코드 실행 여부 검증 문제는 기관 DeFi 도입의 핵심 보안 요소이며, 커버리지 프로토콜의 신뢰도에 직접적인 영향을 미친다.

## 원문 미리보기
<p>The verified badge on an explorer shows that some source compiles to the code at an address. It doesn’t say which commit that source came from, and on a proxy it says nothing about the logic behind it. So when someone asks whether an upgradeable contract still runs the commit its audit covered, the honest answer is often a guess, and a few upgrades after launch the guess can be wrong.</p>
<p>I’ve been writing down what a real check needs. Most of it is small.</p>
<h3><a name="p-76393-rebuilding-the-commit-1" class="anchor" href="https://ethereum-magicians.org#p-76393-rebuilding-the-commit-1