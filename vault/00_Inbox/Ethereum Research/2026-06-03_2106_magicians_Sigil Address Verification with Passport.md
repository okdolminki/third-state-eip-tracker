---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Sigil: Address Verification with Passport - good or bad idea?"
author: ""
pub_date: "Wed, 03 Jun 2026 05:31:35 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-03
sources:
  - "https://ethereum-magicians.org/t/sigil-address-verification-with-passport-good-or-bad-idea/28689"
---
# Sigil: Address Verification with Passport - good or bad idea?

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/sigil-address-verification-with-passport-good-or-bad-idea/28689)  |  Wed, 03 Jun 2026 05:31:35 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** Sigil은 여권당 고유한 널리파이어를 생성하여 이더리움 주소와 연결, 주소 수준의 신원 증명 및 시빌 저항을 가능하게 하는 시스템을 제안한다.

**리서치 앵글:** 주소 수준의 신원 증명 및 시빌 저항은 기관 DeFi 도입 및 RWA 프로토콜의 규제 준수 요구사항을 충족하는 데 기여할 수 있다.

## 원문 미리보기
<blockquote>
<p><strong>TL; DR</strong> - I created Sigil which generates a unique nullifier per passport that can be associated with ethereum addresses. This basically enables proof of personhood at the address level and promotes sybil-resistance, i.e. protocols can enforce one passport per protocol rather than per address.</p>
</blockquote>
<h2><a name="p-70550-overview-1" class="anchor" href="https://ethereum-magicians.org#p-70550-overview-1" aria-label="Heading link"></a><strong>Overview</strong></h2>
<p>I started my web3 journey relatively recently and became interested in privacy/identit