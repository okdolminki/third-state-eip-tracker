---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8408: eth/73 - Indexed Cell Requests"
author: ""
pub_date: "Thu, 03 Sep 2026 08:39:18 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-09-03
sources:
  - "https://ethereum-magicians.org/t/eip-8408-eth-73-indexed-cell-requests/29575"
---
# EIP-8408: eth/73 - Indexed Cell Requests

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8408-eth-73-indexed-cell-requests/29575)  |  Thu, 03 Sep 2026 08:39:18 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8408은 이기종 GetCells 및 Cells 메시지에 대한 인덱싱된 마스크 인코딩을 제안하여 이더리움 네트워크의 데이터 요청 효율성을 개선합니다.

**리서치 앵글:** 이더리움 네트워크의 데이터 처리 효율성 개선은 장기적으로 L2 확장성에 간접적인 영향을 미칠 수 있습니다.

## 원문 미리보기
<p>Hi everyone,</p>
<p>EIP 8408 proposes indexed mask encoding for heterogeneous <code>GetCells</code> and <code>Cells</code> messages while preserving the existing shared mask encoding for uniform requests.</p>
<h2><a name="p-73824-motivation-1" class="anchor" href="https://ethereum-magicians.org#p-73824-motivation-1" aria-label="Heading link"></a>Motivation</h2>
<p>The <code>eth/72</code> <code>GetCells</code> message applies one cell mask to every transaction hash in a request.</p>
<p>When every transaction requires the same cells, this representation is compact and efficient. When transact