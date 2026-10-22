---
source: "Ethereum Research"
source_type: research
title: "SEACAST: fast, lean broadcast for Ethereum, with an executable spec and a formal model"
author: ""
pub_date: "Wed, 21 Oct 2026 15:48:38 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-22
sources:
  - "https://ethresear.ch/t/seacast-fast-lean-broadcast-for-ethereum-with-an-executable-spec-and-a-formal-model/26167"
---
# SEACAST: fast, lean broadcast for Ethereum, with an executable spec and a formal model

> 출처: [Ethereum Research](https://ethresear.ch/t/seacast-fast-lean-broadcast-for-ethereum-with-an-executable-spec-and-a-formal-model/26167)  |  Wed, 21 Oct 2026 15:48:38 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 이더리움 내 대형 페이로드를 지연 없이 효율적으로 전파하여 홈 빌더의 경쟁력을 높이고 탈중앙화를 지원하는 브로드캐스트 프로토콜 SEACAST를 제안합니다.

**리서치 앵글:** 블록 전파 지연 단축을 통해 MEV 빌더 중앙화를 완화하고 L2 데이터 가용성(DA) 확장성에 중기적 영향을 줄 수 있습니다.

## 원문 미리보기
<p><em>This post follows <a href="https://ethresear.ch/t/informed-diffusion-making-home-builders-publish-fast/26151">Informed Diffusion: making home builders publish fast</a> (2026).</em></p>
<p>Author: <a class="mention" href="https://ethresear.ch/u/cskiraly">@cskiraly</a></p>
<h2><a name="p-62800-tldr-1" class="anchor" href="https://ethresear.ch#p-62800-tldr-1" aria-label="Heading link"></a>TL;DR</h2>
<ul>
<li><strong>Ethereum has more and more large objects to broadcast, and little time for each.</strong> Today’s payloads are small and datacenters carry them, which is much of why mainnet is