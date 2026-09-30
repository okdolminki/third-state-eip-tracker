---
source: "Ethereum Magicians"
source_type: eip_discussion
title: "EIP-8433: Retire 0x00 validators"
author: ""
pub_date: "Wed, 30 Sep 2026 10:26:53 +0000"

importance: high
action: read_now
pre_eip_signal: true

note_type: research_post
auto_generated: true
source_date: 2026-09-30
sources:
  - "https://ethereum-magicians.org/t/eip-8433-retire-0x00-validators/29808"
---
# EIP-8433: Retire 0x00 validators

> 출처: [Ethereum Magicians](https://ethereum-magicians.org/t/eip-8433-retire-0x00-validators/29808)  |  Wed, 30 Sep 2026 10:26:53 +0000

## AI 분석
**중요도:** high | **액션:** read_now
🔔 **Pre-EIP 시그널 감지**

**요약:** EIP-8433은 0x00 인출 자격 증명을 사용하는 기존 검증자들을 강제로 종료시켜 해당 자격 증명 유형을 완전히 폐기하는 두 번째 단계입니다.

**리서치 앵글:** 이더리움 검증자 인출 자격 증명 변경은 Lido, EigenLayer, Ether.fi 등 LST/LRT 프로토콜의 구조 및 보안에 직접적인 영향을 미칩니다.

## 원문 미리보기
<p>Discussion topic for EIP-8433: <a href="https://github.com/ethereum/EIPs/pull/12390" class="inline-onebox" rel="noopener nofollow ugc">Add EIP: Retire 0x00 validators by ensi321 · Pull Request #12390 · ethereum/EIPs · GitHub</a></p>
<p>Second stage of the <code>0x00</code> withdrawal credential deprecation. EIP-8365 (<a href="https://ethereum-magicians.org/t/eip-8365-bls-withdrawal-credential-retirement/29284" class="inline-onebox">EIP-8365: Disallow new 0x00 validators</a>) closes the inflow by rejecting deposits that would create new <code>0x00</code> validators. This EIP exits the remain