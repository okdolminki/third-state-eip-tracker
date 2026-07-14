---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Token-Bound Executable Skills — the artifact identity & integrity layer under skill registries (ERC-721 extension)"
author: ""
pub_date: "Mon, 13 Jul 2026 20:26:02 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-07-14
sources:
  - "https://ethereum-magicians.org/t/token-bound-executable-skills-the-artifact-identity-integrity-layer-under-skill-registries-erc-721-extension/29005"
---
# Token-Bound Executable Skills — the artifact identity & integrity layer under skill registries (ERC-721 extension)

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/token-bound-executable-skills-the-artifact-identity-integrity-layer-under-skill-registries-erc-721-extension/29005)  |  Mon, 13 Jul 2026 20:26:02 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 오프체인 런타임(LLM 에이전트 포함)이 온체인 앵커를 통해 검증하고 실행할 수 있는 '실행 가능한 스킬'에 토큰을 바인딩하는 ERC-721 확장 제안.

**리서치 앵글:** 토큰에 실행 가능한 스킬을 바인딩하여 LLM 에이전트 등 오프체인 런타임이 활용하는 방식은 계정 추상화(EIP-7702)와 연관되어 미래 온체인 상호작용의 복잡성을 높일 수 있음.

## 원문 미리보기
<p><strong>Summary</strong></p>
<p>We propose an ERC-721 extension that binds a token to an <strong>executable skill</strong>: a package of files, led by a primary Markdown document, that an off-chain runtime (including LLM agent runtimes) can fetch from anywhere, verify byte-for-byte against on-chain anchors, and execute.</p>
<p>On-chain, each token carries a <code>SkillBinding</code>: <code>mdHash</code> (SHA-256 of the plaintext primary document — a commitment that survives encryption), <code>packageHash</code> (SHA-256 of a deterministically encoded, content-addressed object graph — the Sk