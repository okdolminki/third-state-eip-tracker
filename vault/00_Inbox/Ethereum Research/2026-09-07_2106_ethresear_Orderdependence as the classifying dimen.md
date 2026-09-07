---
source: "Ethereum Research"
source_type: research
title: "Order-dependence as the classifying dimension for frame-transaction mempool admission"
author: ""
pub_date: "Mon, 07 Sep 2026 10:49:29 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-09-07
sources:
  - "https://ethresear.ch/t/order-dependence-as-the-classifying-dimension-for-frame-transaction-mempool-admission/25934"
---
# Order-dependence as the classifying dimension for frame-transaction mempool admission

> 출처: [Ethereum Research](https://ethresear.ch/t/order-dependence-as-the-classifying-dimension-for-frame-transaction-mempool-admission/25934)  |  Mon, 07 Sep 2026 10:49:29 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 프레임 트랜잭션의 멤풀 승인 규칙을 유효성 검사가 순서 의존적 상태를 읽는지 여부에 따라 분류하는 방법에 대한 연구.

**리서치 앵글:** 프레임 트랜잭션의 멤풀 승인 규칙 연구는 계정 추상화(EIP-7702) 및 L2 확장성 테마와 밀접하게 연관됩니다.

## 원문 미리보기
<p>The mempool-admission rules being layered onto frame transactions share a single implicit classifier: whether a validity check reads order-dependent state. This note names that classifier, grounds it in the <a href="https://arxiv.org/abs/1901.01930" rel="noopener nofollow ugc">CALM theorem</a> and the <a href="https://cs.brown.edu/~mph/Herlihy91/p124-herlihy.pdf" rel="noopener nofollow ugc">Herlihy consensus hierarchy</a>, and derives the irreducible core it implies.</p>
<h2><a name="p-62337-h-1-problem-1" class="anchor" href="https://ethresear.ch#p-62337-h-1-problem-1"></a>1. Problem</h2>
