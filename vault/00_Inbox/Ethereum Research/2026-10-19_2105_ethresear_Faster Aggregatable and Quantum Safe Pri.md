---
source: "Ethereum Research"
source_type: research
title: "Faster, Aggregatable and Quantum Safe Privacy Pools"
author: ""
pub_date: "Mon, 19 Oct 2026 10:59:11 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-19
sources:
  - "https://ethresear.ch/t/faster-aggregatable-and-quantum-safe-privacy-pools/26163"
---
# Faster, Aggregatable and Quantum Safe Privacy Pools

> 출처: [Ethereum Research](https://ethresear.ch/t/faster-aggregatable-and-quantum-safe-privacy-pools/26163)  |  Mon, 19 Oct 2026 10:59:11 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 토네이도 캐시를 양자 내성 SNARK인 Flock으로 포팅하여 프라이버시 풀의 양자 안전성을 확보하고, 기존 풀이 이산 로그 문제 공격에 대비할 수 있는 복구 프로토콜을 제안한다.

**리서치 앵글:** 기관 DeFi 도입을 위한 필수적인 프라이버시 인프라의 양자 안전성 및 장기 보안 강화.

## 원문 미리보기
<p>In collaboration with <a class="mention" href="https://ethresear.ch/u/winderica">@winderica</a></p>
<p><em>TLDR: we port Tornado Cash to Flock, a post-quantum binary-field SNARK, proving a depth-32 withdrawal over SHA-256 in under 30 ms, and describe a simple recovery protocol, requiring only that wallets derive note secrets from a seed, that lets existing pools survive a discrete log break.</em></p>
<h2><a name="p-62794-introduction-1" class="anchor" href="https://ethresear.ch#p-62794-introduction-1" aria-label="Heading link"></a>Introduction</h2>
<p>Privacy pools such as Tornado Cash rest