---
source: "Ethereum Research"
source_type: research
title: "Post-quantum signatureless authorization with recursive verification"
author: ""
pub_date: "Fri, 30 Oct 2026 07:13:28 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-30
sources:
  - "https://ethresear.ch/t/post-quantum-signatureless-authorization-with-recursive-verification/26196"
---
# Post-quantum signatureless authorization with recursive verification

> 출처: [Ethereum Research](https://ethresear.ch/t/post-quantum-signatureless-authorization-with-recursive-verification/26196)  |  Fri, 30 Oct 2026 07:13:28 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 양자 컴퓨터 위협에 대비하여 기존 디지털 서명을 대체할 수 있는 양자 내성 또는 서명 없는 권한 부여 방식과 재귀적 검증에 대한 연구.

**리서치 앵글:** 양자 내성 서명 및 서명 없는 권한 부여 방식은 EIP-7702와 같은 계정 추상화의 장기적인 보안 및 구현에 필수적인 요소.

## 원문 미리보기
<p>Digital signatures control who can spend funds, issue commands and authorize requests. Widely used schemes rely on factoring or discrete logarithms, assumptions threatened by Shor’s quantum algorithm. The post-quantum transition therefore reaches the mechanism used to establish authority itself.</p>
<p>Post-quantum signatures provide replacements with different security assumptions, key sizes, signature sizes and verification costs. Applications that also prove execution must express that verification in their proof arithmetic.</p>
<p>Signatureless authorization takes a direct proof-of-know