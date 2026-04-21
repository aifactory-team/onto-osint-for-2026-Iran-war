# 온톨로지 확장 분석 — 2026-04-21

## 날짜
2026-04-21 (전쟁 53일차, 휴전 14일차, 레바논 휴전 5일차)

## 신규 엔티티 (ent-158 ~ ent-163)

### ent-158: Trump Ceasefire Extension Indefinite (Apr 21)
- **유형:** Event
- **근거:** 트럼프가 4/20 "highly unlikely" → 4/21 오전 CNBC "I don't want to" → 4/21 오후 4시 Truth Social에서 "until such time as their proposal is submitted"로 무기한 연장. 24시간 내 3번의 입장 변화는 이례적. 파키스탄(Munir + Sharif)의 요청을 직접 인용. 봉쇄는 유지("continue the Blockade and, in all other respects, remain ready and able").
- **기존 엔티티 연결:** ent-030(2주 휴전), ent-153(연장 거의 불가 선언), ent-029(파키스탄)
- **스키마 변경 필요:** 없음 — 기존 Event 클래스로 충분

### ent-159: Vance Trip Postponed Indefinitely (Apr 21)
- **유형:** Event
- **근거:** Axios 보도 "postponed indefinitely" — 밴스가 이슬라마바드로 출발하지 않음. 이란의 회담 보이콧이 직접 원인. 4/20에 300명 대표단 이끌고 이슬라마바드 출발 확정이었으나 하루 만에 무기한 연기.
- **기존 엔티티 연결:** ent-041(Vance), ent-119(2차 회담), ent-140(이란 거부 Apr 19)
- **스키마 변경 필요:** 없음

### ent-160: Iran Official Talk Refusal via Pakistani Intermediary (Apr 21)
- **유형:** Event
- **근거:** 파키스탄 중개인을 통해 공식 전달. "waste of time"이라 규정. 3가지 이유 제시: (1) 레바논 미포함, (2) 과도한 요구, (3) 해상 봉쇄. 갈리바프 측근: "losing side cannot dictate terms." FM: 봉쇄는 "act of war."
- **기존 엔티티 연결:** ent-140(4/19 거부), ent-095(CENTCOM 봉쇄), ent-135(IRGC-외교부 분열)
- **스키마 변경 필요:** 없음

### ent-161: Hezbollah First Rocket Fire Since Ceasefire (Apr 21)
- **유형:** Event
- **근거:** Rab al-Thalathine에 로켓 발사 + 이스라엘 방향 드론. 4/16 레바논 휴전 이후 최초의 헤즈볼라 공격 행위. 헤즈볼라 측 220+ 이스라엘 위반 주장. Legal Agenda: 4/17-19간 220회 위반, 3명 사망 7명 부상.
- **기존 엔티티 연결:** ent-047(Hezbollah), ent-109(레바논 휴전), ent-143(Yellow Line)
- **스키마 변경 필요:** 없음

### ent-162: Israel-US Joint Attack Planning (Apr 21)
- **유형:** Event
- **근거:** Kan 방송: 이스라엘 고위 안보 관계자 "jointly preparing with Washington for war's resumption." 이란 딜 회의론이 직접적 동기. 이스라엘이 미국과 공동으로 전쟁 재개를 준비한다는 최초의 명시적 보도.
- **기존 엔티티 연결:** ent-004(Israel), ent-003(US Military), ent-160(이란 회담 거부)
- **스키마 변경 필요:** 없음

### ent-163: Oil Price Movements Apr 21
- **유형:** Event
- **근거:** Brent $98.48 (+3%) / WTI $92.13 (+3%). 장 마감 후 휴전 연장 뉴스에 WTI $88.60, Brent $94.89로 하락. S&P/Nasdaq/Dow 모두 ~0.6% 하락. 4일 연속 대형 변동 지속.
- **기존 엔티티 연결:** ent-144(유가 급등 Apr 19), ent-008(호르무즈)
- **스키마 변경 필요:** 없음

## 기존 엔티티 업데이트

| 엔티티 | 변경 내용 |
|--------|----------|
| ent-001 Trump | action_apr21: 오전 CNBC "don't want to extend" → 오후 4시 Truth Social 무기한 연장; "seriously fractured" 이란 정부 언급; 봉쇄 유지 지시 |
| ent-002 Iran | action_apr21: "waste of time", 공식 거부, "act of war", IRGC "ridiculous spectacle" |
| ent-041 Vance | action_apr21: 이슬라마바드행 무기한 연기 (출발 안 함) |
| ent-047 Hezbollah | action_apr21: 4/16 휴전 이후 최초 로켓 발사, 220+ 이스라엘 위반 주장 |
| ent-008 Hormuz | status_apr21: Brent $98.48, WTI $92.13, 봉쇄 지속, 장 마감 후 하락 |
| ent-004 Israel | action_apr21: 미국과 공동 공격 계획, 이란 딜 회의론 |
| ent-029 Pakistan | action_apr21: Munir+Sharif가 트럼프에 연장 요청 → 성공, racing against time |
| ent-119 2nd Round | status_apr21: 사실상 무기한 연기 — 이란 보이콧, 밴스 미출발 |

## 이전 보고서 연관관계 분석

### 4/20 → 4/21 핵심 전환
1. **트럼프 180도 선회:** 4/20 "highly unlikely" + "lots of bombs" → 4/21 무기한 연장. 파키스탄 중재 채널이 유일한 외교 경로로 재확인. 그러나 봉쇄 유지로 압박-유화 이중 전략 지속.
2. **이란 완전 봉쇄:** 4/19 "거부" → 4/21 "waste of time" 공식화. IRGC 완전 주도권 확인. 실용파(Araghchi/Pezeshkian) 완전 소외.
3. **레바논 휴전 붕괴 시작:** 4/16 휴전 → 4/17 위반 → 4/19 Yellow Line → 4/21 헤즈볼라 최초 로켓. 5일 만에 휴전 사실상 와해 경로 진입.

### 구조적 패턴
- **이란 "seriously fractured"**: 트럼프의 이 표현이 정확하다면, 그가 무기한 연장한 이유는 이란 내부 분열이 시간이 지나면 자체적으로 타협파를 강화할 것이라는 계산.
- **봉쇄+휴전 결합**: 군사적 압박(봉쇄)은 유지하면서 정치적 여지(휴전)를 주는 전략. 이란이 "당신들이 패배한 쪽"이라고 반박하는 것과 대조.
- **이스라엘-미국 공동 전쟁 준비**: 휴전 중에도 전쟁 재개 시나리오를 준비하는 것은 협상 레버리지이자 실질적 대비. 이란 딜 무산 시 즉각 전환 가능성.

## 스키마 변경
- **새 클래스:** 없음 (0/5 한도)
- **새 관계 유형:** 없음 (0/10 한도)
- 6개 신규 엔티티 모두 기존 클래스(Event)로 분류 가능
- 30개 새 관계 + 6개 추론 모두 기존 관계 유형으로 표현 가능
