---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Draft ERC: Evaluated Work Records"
author: ""
pub_date: "Thu, 19 Nov 2026 08:32:47 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-19
sources:
  - "https://ethereum-magicians.org/t/draft-erc-evaluated-work-records/30447"
---
# Draft ERC: Evaluated Work Records

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/draft-erc-evaluated-work-records/30447)  |  Thu, 19 Nov 2026 08:32:47 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** ERC-8004의 한계를 보완하여, 에스크로 정산 작업에 대한 평가 기록을 온체인에서 증거와 함께 확인할 수 있도록 하는 ERC 초안이 제안되었습니다.

**리서치 앵글:** 계정 추상화(EIP-7702)와 연계하여 온체인 작업의 신뢰성 있는 평가 및 기록 메커니즘을 구축하는 데 기여할 수 있습니다.

## 원문 미리보기
<p>An <a href="https://ethereum-magicians.org/t/erc-8004-trustless-agents/25098">ERC-8004</a> feedback entry can name a task, but nothing ties its score to paid work. This draft posts one entry per escrow-settled task, with evidence checkable against the escrow’s logs.</p>
<p>Draft: <a href="https://github.com/kurokawasato/ERCs/blob/add-erc-evaluated-work-records/ERCS/erc-draft_evaluated_work_records.md" rel="noopener nofollow ugc">erc-draft_evaluated_work_records.md</a>. The pull request to ethereum/ERCs follows as soon as this thread exists, since the draft’s preamble links here.</p>
<p>For 