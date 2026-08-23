---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8390: Remove the Sync Committee"
author: ""
pub_date: "Sun, 23 Aug 2026 09:30:18 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-23
sources:
  - "https://ethereum-magicians.org/t/eip-8390-remove-the-sync-committee/29486"
---
# EIP-8390: Remove the Sync Committee

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8390-remove-the-sync-committee/29486)  |  Sun, 23 Aug 2026 09:30:18 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8390은 동기화 위원회 및 관련 구성 요소를 제거하고, Altair 라이트 클라이언트 프로토콜을 폐지하며, 합의 발행량을 2/64 감소시키는 것을 제안합니다.

**리서치 앵글:** 동기화 위원회 제거는 L2 확장성 및 라이트 클라이언트 기반의 계정 추상화 구현에 잠재적 영향을 미칠 수 있습니다.

## 원문 미리보기
<p>Discussion thread for EIP-8390.</p>
<p>Removes the sync committee, its aggregate, subnets, domains and rewards, and the Altair light client protocol built on it. <code>SYNC_REWARD_WEIGHT</code> is removed and not redistributed, so consensus issuance falls by 2/64.</p>
<h4><a name="p-73502-update-log-1" class="anchor" href="https://ethereum-magicians.org#p-73502-update-log-1" aria-label="Heading link"></a>Update Log</h4>
<ul>
<li>2026-08-20: initial draft</li>
</ul>
<h4><a name="p-73502-external-reviews-2" class="anchor" href="https://ethereum-magicians.org#p-73502-external-reviews-2" aria-l