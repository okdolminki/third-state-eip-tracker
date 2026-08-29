---
source: "Ethereum Research"
source_type: research
title: "Proposed PQ upgrade for ecrecover"
author: ""
pub_date: "Fri, 28 Aug 2026 15:08:16 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-29
sources:
  - "https://ethresear.ch/t/proposed-pq-upgrade-for-ecrecover/25844"
---
# Proposed PQ upgrade for ecrecover

> 출처: [Ethereum Research](https://ethresear.ch/t/proposed-pq-upgrade-for-ecrecover/25844)  |  Fri, 28 Aug 2026 15:08:16 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 기존 EVM 컨트랙트의 양자 공격 취약성에 대응하기 위해 `ecrecover` opcode를 양자 내성 서명을 지원하도록 업데이트하는 방안이 제안되었습니다.

**리서치 앵글:** 계정 추상화(EIP-7702)를 포함한 서명 관련 연구 및 기관 DeFi 도입의 장기적인 보안 기반에 영향을 미칠 수 있습니다.

## 원문 미리보기
<h1><a name="p-62150-proposed-pq-hotfix-for-ecrecover-1" class="anchor" href="https://ethresear.ch#p-62150-proposed-pq-hotfix-for-ecrecover-1"></a>Proposed PQ hotfix for ecrecover</h1>
<p>Many EVM contracts deployed today use <code>ecrecover</code> to verify ECDSA signatures and are thus vulnerable to quantum attacks. Rather than completely disabling the <code>ecrecover</code> opcode, we can update <code>ecrecover</code> to read post-quantum signatures from EIP-8141 frame transactions. The 65-byte signature <code>(v, r, s)</code> can be used to encode lookup values. A sentinel value would trig