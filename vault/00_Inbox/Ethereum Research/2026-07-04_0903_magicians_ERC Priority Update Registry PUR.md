---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC: Priority Update Registry (PUR)"
author: ""
pub_date: "Fri, 03 Jul 2026 20:14:50 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-04
sources:
  - "https://ethereum-magicians.org/t/erc-priority-update-registry-pur/28921"
---
# ERC: Priority Update Registry (PUR)

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-priority-update-registry-pur/28921)  |  Fri, 03 Jul 2026 20:14:50 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EVM 기반 PropAMM을 위한 Priority Update Registry (PUR) ERC 초안이 제안되었으며, 이는 이미 이더리움에서 상당한 거래량을 처리하고 있어 표준화가 추진 중이다.

**리서치 앵글:** 새로운 AMM 표준 제안으로 DEX 경쟁 구도 및 운영 방식에 미칠 영향 분석이 필요하다.

## 원문 미리보기
<p>gm,</p>
<p>Here is a draft contract standard for PropAMMs on the EVM (and similar use cases). <a href="https://etherscan.io/address/0xda7afeed01fe625cf15d187a19f94b45f00b8c5f" rel="noopener nofollow ugc">An instance of this contract</a> is live on Ethereum since May ‘26 and handles almost all of the propAMM volume across multiple builders. We’re hoping to standardise this across EVM chains.</p>
<p><a href="https://github.com/ethereum/ERCs/pull/1852" rel="noopener nofollow ugc">PR Link</a>; <a href="https://ethereum-magicians.org/t/erc-priority-update-registry-pur/28921">reference implementa