---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Draft ERC: AI Inference Token Onchain (AITO) - consumable entitlements to AI inference supply, with metering, authorized consumption and settlement"
author: ""
pub_date: "Fri, 20 Nov 2026 02:25:30 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-20
sources:
  - "https://ethereum-magicians.org/t/draft-erc-ai-inference-token-onchain-aito-consumable-entitlements-to-ai-inference-supply-with-metering-authorized-consumption-and-settlement/30453"
---
# Draft ERC: AI Inference Token Onchain (AITO) - consumable entitlements to AI inference supply, with metering, authorized consumption and settlement

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/draft-erc-ai-inference-token-onchain-aito-consumable-entitlements-to-ai-inference-supply-with-metering-authorized-consumption-and-settlement/30453)  |  Fri, 20 Nov 2026 02:25:30 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** AITO는 온체인 AI 추론 공급에 대한 권한을 보유, 전송 및 소비하기 위한 프레임워크이다.

**리서치 앵글:** 온체인 AI 추론 토큰은 L2 확장성 및 새로운 온체인 서비스 도입과 관련이 있다.

## 원문 미리보기
<p>This topic is the discussion thread for a draft ERC, <strong>AI Inference Token Onchain (AITO)</strong>.</p>
<h2><a name="p-76973-summary-1" class="anchor" href="https://ethereum-magicians.org#p-76973-summary-1" aria-label="Heading link"></a>Summary</h2>
<p>AITO is a framework for holding, transferring and consuming entitlements to AI inference supply on chain.</p>
<p>The “token” in the name is the inference token, the unit in which inference usage is counted. It is the denomination of the entitlement, not a blockchain token. An AITO unit expresses, under a versioned execution specification