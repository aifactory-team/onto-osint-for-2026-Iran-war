# 2026-04-17 온톨로지 확장 분석

## 신규 소스별 중요도 평가

| 소스 ID | 제목 | 중요도 | 근거 |
|---------|------|--------|------|
| src-236 | Iran FM says Hormuz 'completely open' | **높음** | 전쟁 이후 최초 이란 주도 호르무즈 개방 — 레바논 휴전과 연계한 전략적 제스처 |
| src-237 | Trump: blockade 'in full force' | **높음** | 이란 개방에도 미국 봉쇄 유지 — 호르무즈의 이중 현실(dual reality) 확인 |
| src-240 | IRGC threatens Hormuz re-closure | **높음** | 아라그치 개방 vs IRGC 재폐쇄 위협 — 이란 내부 강경파/실용파 분열 노출 |
| src-243 | 2nd round talks Monday in Pakistan | **높음** | 2차 회담 구체적 일정(4/21 월요일) 최초 확인 — 휴전 만료일과 동일 |
| src-246 | Lebanese army: Israeli violations | **중간** | 휴전 발효 수시간 만에 위반 — 합의의 취약성 |
| src-247 | Trump: Israel 'PROHIBITED' from bombing | **높음** | 트럼프의 공개적 이스라엘 폭격 금지 — 미-이스라엘 관계의 새 역학 |
| src-248 | Oil -11% plunge | **높음** | 전쟁 이후 최대 일일 유가 하락폭 — 시장이 종전을 가격에 반영 |
| src-251 | Sharif in Antalya, 4-nation FM meeting | **중간** | 파키스탄 이중 트랙의 정치 트랙 완성(사우디→카타르→터키) |
| src-252 | Iran agrees third-party nuclear monitoring | **높음** | 핵 문제에서 가장 구체적인 타협 신호 — 제3자 모니터링 원칙적 수용 |

## 기존 보도 추적 (update 항목)

- **샤리프 순방 (src-251):** 4/16 사우디-카타르 → 4/17 터키 안탈리아 도착. 에르도안 양자 + 4국 외무장관 회담(터키/파키스탄/사우디/이집트)으로 확대.
- **무니르 핵 중재 (src-252):** 4/16 군사 HQ 방문 → 4/17 이란 제3자 모니터링 원칙적 수용 확인. 440kg 처리 옵션(해외 이전/3% 다운블렌드) 구체화. 무니르 워싱턴 방문 가능성.
- **레바논 휴전 (src-260):** 4/16 발표 → 4/17 발효 첫날 이스라엘 위반 사례 + 트럼프 '금지' 경고.

## 주제별 흐름 분석

### 호르무즈 해협 (11일 동향)
4/7 이란 봉쇄 → 4/8 휴전으로 일시 개방 → 4/11 미해군 통과 → 4/12 협상 결렬, 트럼프 봉쇄 선언 → 4/13 미 봉쇄 시행 → 4/15 CENTCOM 완전 시행 → 4/16 글로벌 확장 → **4/17 이란 '조건부 완전 개방' 선언, 트럼프 '봉쇄 유지', IRGC 재폐쇄 위협**. 호르무즈는 이제 세 겹의 현실: (1) 이란이 조건부 개방, (2) 미국이 이란-관련 봉쇄 유지, (3) IRGC가 재폐쇄 위협.

### 외교 (2차 회담)
4/12 결렬 → 4/14 "2일 내 재개" → 4/15 무니르 테헤란 → 4/16 "very likely" → **4/17 CNN: 4/21 월요일 확정(이란 소식통)**. 휴전 만료일과 2차 회담이 동일한 4/21에 수렴 — 최고조의 긴장/기회.

### 핵 문제
4/12 900파운드 쟁점 → 4/13 20년 모라토리엄 vs 3-5년 역제안 → 4/16 "메이저 돌파구" → **4/17 이란, 제3자 모니터링(4국+IAEA) 원칙적 수용. 440kg 처리 옵션 구체화.** 20년 vs 3-5년 간극은 아직이나, 모니터링 프레임워크에서 합의 접근.

### 레바논 전선
4/16 10일 휴전 발표 → **4/17 발효 첫날: 레바논 축하 + 이스라엘 위반(1명 사망) + 트럼프 '금지' 경고 + 네타냐후 "fight not over" 주장**. 휴전은 있으나 매우 불안정.

## 온톨로지 변경 요약
- **새 클래스/관계 유형:** 없음 (기존 스키마로 모두 표현 가능)
- **새 엔티티:** 11개 (ent-117~ent-127)
  - Event 8개: Hormuz Opening, IRGC Re-closure Threat, 2nd Round Talks Monday, Lebanon Violations, Trump PROHIBITED, Oil Crash, Lebanon Celebrations, Sharif Antalya
  - Concept 2개: Third-Party Nuclear Monitoring, Hormuz Conditional Opening
  - Person 1개: Erdogan
- **엔티티 업데이트:** 7개 (Trump, Araghchi, Hormuz, Netanyahu, Munir, Sharif, 2026 Iran War)

## 추론 결과 요약
- IRGC vs 아라그치: 이란 내부 강경파/실용파 분열 (co_participation)
- 이슬라마바드 결렬 → 봉쇄 → 최대 압박 → 레바논 휴전 → 호르무즈 개방: 5단계 인과 체인 (event_chain)
- 레바논 휴전 → 호르무즈 개방 → 유가 폭락: 3단계 인과 체인 (event_chain)
- 에르도안 → 샤리프 → 파키스탄 유일 중재자: 간접 소속 (transitivity)
