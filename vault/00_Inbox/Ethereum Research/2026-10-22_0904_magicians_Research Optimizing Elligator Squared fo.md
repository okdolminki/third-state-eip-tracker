---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "[Research] Optimizing Elligator Squared for BLS Curves via Jacobi Quartics"
author: ""
pub_date: "Wed, 21 Oct 2026 19:30:45 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-22
sources:
  - "https://ethereum-magicians.org/t/research-optimizing-elligator-squared-for-bls-curves-via-jacobi-quartics/30041"
---
# [Research] Optimizing Elligator Squared for BLS Curves via Jacobi Quartics

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/research-optimizing-elligator-squared-for-bls-curves-via-jacobi-quartics/30041)  |  Wed, 21 Oct 2026 19:30:45 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** BLS 서명 공개키 난독화의 계산 오버헤드를 획기적으로 줄이는 최적화 연구로, 기존 방식의 높은 지연 시간 문제를 해결하고자 함.

**리서치 앵글:** BLS 서명 최적화를 통해 LST/LRT 구조의 효율성 및 검증자 프라이버시 개선 가능성.

## 원문 미리보기
<p>Hi everyone,</p>
<p>I’d like to share some recent research on drastically reducing the computational overhead of public key obfuscation for BLS signatures.</p>
<p>While the raw storage of BLS12-381 public keys is great for signature aggregation, it exposes validators to linkability and subgroup membership leakage. Obfuscating these keys into uniform random strings via the Elligator Squared framework is mathematically sound, but typically introduces a massive latency penalty due to costly inverse isogeny maps and heavy cofactor blinding/clearing.</p>
<p>We have developed an optimized obfusca