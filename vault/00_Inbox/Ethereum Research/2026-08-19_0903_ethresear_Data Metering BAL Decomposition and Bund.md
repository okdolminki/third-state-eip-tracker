---
source: "Ethereum Research"
source_type: research
title: "Data Metering, BAL Decomposition, and Bundle Pricing Under EIP-7999"
author: ""
pub_date: "Tue, 18 Aug 2026 16:40:22 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-19
sources:
  - "https://ethresear.ch/t/data-metering-bal-decomposition-and-bundle-pricing-under-eip-7999/25747"
---
# Data Metering, BAL Decomposition, and Bundle Pricing Under EIP-7999

> 출처: [Ethereum Research](https://ethresear.ch/t/data-metering-bal-decomposition-and-bundle-pricing-under-eip-7999/25747)  |  Tue, 18 Aug 2026 16:40:22 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-7999 및 EIP-7928(BAL) 하에서 데이터 측정, BAL 분해, 번들 가격 책정 등 이더리움 프로토콜의 기술적 개선 사항을 다룹니다.

**리서치 앵글:** EIP 관련 내용은 MEV 전략, L2 확장성, 그리고 전반적인 DeFi 프로토콜의 트랜잭션 비용 및 처리 방식에 중대한 영향을 미칠 수 있습니다.

## 원문 미리보기
<p><em>by <a href="https://x.com/William33203632" rel="noopener nofollow ugc">Fei Wu</a> - This work was conducted during my internship at the EF. I thank my mentor <a class="mention" href="https://ethresear.ch/u/misilva73">@misilva73</a> for valuable discussions, feedback, and comments.</em></p>
<h2><a name="p-61953-overview-1" class="anchor" href="https://ethresear.ch#p-61953-overview-1"></a>Overview</h2>
<p><a href="https://github.com/ethereum/EIPs/blob/0603514569547869ae2531a4e5b2b62875888db3/EIPS/eip-7928.md" rel="noopener nofollow ugc">EIP-7928</a> specifies Block-Level Access Lists (BAL