---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8407: Extensible Contract Metadata"
author: ""
pub_date: "Wed, 02 Sep 2026 08:41:22 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-09-02
sources:
  - "https://ethereum-magicians.org/t/erc-8407-extensible-contract-metadata/29565"
---
# ERC-8407: Extensible Contract Metadata

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8407-extensible-contract-metadata/29565)  |  Wed, 02 Sep 2026 08:41:22 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 기존 온체인 메타데이터 노출 방식의 비효율성을 개선하기 위한 확장 가능한 컨트랙트 메타데이터 ERC 초안에 대한 피드백 요청.

**리서치 앵글:** L2 확장성 및 계정 추상화(EIP-7702)와 관련하여 컨트랙트의 정보 노출 방식 개선 가능성을 시사함.

## 원문 미리보기
<p>We’d like to gather feedback on a draft ERC, <strong>Extensible Contract Metadata</strong>, before opening a PR to <code>ethereum/ERCs</code>.</p>
<h2><a name="p-73793-the-problem-1" class="anchor" href="https://ethereum-magicians.org#p-73793-the-problem-1" aria-label="Heading link"></a>The problem</h2>
<p>Onchain metadata is conventionally exposed through purpose-built functions — one function per piece of metadata, each returning a specific value. Adopting a <em>new</em> piece of metadata therefore means adding a new function, i.e. <strong>changing the contract’s code</strong>. For alread