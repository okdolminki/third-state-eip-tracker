---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC idea: NFT Controlled Application Spaces from Voiddeeds"
author: ""
pub_date: "Tue, 03 Nov 2026 03:35:59 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-03
sources:
  - "https://ethereum-magicians.org/t/erc-idea-nft-controlled-application-spaces-from-voiddeeds/30258"
---
# ERC idea: NFT Controlled Application Spaces from Voiddeeds

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-idea-nft-controlled-application-spaces-from-voiddeeds/30258)  |  Tue, 03 Nov 2026 03:35:59 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** NFT가 블록체인 상의 애플리케이션 공간을 제어하고, NFT 보유자가 수수료를 관리하며 빌더가 앱을 게시할 수 있는 Voiddeeds 프로토콜의 ERC 아이디어를 논의합니다.

**리서치 앵글:** NFT 기반 애플리케이션 공간 제어는 L2 확장성 및 새로운 온체인 애플리케이션 구조에 대한 잠재적 영향을 가집니다.

## 원문 미리보기
<p>I’m building Voiddeeds, a protocol where an NFT represents control over a logical application space on a blockchain. The testnet is running at <a href="https://voiddeeds.xyz" rel="noopener nofollow ugc">https://voiddeeds.xyz</a>. I’d like to discuss whether the interfaces around these spaces would be useful as an ERC, or whether they fit better as an extension to existing work.</p>
<p>The NFT holder controls the space’s toll and payment recipients. Builders can publish independent applications in that space, and users interact with them through its Runtime. A space here is an execution and 