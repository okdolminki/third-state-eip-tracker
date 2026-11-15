---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Draft ERC: Generative Engine Optimization Framework (GEOF) — attributable declarations, observation commitments and profiles for how generative engines represent objects"
author: ""
pub_date: "Sat, 14 Nov 2026 16:58:47 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-15
sources:
  - "https://ethereum-magicians.org/t/draft-erc-generative-engine-optimization-framework-geof-attributable-declarations-observation-commitments-and-profiles-for-how-generative-engines-represent-objects/30396"
---
# Draft ERC: Generative Engine Optimization Framework (GEOF) — attributable declarations, observation commitments and profiles for how generative engines represent objects

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/draft-erc-generative-engine-optimization-framework-geof-attributable-declarations-observation-commitments-and-profiles-for-how-generative-engines-represent-objects/30396)  |  Sat, 14 Nov 2026 16:58:47 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** GEOF는 생성 엔진(AI 검색, 에이전트 런타임 등)이 객체를 표현하고 측정하며 검증하는 방식을 정의하는 프레임워크입니다.

**리서치 앵글:** 생성형 엔진이 DeFi 객체를 표현하는 방식은 기관 DeFi 도입 및 에이전트 기반 상호작용에 영향을 줄 수 있습니다.

## 원문 미리보기
<h2><a name="p-76641-summary-1" class="anchor" href="https://ethereum-magicians.org#p-76641-summary-1" aria-label="Heading link"></a>Summary</h2>
<p>GEOF is a descriptive framework for recording how generative engines — answer engines, AI search surfaces, and agent runtimes with discovery layers — represent an object, how that representation is measured, and how independent parties exchange and verify the measurements.</p>
<p>It lets independent parties declare, for the same object or dissemination process, what they observed; and, when a dissemination intent has been declared, how much of it 