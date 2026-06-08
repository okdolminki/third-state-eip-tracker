---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Time-Delayed Access Control"
author: ""
pub_date: "Mon, 08 Jun 2026 06:30:02 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-08
sources:
  - "https://ethereum-magicians.org/t/time-delayed-access-control/28741"
---
# Time-Delayed Access Control

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/time-delayed-access-control/28741)  |  Mon, 08 Jun 2026 06:30:02 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 권한 부여 및 박탈에 설정 가능한 지연 시간을 도입하여 권한 상승 공격을 방어하는 스마트 계약 접근 제어 표준(ERC) 제안입니다.

**리서치 앵글:** 기관 DeFi 도입 및 주요 프로토콜(Aave, Lido 등)의 거버넌스 및 멀티시그 보안 강화를 위한 시간 지연 제어 표준으로서 연구 가치가 있습니다.

## 원문 미리보기
<p>This ERC provides time-delayed role management in access control, where role grants and revocations take effect after a configurable delay, providing a defense window against privilege escalation.</p>
<h2><a name="p-70695-abstract-1" class="anchor" href="https://ethereum-magicians.org#p-70695-abstract-1" aria-label="Heading link"></a>Abstract</h2>
<p>This ERC introduces a minimal interface for time-delayed role management in smart contract access control systems. A “delayed role activation” is a role change (grant or revocation) that enters a pending state for a configurable delay period be