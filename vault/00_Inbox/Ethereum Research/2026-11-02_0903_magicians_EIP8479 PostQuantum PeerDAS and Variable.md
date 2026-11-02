---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8479: Post-Quantum PeerDAS and Variable-Size Blobs"
author: ""
pub_date: "Sun, 01 Nov 2026 17:22:30 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-02
sources:
  - "https://ethereum-magicians.org/t/eip-8479-post-quantum-peerdas-and-variable-size-blobs/30167"
---
# EIP-8479: Post-Quantum PeerDAS and Variable-Size Blobs

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8479-post-quantum-peerdas-and-variable-size-blobs/30167)  |  Sun, 01 Nov 2026 17:22:30 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** 이 EIP는 PeerDAS에 양자 내성 데이터 가용성 구조를 도입하여 KZG 대신 Keccak-256 머클 커밋먼트와 STARK를 사용하며, 가변 크기 블롭을 허용합니다.

**리서치 앵글:** 이 EIP는 이더리움의 데이터 가용성 레이어 개선을 통해 L2 확장성 및 효율성에 직접적인 영향을 미칩니다.

## 원문 미리보기
<p>Discussion topic for EIP-9999.</p>
<p>This EIP introduces a post-quantum data-availability construction for PeerDAS. It replaces KZG blob commitments and cell proofs with Keccak-256 Merkle commitments and a LeanDA STARK proving the Reed–Solomon encoding relation and correct commitment derivation.</p>
<p>The existing PeerDAS column-custody, sampling, subnet-allocation, and recovery mechanisms remain unchanged. Sampled cells are authenticated using Merkle authentication paths instead of KZG proofs.</p>
<p>The proposal also allows power-of-two blob sizes between 2 KiB and 512 KiB while retaini