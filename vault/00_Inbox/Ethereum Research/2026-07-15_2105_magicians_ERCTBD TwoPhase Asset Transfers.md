---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-TBD: Two-Phase Asset Transfers"
author: ""
pub_date: "Wed, 15 Jul 2026 07:00:16 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-15
sources:
  - "https://ethereum-magicians.org/t/erc-tbd-two-phase-asset-transfers/29017"
---
# ERC-TBD: Two-Phase Asset Transfers

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-tbd-two-phase-asset-transfers/29017)  |  Wed, 15 Jul 2026 07:00:16 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 발신자가 자산을 에스크로에 잠그고 수신자가 수락해야만 전송이 완료되며, 수신자가 수락하기 전까지 발신자가 취소할 수 있는 '2단계 자산 전송' 표준이 제안되었습니다.

**리서치 앵글:** 기관 DeFi 도입 시 자산 전송의 안정성과 통제력을 높여 기관 투자자의 참여를 촉진할 수 있는 잠재력이 있습니다.

## 원문 미리보기
<p>Hi all,</p>
<p>I am proposing a standard for two-phase transfers: the sender initiates, the asset is locked in<br>
an escrow and bound to a named receiver, and nothing settles until that receiver accepts. Until<br>
someone accepts, the sender can revoke at any time. After a deadline, the sender can reclaim.</p>
<p>Draft: <a href="https://github.com/ethereum/ERCs/pull/1882" class="inline-onebox" rel="noopener nofollow ugc">Two phase asset transfers by muhammadaus · Pull Request #1882 · ethereum/ERCs · GitHub</a></p>
<h2><a name="p-71870-the-problem-1" class="anchor" href="https://ethereum-ma