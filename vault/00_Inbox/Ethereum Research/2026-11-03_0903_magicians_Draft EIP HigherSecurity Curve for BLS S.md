---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Draft EIP: Higher-Security Curve for BLS Signatures"
author: ""
pub_date: "Mon, 02 Nov 2026 14:21:18 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-03
sources:
  - "https://ethereum-magicians.org/t/draft-eip-higher-security-curve-for-bls-signatures/30184"
---
# Draft EIP: Higher-Security Curve for BLS Signatures

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/draft-eip-higher-security-curve-for-bls-signatures/30184)  |  Mon, 02 Nov 2026 14:21:18 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 이더리움 합의 계층의 핵심 BLS 서명 보안 강화를 위해 BLS12-381에서 BLS48-581과 같은 고보안 곡선으로 전환하는 EIP 초안이 논의 중입니다.

**리서치 앵글:** 이더리움 합의 계층의 근본적인 보안 강화는 LST/LRT 구조의 안정성 및 기관 DeFi 도입의 신뢰도에 영향을 미칩니다.

## 원문 미리보기
<p><strong>Category:</strong> EIPs (core subcategory)</p>
<p><strong>Title:</strong> Draft EIP: Higher-Security Curve for BLS Signatures</p>
<hr>
<p>Discussion topic for a draft EIP. It doesn’t have a number or PR yet: <a href="https://gist.github.com/sauliusgrigaitis/6f833d88d91940e0ea64f1cd43ee5842">draft</a>.</p>
<p>This draft specifies how to move the most security-critical consensus-layer BLS signatures from BLS12-381 to a higher-security pairing-friendly curve, with BLS48-581 as the current candidate. RANDAO reveals, selection proofs, and aggregator signatures stay on BLS12-381. It hedge