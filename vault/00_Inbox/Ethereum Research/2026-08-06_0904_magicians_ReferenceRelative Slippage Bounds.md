---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Reference-Relative Slippage Bounds"
author: ""
pub_date: "Wed, 05 Aug 2026 14:50:36 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-06
sources:
  - "https://ethereum-magicians.org/t/reference-relative-slippage-bounds/29292"
---
# Reference-Relative Slippage Bounds

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/reference-relative-slippage-bounds/29292)  |  Wed, 05 Aug 2026 14:50:36 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 이 ERC 초안은 토큰 스왑 시 참조 가격 기반 슬리피지 보호를 위한 인터페이스를 정의합니다.

**리서치 앵글:** 이 ERC는 토큰 스왑의 슬리피지 보호를 개선하여 DEX 경쟁 구도에 영향을 미칠 수 있습니다.

## 원문 미리보기
<p>Posting the draft spec for a small ERC. It reuses ERC-7726 for the reference price, so it stays intentionally narrow. Feedback welcome, especially on the open questions at the end.</p>
<p><code>requires: ERC-165, ERC-7726</code></p>
<h2><a name="p-72679-abstract-1" class="anchor" href="https://ethereum-magicians.org#p-72679-abstract-1" aria-label="Heading link"></a>Abstract</h2>
<p>This proposal defines an interface for reference-relative slippage protection on token swaps. Instead of committing to a static <code>minAmountOut</code> at signing time, the caller supplies a slippage policy, an