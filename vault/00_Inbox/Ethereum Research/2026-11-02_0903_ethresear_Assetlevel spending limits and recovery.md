---
source: "Ethereum Research"
source_type: research
title: "Asset-level spending limits and recovery: should rate limiting live in the asset rather than the account?"
author: ""
pub_date: "Sun, 01 Nov 2026 17:15:34 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-02
sources:
  - "https://ethresear.ch/t/asset-level-spending-limits-and-recovery-should-rate-limiting-live-in-the-asset-rather-than-the-account/26205"
---
# Asset-level spending limits and recovery: should rate limiting live in the asset rather than the account?

> 출처: [Ethereum Research](https://ethresear.ch/t/asset-level-spending-limits-and-recovery-should-rate-limiting-live-in-the-asset-rather-than-the-account/26205)  |  Sun, 01 Nov 2026 17:15:34 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 계정 수준이 아닌 자산(토큰 컨트랙트) 수준에서 지출 한도 및 복구 기능을 적용하여 기존 보안 취약점(특히 Allowance)을 해결하자는 제안.

**리서치 앵글:** 계정 추상화(EIP-7702) 및 기관 DeFi 도입과 관련된 자산 보안 아키텍처의 근본적인 변화를 탐구.

## 원문 미리보기
<p>Most key-compromise defenses today (smart wallets, ERC-7579 modules, social recovery, EIP-7702 delegation) enforce policy in the account’s code. ERC-8403 continues this: spend limits and unlock times are authorities committed under the account’s root.</p>
<p>I’d like to probe a different placement: enforcing rate limits at the <strong>asset</strong>: the token contract for ERC-20s, and eventually the protocol itself for native ETH.</p>
<p><strong>Motivation.</strong> Account-level policy only binds while the account’s code is in the transfer path. Two gaps:</p>
<ol>
<li><em>Allowances</em>: