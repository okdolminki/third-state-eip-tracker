---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8476: Permanent EOA Delegation Opt-Out"
author: ""
pub_date: "Fri, 30 Oct 2026 16:35:42 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-31
sources:
  - "https://ethereum-magicians.org/t/eip-8476-permanent-eoa-delegation-opt-out/30134"
---
# EIP-8476: Permanent EOA Delegation Opt-Out

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8476-permanent-eoa-delegation-opt-out/30134)  |  Fri, 30 Oct 2026 16:35:42 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8476은 EOA(Externally Owned Account)가 EIP-7702 기반의 위임 기능을 영구적으로 비활성화할 수 있도록 하는 제안입니다.

**리서치 앵글:** 계정 추상화(EIP-7702)의 EOA 위임 기능과 관련된 사용자 제어 및 보안 측면을 연구합니다.

## 원문 미리보기
<p>Discussion thread for the draft Core EIP <strong>Permanent EOA Delegation Opt-Out</strong>.</p>
<p>PR: <a href="https://github.com/ethereum/EIPs/pull/12600" class="inline-onebox" rel="noopener nofollow ugc">Add EIP: Permanent EOA Delegation Opt-Out by nicolashw · Pull Request #12600 · ethereum/EIPs · GitHub</a></p>
<h2><a name="p-75939-abstract-1" class="anchor" href="https://ethereum-magicians.org#p-75939-abstract-1" aria-label="Heading link"></a>Abstract</h2>
<p>Allow an externally owned account (EOA) to permanently disable <a href="https://eips.ethereum.org/EIPS/eip-7702" rel="noopener n