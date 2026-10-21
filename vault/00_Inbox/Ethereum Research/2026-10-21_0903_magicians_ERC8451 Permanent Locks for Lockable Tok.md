---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "ERC-8451: Permanent Locks for Lockable Tokens (ERC-6982 extension)"
author: ""
pub_date: "Tue, 20 Oct 2026 20:00:59 +0000"

importance: medium
action: weekly_review
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-10-21
sources:
  - "https://ethereum-magicians.org/t/erc-8451-permanent-locks-for-lockable-tokens-erc-6982-extension/30030"
---
# ERC-8451: Permanent Locks for Lockable Tokens (ERC-6982 extension)

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/erc-8451-permanent-locks-for-lockable-tokens-erc-6982-extension/30030)  |  Tue, 20 Oct 2026 20:00:59 +0000

## AI 분석
**중요도:** medium | **액션:** weekly_review
🔔 **Pre-EIP 시그널 감지**

**요약:** ERC-6982의 확장인 ERC-8451은 토큰에 영구적인 잠금 기능을 추가하는 표준에 대한 논의입니다.

**리서치 앵글:** 토큰 잠금 기능은 LST/LRT 구조 및 RWA 토큰화 방식에 영향을 줄 수 있습니다.

## 원문 미리보기
<p>Hi all! I’m opening discussion for ERC-8451: <strong>Permanent Locks for Lockable Tokens</strong>, an extension of ERC-6982.</p>
<p><strong>PR:</strong> <a href="https://github.com/ethereum/ERCs/pull/2084" class="inline-onebox" rel="noopener nofollow ugc">Add ERC: Permanent Locks for Lockable Tokens by ryanio · Pull Request #2084 · ethereum/ERCs · GitHub</a></p>
<h2><a name="p-75483-abstract-1" class="anchor" href="https://ethereum-magicians.org#p-75483-abstract-1" aria-label="Heading link"></a>Abstract</h2>
<p>ERC-6982 lets a contract lock or unlock every token with one <code>DefaultLocked