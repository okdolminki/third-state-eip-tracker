---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8395: Signed HTTP Requests with Ethereum"
author: ""
pub_date: "Wed, 26 Aug 2026 01:50:44 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-26
sources:
  - "https://ethereum-magicians.org/t/erc-8395-signed-http-requests-with-ethereum/29514"
---
# ERC-8395: Signed HTTP Requests with Ethereum

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8395-signed-http-requests-with-ethereum/29514)  |  Wed, 26 Aug 2026 01:50:44 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** ERC-8395는 EIP-712 위임 권한을 활용하여 인증된 HTTP 요청을 위한 위임 서명 HTTP 요청 표준을 논의합니다.

**리서치 앵글:** EIP-712 기반 위임 서명 HTTP 요청은 기관 DeFi 도입 및 계정 추상화(EIP-7702)와 관련된 보안 및 사용자 경험 개선에 기여할 수 있습니다.

## 원문 미리보기
<p>Discussion for ERC-8395: Delegated Signed HTTP Requests — an ERC-8128 extension with recursive, attenuating EIP-712 Delegation Grants for authenticated HTTP requests.</p>
<aside class="onebox githubpullrequest" data-onebox-src="https://github.com/ethereum/ERCs/pull/1967">
  <header class="source">

      <a href="https://github.com/ethereum/ERCs/pull/1967" target="_blank" rel="noopener nofollow ugc">github.com/ethereum/ERCs</a>
  </header>

  <article class="onebox-body">
    <div class="github-row" data-github-private-repo="false">



    <div class="github-icon-container" title="Pull Requ