---
source: "Ethereum Research"
source_type: research
title: "Extraction Is Conserved: From MEV to GEV"
author: ""
pub_date: "Mon, 25 May 2026 18:47:38 +0000"

importance: high
action: read_now
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-05-31
sources:
  - "https://ethresear.ch/t/extraction-is-conserved-from-mev-to-gev/24953"
---
# Extraction Is Conserved: From MEV to GEV

> 출처: [Ethereum Research](https://ethresear.ch/t/extraction-is-conserved-from-mev-to-gev/24953)  |  Mon, 25 May 2026 18:47:38 +0000

## AI 분석
**중요도:** high | **액션:** read_now

**요약:** MEV는 너무 좁은 개념이며, 추출은 프로토콜 계층 전반에 걸쳐 보존되므로 부분적인 해결책은 추출을 제거하는 것이 아니라 재배치할 뿐이라는 GEV(Generalized Extractable Value) 개념을 제시한다.

**리서치 앵글:** MEV를 GEV로 확장하고 추출 보존을 주장하며, 이는 MEV, DEX 경쟁구도, L2 확장성, 기관 DeFi 도입 테마에 핵심적이다.

## 원문 미리보기
<p><em>Part 3 of the airgap-closure series. Following on from Part 1 (the airgap problem in DeFi) and Part 2 (augmented mechanism design as methodology), this post argues that the MEV abstraction is too narrow, and the right unit of analysis is generalized extractable value. Extraction is conserved across protocol layers, which means partial fixes relocate rather than eliminate.</em></p>
<h2><a name="p-60134-the-narrow-frame-1" class="anchor" href="https://ethresear.ch#p-60134-the-narrow-frame-1"></a>The narrow frame</h2>
<p>MEV discourse since Daian et al. has converged on transaction-orderin