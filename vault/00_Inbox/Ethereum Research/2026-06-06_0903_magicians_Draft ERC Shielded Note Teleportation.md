---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Draft ERC: Shielded Note Teleportation"
author: ""
pub_date: "Fri, 05 Jun 2026 16:39:51 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-06
sources:
  - "https://ethereum-magicians.org/t/draft-erc-shielded-note-teleportation/28721"
---
# Draft ERC: Shielded Note Teleportation

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/draft-erc-shielded-note-teleportation/28721)  |  Fri, 05 Jun 2026 16:39:51 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-7503의 zkwormhole 개념을 확장하여, 사용자가 자산을 공개적으로 인출 및 재예치할 필요 없이 기존 프라이버시 프로토콜 간에 자산을 이동할 수 있도록 하는 새로운 ERC 표준을 제안합니다.

**리서치 앵글:** 프라이버시 프로토콜 간 상호운용성 개선은 기관의 DeFi 도입 시 요구되는 프라이버시 및 자산 관리 효율성 증대에 기여할 수 있습니다.

## 원문 미리보기
<p>Hi everyone,</p>
<p>I am proposing a new ERC standard that I would greatly appreciate feedback on.</p>
<p>While experimenting with improvements and other ways to apply the concept of zkwormholes from <a href="https://eips.ethereum.org/EIPS/eip-7503" rel="noopener nofollow ugc">EIP-7503</a>, I discovered a way for it to enable interoperability between privacy protocols, even existing ones such as Tornado Cash, 0xbow’s Privacy Pools and Railgun. Users can move assets from one privacy protocol to another without publicly withdrawing and re-depositing. This is achieved by the user creating a no