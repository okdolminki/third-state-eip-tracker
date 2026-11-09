---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Who can upgrade 7 tokenized treasury/gold tokens on Ethereum? A read-only look at upgrade control"
author: ""
pub_date: "Mon, 09 Nov 2026 03:47:13 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-09
sources:
  - "https://ethereum-magicians.org/t/who-can-upgrade-7-tokenized-treasury-gold-tokens-on-ethereum-a-read-only-look-at-upgrade-control/30313"
---
# Who can upgrade 7 tokenized treasury/gold tokens on Ethereum? A read-only look at upgrade control

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/who-can-upgrade-7-tokenized-treasury-gold-tokens-on-ethereum-a-read-only-look-at-upgrade-control/30313)  |  Mon, 09 Nov 2026 03:47:13 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 이더리움 상 7개 토큰화된 국채/금 토큰의 업그레이드 제어 방식을 분석한 결과, EOA, 멀티시그, 타임락 등 다양한 제어 구조가 발견되었습니다.

**리서치 앵글:** RWA 및 기관 DeFi 도입 관점에서 토큰화된 자산의 업그레이드 제어 방식과 보안 취약성 분석에 활용.

## 원문 미리보기
<p>I read the upgrade control of 7 tokenized treasury and gold fund tokens on Ethereum straight from the chain. Snapshot: 9 Nov 2026. Read-only; nothing was tested on live contracts.</p>
<p><strong>Result</strong> (7 tokens I looked at, not a market ranking):</p>
<ul>
<li>3: the upgrade owner is one externally owned address (no contract code), no on-chain delay</li>
<li>2: Safe multisig, 4-of-7, no delay found</li>
<li>1: older multisig, 3-of-6, no delay found</li>
<li>1: timelock, 24h minimum delay</li>
</ul>
<p><strong>What this does NOT say:</strong> that any key is stored badly (it may sit