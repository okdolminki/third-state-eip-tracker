---
source: "Ethereum Research"
source_type: research
title: "Exploring post-quantum signature aggregation for EIP-8288"
author: ""
pub_date: "Mon, 16 Nov 2026 16:33:57 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-17
sources:
  - "https://ethresear.ch/t/exploring-post-quantum-signature-aggregation-for-eip-8288/26261"
---
# Exploring post-quantum signature aggregation for EIP-8288

> 출처: [Ethereum Research](https://ethresear.ch/t/exploring-post-quantum-signature-aggregation-for-eip-8288/26261)  |  Mon, 16 Nov 2026 16:33:57 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8288을 위한 양자 내성 서명 집계 방안을 탐색하며, 지갑 생태계의 임계값 서명, 키 파생 등 보안 모델 개선을 논의합니다.

**리서치 앵글:** EIP-8288의 양자 내성 서명 집계 논의는 계정 추상화(EIP-7702)와 연관된 지갑 보안 및 기능 개선에 대한 리서치 테마와 관련이 있습니다.

## 원문 미리보기
<p><em>by Manuel B. Santos (<a class="mention" href="https://ethresear.ch/u/manel1874">@manel1874</a>) <a href="https://www.multivmlabs.com/" rel="noopener nofollow ugc">MultiVM Labs</a></em>.</p>
<h1><a name="p-63028-motivation-1" class="anchor" href="https://ethresear.ch#p-63028-motivation-1" aria-label="Heading link"></a>Motivation</h1>
<p>Nowadays, the wallet ecosystem contains a plethora of features depending on different security models. These features require classical signatures to support threshold signing, key derivation or implementations that fit hardware signers. These properties 