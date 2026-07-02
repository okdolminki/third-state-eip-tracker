---
source: "Ethereum Research"
source_type: research
title: "SPREAD: Extending GossipSub with Efficient Anonymous Dissemination"
author: ""
pub_date: "Thu, 02 Jul 2026 01:27:45 +0000"

importance: medium
action: weekly_review
pre_eip_signal: false

note_type: research_post
auto_generated: true
source_date: 2026-07-02
sources:
  - "https://ethresear.ch/t/spread-extending-gossipsub-with-efficient-anonymous-dissemination/25343"
---
# SPREAD: Extending GossipSub with Efficient Anonymous Dissemination

> 출처: [Ethereum Research](https://ethresear.ch/t/spread-extending-gossipsub-with-efficient-anonymous-dissemination/25343)  |  Thu, 02 Jul 2026 01:27:45 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review

**요약:** SSV 네트워크 DAO의 지원을 받아 작성된 이 연구는 이더리움 P2P 네트워크의 핵심인 GossipSub을 확장하여 노드의 익명성을 보장하면서도 효율적으로 메시지를 전파하는 SPREAD 프로토콜을 제안합니다.

**리서치 앵글:** LST/LRT의 기반이 되는 분산 검증인 기술(DVT) 및 검증인 노드의 IP 익명성 확보를 통한 네트워크 보안 및 MEV 차단 효과 측면에서 분석할 가치가 있습니다.

## 원문 미리보기
<p>Authors: Diogo Cardoso, Matheus Franco, Rodrigo Rodrigues</p>
<p><em>Acknowledgement:</em> This work was supported by a <a href="https://forum.ssv.network/t/ssv-x-university-of-lisbon-grant-proposal-blockchain-research-p2p/1939" rel="noopener nofollow ugc">grant</a> from the <strong>SSV Network DAO</strong> awarded to the University of Lisbon.</p>
<p>A draft spec was proposed to <code>libp2p/specs</code> (<a href="https://github.com/libp2p/specs/pull/726" rel="noopener nofollow ugc">PR #726</a>).<br>
A reference implementation is open for <code>go-libp2p-pubsub</code> (<a href="https://gith