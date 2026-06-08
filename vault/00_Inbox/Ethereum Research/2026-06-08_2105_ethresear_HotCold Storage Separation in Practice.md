---
source: "Ethereum Research"
source_type: research
title: "Hot-Cold Storage Separation in Practice"
author: ""
pub_date: "Mon, 08 Jun 2026 04:19:59 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-08
sources:
  - "https://ethresear.ch/t/hot-cold-storage-separation-in-practice/25119"
---
# Hot-Cold Storage Separation in Practice

> 출처: [Ethereum Research](https://ethresear.ch/t/hot-cold-storage-separation-in-practice/25119)  |  Mon, 08 Jun 2026 04:19:59 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8188은 계정 및 저장 슬롯의 마지막 변경 시점을 기록하는 타임스탬프를 추가하여, 비활성 상태 쓰기에 더 높은 비용을 부과하는 방안을 제안한다.

**리서치 앵글:** EIP-8188의 핫-콜드 스토리지 분리 및 비용 정책은 L2 확장성에 중대한 영향을 미칠 수 있다.

## 원문 미리보기
<h1><a name="p-60514-hot-cold-storage-separation-in-practice-1" class="anchor" href="https://ethresear.ch#p-60514-hot-cold-storage-separation-in-practice-1"></a>Hot-Cold Storage Separation in Practice</h1>
<p><a href="https://eips.ethereum.org/EIPS/eip-8188" rel="noopener nofollow ugc">EIP-8188</a> adds a consensus-visible timestamp to every account and storage slot, recording when each was last mutated. Its pricing rules use that field to charge more for writing to write-inactive state, but the field itself is the part that matters here because it gives every client the same signal for which 