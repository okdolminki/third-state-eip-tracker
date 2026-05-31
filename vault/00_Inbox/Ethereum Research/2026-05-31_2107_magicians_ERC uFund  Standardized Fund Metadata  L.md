---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC: uFund - Standardized Fund Metadata & Lifecycle Interface"
author: ""
pub_date: "Fri, 29 May 2026 04:57:23 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-05-31
sources:
  - "https://ethereum-magicians.org/t/erc-ufund-standardized-fund-metadata-lifecycle-interface/28660"
---
# ERC: uFund - Standardized Fund Metadata & Lifecycle Interface

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-ufund-standardized-fund-metadata-lifecycle-interface/28660)  |  Fri, 29 May 2026 04:57:23 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** uFund는 토큰화된 투자 펀드를 위한 표준화된 메타데이터 및 라이프사이클 인터페이스를 정의하는 ERC 제안입니다.

**리서치 앵글:** 토큰화된 투자 펀드의 표준화된 인터페이스를 제공하여 RWA 및 기관 DeFi 도입에 중요한 영향을 미칠 수 있습니다.

## 원문 미리보기
<h2><a name="p-70416-summary-1" class="anchor" href="https://ethereum-magicians.org#p-70416-summary-1" aria-label="Heading link"></a>Summary</h2>
<p>uFund is a proposed ERC interface for tokenized investment funds.</p>
<p>It defines a minimal, read-heavy, base-token-agnostic interface for querying fund-level information such as:</p>
<ul>
<li>Net Asset Value (NAV) per share</li>
<li>NAV freshness/staleness</li>
<li>fund lifecycle state</li>
<li>declared and paid distributions</li>
<li>basic fee metadata</li>
<li>subscription and redemption windows</li>
<li>maturity date</li>
</ul>
<p>It also de