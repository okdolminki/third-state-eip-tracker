---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8356: Purpose-Bound Third-Party Data Consent"
author: ""
pub_date: "Fri, 31 Jul 2026 04:41:15 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-31
sources:
  - "https://ethereum-magicians.org/t/erc-8356-purpose-bound-third-party-data-consent/29217"
---
# ERC-8356: Purpose-Bound Third-Party Data Consent

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8356-purpose-bound-third-party-data-consent/29217)  |  Fri, 31 Jul 2026 04:41:15 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 제3자 데이터 동의 표준화에 대한 ERC 초안으로, 동의 주체, 수혜자, 위험 부담자가 다른 경우를 다룹니다.

**리서치 앵글:** 기관 DeFi 도입 및 RWA 관련 데이터 공유 시 필요한 정교한 동의 및 권한 관리 메커니즘 구축에 기여할 수 있습니다.

## 원문 미리보기
<p>I would like feedback on a draft ERC before I open a PR.</p>
<p><strong>The one-line version.</strong> Every delegation standard I have found on the Standards Track is two-party: the party who consents is the party who benefits, and the party at risk is the party who signed. I want to standardize the case where those are different people, because that is the shape of consent to use someone’s data.</p>
<p>Disclosure: I am the founder of <a href="http://GenoBank.io" rel="noopener nofollow ugc">GenoBank.io</a>, which builds a decentralized biobanking system in which patients grant researchers 