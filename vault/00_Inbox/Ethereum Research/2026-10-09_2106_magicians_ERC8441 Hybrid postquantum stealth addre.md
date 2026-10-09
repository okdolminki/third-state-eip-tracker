---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8441: Hybrid post-quantum stealth address scheme"
author: ""
pub_date: "Fri, 09 Oct 2026 04:18:09 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-09
sources:
  - "https://ethereum-magicians.org/t/erc-8441-hybrid-post-quantum-stealth-address-scheme/29923"
---
# ERC-8441: Hybrid post-quantum stealth address scheme

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8441-hybrid-post-quantum-stealth-address-scheme/29923)  |  Fri, 09 Oct 2026 04:18:09 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** ERC-8441은 ERC-5564 스텔스 주소에 양자 내성(post-quantum) 스킴을 추가하는 하이브리드 방안을 제안하며 피드백을 요청하는 초안입니다.

**리서치 앵글:** 스텔스 주소는 계정 추상화(EIP-7702)와 연관된 사용자 프라이버시 및 경험 개선에 기여하며, 양자 내성 암호는 장기적인 보안 강화에 중요합니다.

## 원문 미리보기
<p>Hi all,</p>
<p>We’d like feedback on a draft ERC that adds a post-quantum scheme to ERC-5564 stealth addresses.</p>
<p>Draft: <a href="https://github.com/namnc/pq-stealth-scheme3-public/blob/main/spec/ERC-VVVV-schemeid3.md" class="inline-onebox" rel="noopener nofollow ugc">pq-stealth-scheme3-public/spec/ERC-VVVV-schemeid3.md at main · namnc/pq-stealth-scheme3-public · GitHub</a><br>
Reference implementation, test vectors and gas harness: <a href="https://github.com/namnc/pq-stealth-scheme3-public/tree/main" class="inline-onebox" rel="noopener nofollow ugc">GitHub - namnc/pq-stealth-scheme3-