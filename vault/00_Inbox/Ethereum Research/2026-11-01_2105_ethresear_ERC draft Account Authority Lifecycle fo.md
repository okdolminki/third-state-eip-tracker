---
source: "Ethereum Research"
source_type: research
title: "ERC draft: Account Authority Lifecycle for STVA"
author: ""
pub_date: "Sun, 01 Nov 2026 10:54:19 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-01
sources:
  - "https://ethresear.ch/t/erc-draft-account-authority-lifecycle-for-stva/26202"
---
# ERC draft: Account Authority Lifecycle for STVA

> 출처: [Ethereum Research](https://ethresear.ch/t/erc-draft-account-authority-lifecycle-for-stva/26202)  |  Sun, 01 Nov 2026 10:54:19 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 계정 권한의 전체 생명주기(발급, 활성화, 감쇠, 검토, 정지, 철회, 복구)를 위한 표준 모델 및 인터페이스를 제안하여 권한 유실을 방지하고 고가치 계정 및 멀티시그의 거버넌스 기반을 제공합니다.

**리서치 앵글:** 이 ERC 초안은 Third State의 주요 리서치 테마인 계정 추상화(EIP-7702)와 직접적으로 연관되며, 계정 권한 관리 및 보안 모델에 대한 심층 분석에 기여합니다.

## 원문 미리보기
<p><strong>Description:</strong></p>
<p>A standard model and interface for the full lifecycle of authority over an account: issuance, activation, attenuation (via Scoped Capabilities), review, suspension, revocation, and recovery. Prevents authority drift (stale owners, modules, or keys that outlive their intended purpose).</p>
<p>Provides the governance backbone that makes Scoped Capability Tokens and independent simulation operationally meaningful for high-value accounts and multisigs.</p>
<p>author: <a class="mention" href="https://ethresear.ch/u/matoboycrypto65">@MATOBOYCRYPTO65</a></p>
<p