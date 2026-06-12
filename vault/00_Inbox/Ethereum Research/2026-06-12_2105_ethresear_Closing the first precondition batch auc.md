---
source: "Ethereum Research"
source_type: research
title: "Closing the first precondition: batch auctions remove the ordering surface, they do not relocate it"
author: ""
pub_date: "Fri, 12 Jun 2026 01:11:40 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-12
sources:
  - "https://ethresear.ch/t/closing-the-first-precondition-batch-auctions-remove-the-ordering-surface-they-do-not-relocate-it/25160"
---
# Closing the first precondition: batch auctions remove the ordering surface, they do not relocate it

> 출처: [Ethereum Research](https://ethresear.ch/t/closing-the-first-precondition-batch-auctions-remove-the-ordering-surface-they-do-not-relocate-it/25160)  |  Fri, 12 Jun 2026 01:11:40 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 배치 경매는 MEV의 표면적 추출 문제를 해결하지만, 근본적인 시퀀싱 권한이라는 추출의 전제 조건은 여전히 존재함을 지적한다.

**리서치 앵글:** MEV 테마와 직접적으로 연관되며, 배치 경매가 DEX 경쟁 구도 및 L2 확장성에 미칠 잠재적 영향에 대한 심층 연구 필요성을 시사한다.

## 원문 미리보기
<p><em>Airgap closure, Part 4. Follows “Extraction is conserved: from MEV to GEV.”</em></p>
<p>In Part 3 the framing got corrected in the replies, and the correction matters enough to lead with it. <strong>The conserved quantity is not extraction across channels. It is extraction across preconditions.</strong> A channel is a surface. A precondition is the structural fact that makes the surface extractable in the first place. Sequencing privilege is one precondition, and it surfaces as both ordering extraction (MEV proper) and liquidation-ordering extraction. Close the surface while the precond