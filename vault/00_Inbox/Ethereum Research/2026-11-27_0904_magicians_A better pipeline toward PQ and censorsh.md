---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "A better pipeline toward PQ and censorship resistant Ethereum"
author: ""
pub_date: "Thu, 26 Nov 2026 12:47:29 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-27
sources:
  - "https://ethereum-magicians.org/t/a-better-pipeline-toward-pq-and-censorship-resistant-ethereum/30522"
---
# A better pipeline toward PQ and censorship resistant Ethereum

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/a-better-pipeline-toward-pq-and-censorship-resistant-ethereum/30522)  |  Thu, 26 Nov 2026 12:47:29 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 양자 내성 및 검열 저항성을 달성하기 위해 차기 하드포크 범위를 재조정하고 탈동기화 합의(Decoupled Consensus) 파이프라인을 체계화하자는 제안입니다.

**리서치 앵글:** 검열 저항성 개선 및 합의 구조 변경은 장기적으로 L1 MEV 생태계와 L2 최종성(finality) 아키텍처에 영향을 미칠 수 있습니다.

## 원문 미리보기
<p>Ethereum is accelerating the post-quantum transition. To that end, we’re rescoping Hegotá. I think we should decide what to ship by looking at where each feature sits in the research, development and testing pipeline and how much work can move forward in parallel.</p>
<p>PQ Decoupled Consensus is seen as an ideal design for PQ-resistant Ethereum. Decoupled Consensus is the culmination of more than four years of research and would significantly improve the consensus layer. It would also make the PQ transition easier by moving signature aggregation off the critical path. However, it’s still i