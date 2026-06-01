---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Draft ERC: Permission Registry — function-scoped delegation for agents, without custody"
author: ""
pub_date: "Mon, 01 Jun 2026 05:36:04 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-01
sources:
  - "https://ethereum-magicians.org/t/draft-erc-permission-registry-function-scoped-delegation-for-agents-without-custody/28670"
---
# Draft ERC: Permission Registry — function-scoped delegation for agents, without custody

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/draft-erc-permission-registry-function-scoped-delegation-for-agents-without-custody/28670)  |  Mon, 01 Jun 2026 05:36:04 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 스마트 컨트랙트의 모든 함수에 대해 ERC20.approve와 유사한 기능 범위 위임 권한을 제공하는 새로운 ERC 초안이 논의 중입니다.

**리서치 앵글:** 스마트 컨트랙트 함수 단위 위임 권한은 기관 DeFi 도입 및 계정 추상화(EIP-7702) 연구에 중요한 영향을 미칠 수 있습니다.

## 원문 미리보기
<p>Hi everyone,</p>
<p>I’m working on a draft ERC for a registry-based delegated authorization primitive and would love feedback before opening the EIP PR.</p>
<p>The objective is to provide a simple primitive for users of a smart contract to give scoped permissions to call functions on a contract on their behalf. What ERC20.approve does to transfers, this proposal wants to do for every function in a contract.</p>
<ul>
<li>
<p>Repo: <a href="https://github.com/yolo-maxi/erc-approval-registry" rel="noopener nofollow ugc">https://github.com/yolo-maxi/erc-approval-registry</a></p>
</li>
<li>
<p>S