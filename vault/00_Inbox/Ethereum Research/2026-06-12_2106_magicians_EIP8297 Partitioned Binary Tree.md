---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8297: Partitioned Binary Tree"
author: ""
pub_date: "Fri, 12 Jun 2026 02:24:02 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-12
sources:
  - "https://ethereum-magicians.org/t/eip-8297-partitioned-binary-tree/28776"
---
# EIP-8297: Partitioned Binary Tree

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8297-partitioned-binary-tree/28776)  |  Fri, 12 Jun 2026 02:24:02 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 기존 헥사리 패트리샤 트라이를 대체할 새로운 이진 상태 트리를 도입하여 계정, 스토리지, 컨트랙트 코드를 단일 트리로 통합하고, 계정 데이터를 256개 단위로 그룹화하여 지역성을 높이며, 트리를 구역으로 분할하는 EIP-8297 제안.

**리서치 앵글:** 이더리움의 근본적인 상태 트리 구조 변경으로 L2 확장성에 대한 잠재적 영향을 분석.

## 원문 미리보기
<h2><a name="p-70910-abstract-1" class="anchor" href="https://ethereum-magicians.org#p-70910-abstract-1" aria-label="Heading link"></a>Abstract</h2>
<p>Introduce a new binary state tree to replace the hexary Patricia tries. Account and storage tries are merged into a single tree with 32-byte keys that also holds contract code. Account data is broken into independent leaves grouped by 256 to provide locality.</p>
<p>The tree is partitioned into zones. The high 4 bits of every key are a zone identifier that labels the category of state the key holds: account headers, contract code, or storage. S