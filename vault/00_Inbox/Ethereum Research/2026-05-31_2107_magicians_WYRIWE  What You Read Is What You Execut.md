---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "WYRIWE - What You Read Is What You Execute (Input Provenance for Verifiable AI Inference)"
author: ""
pub_date: "Thu, 28 May 2026 11:06:49 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-05-31
sources:
  - "https://ethereum-magicians.org/t/wyriwe-what-you-read-is-what-you-execute-input-provenance-for-verifiable-ai-inference/28655"
---
# WYRIWE - What You Read Is What You Execute (Input Provenance for Verifiable AI Inference)

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/wyriwe-what-you-read-is-what-you-execute-input-provenance-for-verifiable-ai-inference/28655)  |  Thu, 28 May 2026 11:06:49 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** WYRIWE는 온체인 AI 추론 입력의 출처를 검증하기 위한 트리플 해시 커밋먼트 스킴 및 EIP-712 증명 프로필을 정의하는 제안된 ERC에 대한 논의입니다.

**리서치 앵글:** 온체인 AI 에이전트 시스템의 입력 검증은 향후 기관 DeFi 도입 시 신뢰성 확보에 기여할 수 있습니다.

## 원문 미리보기
<p>This thread is the discussion home for WYRIWE, a proposed ERC defining a triple-hash commitment scheme and EIP-712 attestation profile for AI inference input provenance.</p>
<h2><a name="p-70363-the-problem-1" class="anchor" href="https://ethereum-magicians.org#p-70363-the-problem-1" aria-label="Heading link"></a>The Problem</h2>
<p>On-chain AI agent systems (ERC-8004, ERC-8263, ERC-8274) can attest to which model ran and what output was produced, but no standard defines how to commit to <em>what input was actually fed to the model</em>. An agent can sanitize, rewrite, or substitute the use