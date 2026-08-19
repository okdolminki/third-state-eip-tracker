---
source: "Ethereum Research"
source_type: research
title: "Formally Verified Security for PQ-DAS / leanDA"
author: ""
pub_date: "Tue, 18 Aug 2026 15:35:50 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-19
sources:
  - "https://ethresear.ch/t/formally-verified-security-for-pq-das-leanda/25746"
---
# Formally Verified Security for PQ-DAS / leanDA

> 출처: [Ethereum Research](https://ethresear.ch/t/formally-verified-security-for-pq-das-leanda/25746)  |  Tue, 18 Aug 2026 15:35:50 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 포스트 양자 데이터 가용성 샘플링(PQ-DAS)의 보안을 Lean 증명 보조기를 사용하여 형식적으로 검증하는 연구입니다.

**리서치 앵글:** 이더리움 L2 확장성의 핵심 구성 요소인 데이터 가용성 샘플링(DAS)의 보안 검증과 관련되어 L2 확장성 테마와 연관됩니다.

## 원문 미리보기
<h1><a name="p-61952-formally-verified-security-for-pq-das-1" class="anchor" href="https://ethresear.ch#p-61952-formally-verified-security-for-pq-das-1"></a>Formally Verified Security for PQ-DAS</h1>
<p><em>Thanks to Alex Hicks for feedback and discussion.</em></p>
<p><em>The post and a detailed security proof outline was written by the human author, the translation to Lean was done with massive help of AI.</em></p>
<p><em>Disclaimer. The lean code here proves statements about an abstract scheme, under assumptions about abstract building blocks. In particular, it does not prove security of any