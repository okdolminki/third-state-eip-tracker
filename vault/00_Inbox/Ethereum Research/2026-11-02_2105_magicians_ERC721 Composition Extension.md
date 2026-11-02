---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-721 Composition Extension"
author: ""
pub_date: "Mon, 02 Nov 2026 10:32:48 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-02
sources:
  - "https://ethereum-magicians.org/t/erc-721-composition-extension/30181"
---
# ERC-721 Composition Extension

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-721-composition-extension/30181)  |  Mon, 02 Nov 2026 10:32:48 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** ERC-721 토큰이 자체 컨테이너에 자산을 보유하고, 토큰이 존재하는 동안 자산이 컨테이너를 벗어나지 않으며, 어떤 계약이든 토큰이 발행될 때 포함된 자산을 읽을 수 있도록 하는 확장 기능에 대한 논의입니다.

**리서치 앵글:** NFT가 다양한 자산을 컨테이너 형태로 보유하고 그 내용을 투명하게 확인할 수 있게 함으로써 RWA 토큰화 및 기관 DeFi 도입 시 복합 자산 관리의 표준화에 기여할 수 있습니다.

## 원문 미리보기
<p>An ERC-721 extension for tokens that hold assets in a container of their own: nothing leaves the container while the token exists, and any contract can read what the token was minted with.</p>
<p>It grew out of the two ERC-721 extensions <a class="mention" href="https://ethereum-magicians.org/u/jay">@jay</a>  suggested in the <a href="https://ethereum-magicians.org/t/erc-6551-non-fungible-token-bound-accounts/13030/241">ERC-6551 thread</a>: one to read who burned a token, now <a href="https://ethereum-magicians.org/t/erc-8423-erc-721-burn-record-extension/29732">ERC-8423</a>, and one for th