---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8355: Precompiles for ML-DSA verification"
author: ""
pub_date: "Fri, 31 Jul 2026 00:55:36 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-31
sources:
  - "https://ethereum-magicians.org/t/eip-8355-precompiles-for-ml-dsa-verification/29211"
---
# EIP-8355: Precompiles for ML-DSA verification

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8355-precompiles-for-ml-dsa-verification/29211)  |  Fri, 31 Jul 2026 00:55:36 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8355는 FIPS 204 ML-DSA 서명 검증을 위한 세 가지 사전 컴파일을 제안하며, 이는 이더리움에 양자 내성 암호(PQC) 기능을 추가하는 것을 목표로 합니다.

**리서치 앵글:** 이 EIP는 이더리움의 핵심 암호화 기능을 강화하여 장기적인 보안을 확보하며, 이는 기관 DeFi 도입 및 L2 확장성의 근본적인 신뢰도에 영향을 미칠 수 있습니다.

## 원문 미리보기
<p>Discussion topic for EIP-8355 (<a href="https://github.com/ethereum/EIPs/pull/12048">PR #12048</a>)</p>
<p>Three precompiles that verify FIPS 204 ML-DSA signatures at NIST security levels II, III, and V (parameter sets ML-DSA-44, 65, and 87).</p>
<p>This overlaps with <a href="https://eips.ethereum.org/EIPS/eip-8051">EIP-8051</a>, and I want to be upfront that it isn’t a competing design so much as four specific disagreements with it. If those are resolved in EIP-8051, I would rather this be folded into it than shipped alongside or in lieu of.</p>
<p>Each precompile takes a single concatena