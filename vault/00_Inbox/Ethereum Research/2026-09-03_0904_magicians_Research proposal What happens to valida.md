---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Research proposal: What happens to validator control if EIP-8363 works"
author: ""
pub_date: "Wed, 02 Sep 2026 19:14:27 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-09-03
sources:
  - "https://ethereum-magicians.org/t/research-proposal-what-happens-to-validator-control-if-eip-8363-works/29568"
---
# Research proposal: What happens to validator control if EIP-8363 works

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/research-proposal-what-happens-to-validator-control-if-eip-8363-works/29568)  |  Wed, 02 Sep 2026 19:14:27 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8363이 유효성 검사기 제어, 솔로 스테이킹 및 스테이킹 시장에 미칠 잠재적 영향에 대한 연구 제안입니다.

**리서치 앵글:** EIP-8363이 유효성 검사기 제어 및 스테이킹 시장에 미치는 영향은 LST/LRT 구조의 안정성과 경제성에 직접적인 영향을 미칩니다.

## 원문 미리보기
<p>I’ve been reading through the EIP-8363 discussion and the earlier work on issuance, solo staking, validator economics, Maximum Viable Security, and formal models of the staking market. EIP-8363 itself is here: <a href="https://eips.ethereum.org/EIPS/eip-8363" rel="noopener nofollow ugc">https://eips.ethereum.org/EIPS/eip-8363</a></p>
<p>There is already enough serious work in this area that I don’t think the useful thing is to build another generic model showing that different kinds of stakers respond differently to changes in yield. That question has been studied. Some of the work I’m star