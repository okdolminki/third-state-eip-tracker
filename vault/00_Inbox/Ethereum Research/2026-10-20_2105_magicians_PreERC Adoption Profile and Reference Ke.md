---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Pre-ERC: Adoption Profile and Reference Kernel for EOAs Adopting Code via SETCODEFROM"
author: ""
pub_date: "Tue, 20 Oct 2026 11:02:56 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-20
sources:
  - "https://ethereum-magicians.org/t/pre-erc-adoption-profile-and-reference-kernel-for-eoas-adopting-code-via-setcodefrom/30020"
---
# Pre-ERC: Adoption Profile and Reference Kernel for EOAs Adopting Code via SETCODEFROM

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/pre-erc-adoption-profile-and-reference-kernel-for-eoas-adopting-code-via-setcodefrom/30020)  |  Tue, 20 Oct 2026 11:02:56 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8298과 EIP-8151은 EOA가 자체 주소에 코드를 채택하여 스마트 계정으로 전환하고, 이 과정에서 `ecrecover`의 동작을 변경하여 보안을 강화하는 방안을 논의합니다.

**리서치 앵글:** EOA가 스마트 계정으로 전환하는 방식과 관련된 EIP 논의로, Third State의 '계정 추상화' 리서치 테마와 직접적으로 연관됩니다.

## 원문 미리보기
<h2><a name="p-75454-tldr-1" class="anchor" href="https://ethereum-magicians.org#p-75454-tldr-1" aria-label="Heading link"></a>TL;DR</h2>
<p><a href="https://eips.ethereum.org/EIPS/eip-8298" rel="noopener nofollow ugc">EIP-8298</a> (<code>SETCODEFROM</code>) lets an EOA adopt account code at its own address. <a href="https://eips.ethereum.org/EIPS/eip-8151" rel="noopener nofollow ugc">EIP-8151</a> makes <code>ecrecover</code> stop returning addresses that hold regular code. Together, they stop a secp256k1 key from sending transactions or passing <code>ecrecover</code> for that account, without