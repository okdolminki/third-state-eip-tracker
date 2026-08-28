---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Tacet: a trust-minimized encrypted mempool for the OP Stack (working prototype, seeking feedback)"
author: ""
pub_date: "Thu, 27 Aug 2026 18:24:29 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-08-28
sources:
  - "https://ethereum-magicians.org/t/tacet-a-trust-minimized-encrypted-mempool-for-the-op-stack-working-prototype-seeking-feedback/29529"
---
# Tacet: a trust-minimized encrypted mempool for the OP Stack (working prototype, seeking feedback)

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/tacet-a-trust-minimized-encrypted-mempool-for-the-op-stack-working-prototype-seeking-feedback/29529)  |  Thu, 27 Aug 2026 18:24:29 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** Tacet은 OP Stack을 위한 EVM-native 암호화된 멤풀로, 트랜잭션 순서가 확정된 후에만 복호화되어 실행됨으로써 프론트러닝을 방지합니다.

**리서치 앵글:** MEV 방지 및 L2 확장성 개선을 위한 암호화된 멤풀 기술로, Third State의 MEV 및 L2 확장성 연구 테마와 직접적으로 연관됩니다.

## 원문 미리보기
<p>Tacet is an EVM-native encrypted mempool for the OP Stack. (The name is the musical direction <em>tacet</em>: the voice is present in the score but stays silent until its cue - which is exactly what an encrypted transaction does in a committed block.) Transactions are threshold-encrypted before they reach the sequencer; the ordering is committed before anyone (including the sequencer) can read a transaction, and only after the block is fixed do t-of-n keypers release decryption shares (decrypt-then-execute). This takes content-based front-running off the table for everyone who is not the se