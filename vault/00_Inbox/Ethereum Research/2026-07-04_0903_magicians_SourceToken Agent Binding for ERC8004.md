---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Source-Token Agent Binding for ERC-8004"
author: ""
pub_date: "Fri, 03 Jul 2026 18:18:57 +0000"

importance: medium
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-04
sources:
  - "https://ethereum-magicians.org/t/source-token-agent-binding-for-erc-8004/28920"
---
# Source-Token Agent Binding for ERC-8004

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/source-token-agent-binding-for-erc-8004/28920)  |  Fri, 03 Jul 2026 18:18:57 +0000

## AI 분석
**중요도:** medium | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** ERC-8004와 ERC-8217을 통해 기존 NFT를 새로운 온체인 에이전트(Agent)로 활용하여 사용자 신원 및 상호작용 방식을 개선하려는 논의입니다.

**리서치 앵글:** NFT를 활용한 온체인 신원 및 에이전트 바인딩 논의로, 계정 추상화(EIP-7702) 테마와 밀접하게 연관되어 사용자 경험 및 기관 DeFi 도입에 영향을 줄 수 있습니다.

## 원문 미리보기
<p><strong>Source-Token Agent Binding for ERC-8004</strong> — companion to <a href="https://ethereum-magicians.org/t/add-erc-8217-agent-nft-identity-bindings/28339">ERC-8217</a> (Agent NFT Identity Bindings, <a class="mention" href="https://ethereum-magicians.org/u/nxt3d">@nxt3d</a>). Co-authored with <a class="mention" href="https://ethereum-magicians.org/u/tmerlini">@TMerlini</a>.</p>
<p><strong>The gap.</strong> ERC-8004 assumes an agent is minted fresh. In practice the most natural agents are derived from NFTs people already hold — a PFP, a membership token, a game character. Existing stan