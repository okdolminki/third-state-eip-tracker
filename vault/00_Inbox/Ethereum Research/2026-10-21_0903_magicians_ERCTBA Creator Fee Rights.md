---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-TBA: Creator Fee Rights"
author: ""
pub_date: "Tue, 20 Oct 2026 15:30:57 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-21
sources:
  - "https://ethereum-magicians.org/t/erc-tba-creator-fee-rights/30027"
---
# ERC-TBA: Creator Fee Rights

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-tba-creator-fee-rights/30027)  |  Tue, 20 Oct 2026 15:30:57 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 토큰 발행 시 발생하는 창작자 수수료 스트림에 대한 표준 인터페이스 초안으로, 수수료 수령인, 누적액, 청구 메커니즘 및 수령인 변경 규칙의 불변성을 정의합니다.

**리서치 앵글:** DeFi 프로토콜의 토큰 경제 모델 및 가치 흐름에 대한 이해를 심화하며, 향후 DEX 경쟁 구도 및 기관 DeFi 도입 시 토큰 표준에 영향을 줄 수 있습니다.

## 원문 미리보기
<p>Every token launch creates a creator fee stream, and each launchpad models it differently. This draft is one interface for a launched token’s creator fee stream: who receives it (<code>feeRecipient</code>), what it has earned since launch (<code>accruedTotal</code>), what is claimable, a <code>claim</code> anyone can trigger that always pays the recipient, and a recipient that only the current recipient can change (ERC-173’s rule, applied per token). No administrator, upgrade or launchpad setting may redirect a launched token’s recipient or lower its creator share, and fees are accounted wh