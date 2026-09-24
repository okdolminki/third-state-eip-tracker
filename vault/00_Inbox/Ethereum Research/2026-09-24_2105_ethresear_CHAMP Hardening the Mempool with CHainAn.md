---
source: "Ethereum Research"
source_type: research
title: "CHAMP: Hardening the Mempool with CHain-Anchored, Multi-dimensional Peer Protection"
author: ""
pub_date: "Thu, 24 Sep 2026 10:58:21 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-09-24
sources:
  - "https://ethresear.ch/t/champ-hardening-the-mempool-with-chain-anchored-multi-dimensional-peer-protection/26074"
---
# CHAMP: Hardening the Mempool with CHain-Anchored, Multi-dimensional Peer Protection

> 출처: [Ethereum Research](https://ethresear.ch/t/champ-hardening-the-mempool-with-chain-anchored-multi-dimensional-peer-protection/26074)  |  Thu, 24 Sep 2026 10:58:21 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** CHAMP는 무작위 피어 교체 방식의 단점을 보완하여, 체인 앵커링 및 다차원 보호를 통해 멤풀의 보안과 효율성을 강화하는 새로운 피어 관리 시스템을 제안합니다.

**리서치 앵글:** 멤풀 보안 강화는 MEV 완화 및 네트워크 안정성 증진에 기여할 수 있습니다.

## 원문 미리보기
<p><em>Author: <a class="mention" href="https://ethresear.ch/u/cskiraly">@cskiraly</a></em></p>
<h2><a name="p-62624-tldr-1" class="anchor" href="https://ethresear.ch#p-62624-tldr-1" aria-label="Heading link"></a>TL;DR</h2>
<ul>
<li>Clients keep their peer set fresh with <strong>random churn</strong> — periodically dropping random peers. This keeps the network open to newcomers and resistant to eclipse attacks, but it is <strong>blind to peer quality</strong>: it drops our most useful peers as readily as idle ones.</li>
<li>We add <strong>CHAMP</strong>, a set of <strong>protected peer pools</