---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Draft ERC: Policy-Enforced Agent Accounts"
author: ""
pub_date: "Sat, 21 Nov 2026 16:07:33 +0000"

importance: medium
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-22
sources:
  - "https://ethereum-magicians.org/t/draft-erc-policy-enforced-agent-accounts/30467"
---
# Draft ERC: Policy-Enforced Agent Accounts

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/draft-erc-policy-enforced-agent-accounts/30467)  |  Sat, 21 Nov 2026 16:07:33 +0000

## AI 분석
**중요도:** medium | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 에이전트 계정의 외부 정책 서명자 보호 여부, 정책 내용, 거부 사유 등을 표준적으로 확인할 수 있는 방법이 없어, 이를 위한 읽기 및 증거 레이어 ERC 초안이 제안되었습니다.

**리서치 앵글:** 에이전트 계정의 정책 기반 보호 및 검증 표준화는 기관 DeFi 도입과 계정 추상화(EIP-7702) 연구 테마와 밀접하게 연관됩니다.

## 원문 미리보기
<p>Hi all. We’d like feedback on a draft ERC for a problem we hit while running agent accounts in production: <strong>there is no standard way for an app, wallet or lender to tell whether an agent’s account is protected by an external policy signer, what that policy allows, or why something was refused.</strong></p>
<p><strong>What it adds:</strong> a read-and-evidence layer. It doesn’t define how anything is enforced.</p>
<ul>
<li><strong>Discovery (ERC-165 <code>0xcc16d336</code>):</strong> <code>policySigner(account)</code>, <code>policyOf(account)</code>, <code>pendingPolicyOf(account)</co