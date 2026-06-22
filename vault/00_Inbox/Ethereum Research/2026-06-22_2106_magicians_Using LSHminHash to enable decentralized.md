---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "Using LSH/minHash to enable decentralized nft marketplaces"
author: ""
pub_date: "Mon, 22 Jun 2026 04:13:46 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-06-22
sources:
  - "https://ethereum-magicians.org/t/using-lsh-minhash-to-enable-decentralized-nft-marketplaces/28839"
---
# Using LSH/minHash to enable decentralized nft marketplaces

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/using-lsh-minhash-to-enable-decentralized-nft-marketplaces/28839)  |  Mon, 22 Jun 2026 04:13:46 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** 탈중앙화 NFT 마켓플레이스를 위해 LSH/MinHash를 활용하여 NFT 특성 간 유사도를 온체인에서 계산하는 방안을 제안합니다.


## 원문 미리보기
<p>Hello!</p>
<p>I’ve been researching how to enable decentralized nft marketplaces.  Currently most if not all are centralized with an offchain orderbook to facilitate trading over malleable offchain metadata.  The idea I’ve been playing with is to utilize locality sensitive hashing / minhash.  By minHashing all the traits of the nft as “key:value” pairs we can calculate jaccard similarity between an nft and a bid onchain.</p>
<p>In an analogy. the minhash is like a low resolution image of the nft, created by placing all the “key:value” traits on a stage and taking the snapshot.  The bidder c