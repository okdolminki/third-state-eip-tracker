---
source: "Ethereum Research"
source_type: research
title: "ERC-8403: an account as one hash, and post-quantum keys"
author: ""
pub_date: "Sun, 11 Oct 2026 04:24:19 +0000"

importance: medium
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-11
sources:
  - "https://ethresear.ch/t/erc-8403-an-account-as-one-hash-and-post-quantum-keys/26147"
---
# ERC-8403: an account as one hash, and post-quantum keys

> 출처: [Ethereum Research](https://ethresear.ch/t/erc-8403-an-account-as-one-hash-and-post-quantum-keys/26147)  |  Sun, 11 Oct 2026 04:24:19 +0000

## AI 분석
**중요도:** medium | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** ERC-8403은 네이티브 계정 추상화에서 키 관리 방식(키 추가/철회)을 정의하고, EIP-8288 기반의 양자 내성 키를 고려하는 초안입니다.

**리서치 앵글:** 이 제안은 Third State의 주요 리서치 테마인 계정 추상화(EIP-7702)와 직접적으로 연관되며, 향후 기관 DeFi 도입의 핵심 요소인 보안 및 키 관리 표준에 영향을 미칠 것입니다.

## 원문 미리보기
<p>native account abstraction lets an account hold many keys. it does not say what “add a key” or “revoke a key” means. each account model defines that in its own way, and wallets have to follow all of them.</p>
<p><a href="https://github.com/ethereum/ERCs/pull/1979" rel="noopener nofollow ugc">erc-8403</a> is my draft for that part. this post describes it first, and then asks what the same account looks like with post-quantum keys on top of eip-8288.</p>
<h2><a name="p-62757-the-account-stores-one-root-1" class="anchor" href="https://ethresear.ch#p-62757-the-account-stores-one-root-1" aria-la