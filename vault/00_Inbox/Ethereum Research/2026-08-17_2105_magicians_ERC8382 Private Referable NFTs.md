---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8382: Private Referable NFTs"
author: ""
pub_date: "Mon, 17 Aug 2026 07:22:51 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-17
sources:
  - "https://ethereum-magicians.org/t/erc-8382-private-referable-nfts/29442"
---
# ERC-8382: Private Referable NFTs

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8382-private-referable-nfts/29442)  |  Mon, 17 Aug 2026 07:22:51 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 이 ERC는 ERC-721을 확장하여 참조되는 NFT 정보(라벨, 가중치 등)를 공개하지 않고도 NFT 간의 비공개 참조 약정을 가능하게 하며, 영지식 증명 등 프라이버시 보호 기술을 활용할 수 있습니다.

**리서치 앵글:** 프라이버시 보호 기능을 갖춘 NFT 참조는 기관 DeFi 도입 시 자산의 비공개성 및 상호운용성 확보에 기여할 수 있습니다.

## 원문 미리보기
<h2><a name="p-73339-abstract-1" class="anchor" href="https://ethereum-magicians.org#p-73339-abstract-1" aria-label="Heading link"></a><strong>Abstract</strong></h2>
<p>This ERC extends <a>ERC-721</a> with interoperable commitments to private NFT-to-NFT references. A token can publish one or more reference commitments without disclosing the referenced NFT, reference label, weight, or authorization material. Implementations expose a common discovery interface, may require a zero-knowledge or other privacy-preserving proof at mint time, and may support later selective disclosure of individual re