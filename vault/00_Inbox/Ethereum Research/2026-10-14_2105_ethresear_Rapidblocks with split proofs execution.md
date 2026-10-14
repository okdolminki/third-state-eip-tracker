---
source: "Ethereum Research"
source_type: research
title: "Rapidblocks with split proofs: execution proofs that outlive their state"
author: ""
pub_date: "Wed, 14 Oct 2026 07:58:50 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-14
sources:
  - "https://ethresear.ch/t/rapidblocks-with-split-proofs-execution-proofs-that-outlive-their-state/26157"
---
# Rapidblocks with split proofs: execution proofs that outlive their state

> 출처: [Ethereum Research](https://ethresear.ch/t/rapidblocks-with-split-proofs-execution-proofs-that-outlive-their-state/26157)  |  Wed, 14 Oct 2026 07:58:50 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 블록 실행 증명을 세 부분으로 분리하여 트랜잭션 실행 증명과 상태 루트 연결 증명을 분리하고, 헤더가 입력값을 커밋하는 새로운 증명 방식을 제안합니다.

**리서치 앵글:** L2 확장성 및 효율적인 블록 검증 방식에 대한 근본적인 개선 방안을 제시하여, L2 프로토콜의 성능과 보안에 중대한 영향을 미칠 수 있습니다.

## 원문 미리보기
<p>Author: <a class="mention" href="https://ethresear.ch/u/cskiraly">@cskiraly</a></p>
<p><strong>TL;DR</strong></p>
<ul>
<li><strong>Split proofs</strong>: a block’s execution proof splits in three. <span class="math">\Pi_T</span> proves that the transactions, run on the block’s <em>inputs</em>, the values it reads, give its outputs; it names no state root. <span class="math">\Pi_\mathrm{in}</span> and <span class="math">\Pi_\mathrm{out}</span> tie inputs and outputs to state roots, and are Merkle work.</li>
<li><strong>Proofs over committed inputs</strong>: the header commits to the inputs i