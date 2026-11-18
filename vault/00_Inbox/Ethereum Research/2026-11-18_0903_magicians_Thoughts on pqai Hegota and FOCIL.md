---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Thoughts on pqai, Hegota, and FOCIL"
author: ""
pub_date: "Tue, 17 Nov 2026 16:10:16 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-18
sources:
  - "https://ethereum-magicians.org/t/thoughts-on-pqai-hegota-and-focil/30421"
---
# Thoughts on pqai, Hegota, and FOCIL

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/thoughts-on-pqai-hegota-and-focil/30421)  |  Tue, 17 Nov 2026 16:10:16 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 이더리움의 포스트-양자, 포스트-AI 암호화 전환을 가속화하되, 다른 EIP 개발을 병행하여 진행해야 한다는 논의.


## 원문 미리보기
<p><em>By <a href="https://x.com/soispoke" rel="noopener nofollow ugc">Thomas Thiery</a></em></p>
<p><strong>tldr: Let’s accelerate pqai without rushing or stopping everything else. We can parallelise workstreams to keep shipping EIPs that are ready while the cryptography, designs, and specs for PQ are being finalised.</strong></p>
<p><strong>We need to accelerate Ethereum’s transition to post-quantum, post-AI cryptography</strong>. Let’s take this as a given.</p>
<p>There are two ways to think about what we need to do to enable this acceleration.</p>
<ol>
<li>
<p><strong>We deprioritise every