---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-XXXX: Protected Accounts for Fungible Tokens--*"
author: ""
pub_date: "Sat, 07 Nov 2026 07:28:16 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-11-07
sources:
  - "https://ethereum-magicians.org/t/erc-xxxx-protected-accounts-for-fungible-tokens/30297"
---
# ERC-XXXX: Protected Accounts for Fungible Tokens--*

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-xxxx-protected-accounts-for-fungible-tokens/30297)  |  Sat, 07 Nov 2026 07:28:16 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** ERC-20 토큰을 위한 선택적 '보호 계정' 기능을 제안하며, 소액 거래는 즉시 처리하고 고액 거래는 백업 지갑으로 취소 가능한 지연 기능을 도입하여 자산 탈취 및 강압 공격에 대응합니다.

**리서치 앵글:** 계정 추상화(EIP-7702) 테마와 연관되어 기관 DeFi 도입을 위한 ERC-20 자산 보안 강화 방안을 제시합니다.

## 원문 미리보기
<p><strong>TL;DR:</strong> An opt-in, public, per-account “protected” flag for ERC-20s. Small sends stay instant; anything bigger is scheduled and can be cancelled by a pre-registered backup wallet; a “stress” action sweeps everything to the backup and locks it, which also helps against wrench attacks. Turning protection on is instant; weakening it (off, higher limit, shorter waits, new backup) takes a delay the holder picks.</p>
<p><strong>Why:</strong> Today a stolen key or a coerced holder means an instant, final drain. Existing approaches are per-transfer (SLOW), need recipient cooperation