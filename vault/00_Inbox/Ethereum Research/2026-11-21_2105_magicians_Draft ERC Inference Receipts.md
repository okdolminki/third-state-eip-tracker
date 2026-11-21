---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Draft ERC: Inference Receipts"
author: ""
pub_date: "Sat, 21 Nov 2026 11:58:51 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-21
sources:
  - "https://ethereum-magicians.org/t/draft-erc-inference-receipts/30464"
---
# Draft ERC: Inference Receipts

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/draft-erc-inference-receipts/30464)  |  Sat, 21 Nov 2026 11:58:51 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 온체인 결제 후 모델 엔드포인트가 제공한 서비스 내용을 증명하기 위해 호출당 서명된 영수증과 일일 머클 루트를 온체인에 발행하는 ERC 초안.

**리서치 앵글:** 온체인 결제 서비스의 투명성과 감사 가능성을 높여 기관 DeFi 도입에 필요한 신뢰 모델을 강화할 수 있음.

## 원문 미리보기
<p>An agent that pays a model endpoint per call can prove it paid, since the payment settles on chain. It cannot prove what the payment bought, or check later that the endpoint’s account of a day matches the calls it made. This draft defines a signed receipt per paid call and a daily Merkle root over those receipts, published on chain.</p>
<p>Draft: <a href="https://github.com/kurokawasato/ERCs/blob/add-erc-inference-receipts/ERCS/erc-draft_inference_receipts.md" rel="noopener nofollow ugc">erc-draft_inference_receipts.md</a>. The pull request to ethereum/ERCs follows as soon as this thread ex