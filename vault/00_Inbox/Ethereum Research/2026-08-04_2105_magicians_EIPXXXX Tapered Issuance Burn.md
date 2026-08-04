---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-XXXX: Tapered Issuance Burn"
author: ""
pub_date: "Tue, 04 Aug 2026 09:30:30 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-04
sources:
  - "https://ethereum-magicians.org/t/eip-xxxx-tapered-issuance-burn/29263"
---
# EIP-XXXX: Tapered Issuance Burn

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-xxxx-tapered-issuance-burn/29263)  |  Tue, 04 Aug 2026 09:30:30 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 이 EIP는 검증자 보상의 부분적 소각을 통해 ETH 발행 곡선을 수정하는 내용을 담고 있습니다.

**리서치 앵글:** ETH 발행량 및 검증자 보상 변경은 LST/LRT 구조의 경제성에 직접적인 영향을 미칠 수 있습니다.

## 원문 미리보기
<p>Discussion topic for EIP-XXXX: Tapered Issuance Burn</p>
<p>This EIP implements a modification to the ETH issuance curve by way of a partial burn of validator rewards.</p>
<p><strong>References</strong></p>
<p>This core principle is in large part based on <a href="https://github.com/pa7x1/ethereum-issuance" rel="noopener nofollow ugc">prior work by pa7x1</a>. A key refinement - the per-duty version of the burn, is due to Anders Elowsson (key insight contained in <a href="https://ethresear.ch/t/properties-of-issuance-offsets-and-increased-penalties-under-low-zero-negative-issuance-policies/2