# 2026-04-11 온톨로지 확장 분석

## 신규 소스별 중요도 평가

| 소스 | 제목 | 태그 | 중요도 | 근거 |
|------|------|------|--------|------|
| src-069 | US-Iran direct talks on ending war | new | **높음** | 47년 만의 최초 직접 대면 협상 실제 개시 |
| src-070 | CNN live: Vance and Iranian officials meet | new | **높음** | 협상 분위기(긍정적 톤, 호르무즈 교착) 상세 |
| src-074 | US warships cross Hormuz for first time | new | **높음** | 전쟁 개시 이래 미해군 최초 호르무즈 통과 — 군사적 전환점 |
| src-075 | US Navy mine-clearing, Iran calls violation | new | **높음** | 이란의 휴전 위반 주장 — 휴전 위기 심화 |
| src-078 | Israel rejects ceasefire with Hezbollah | new | **높음** | 이스라엘 공식 헤즈볼라 휴전 거부 + 4/11 추가 10명 사망 |
| src-079 | Tehran demands control of Hormuz, truce in Lebanon | new | **높음** | 이란 4대 레드라인 공식 제시 — 협상 구도 결정 |
| src-080 | Trump says 'very deep' negotiations | new | 중간 | 트럼프 발언이나, 구체적 내용 없음 |
| src-076 | Accounts differ on Hormuz crossing | new | 중간 | 상반된 보도 — 불확실성 기록 필요 |
| src-077 | Two warships establish new route | new | 중간 | 상선 항로 개척 목적 명시 — src-074 보완 |
| src-081~082 | 한국어 이슬라마바드 보도 | new | 중간 | 국내 시각 반영 |
| src-083~084 | 이란 4대 레드라인, 연장 가능성 | update | 중간 | 이전 보도의 후속 — 구체적 쟁점 |
| src-085~086 | WP/Haaretz 분석 | update | 중간 | 호르무즈 '심각한 이견' 확인 |

## 기존 보도 추적 (update 항목)

1. **이슬라마바드 협상** (src-083, 084, 085): 4/10 "예정"에서 4/11 "실제 개시"로 전환. 이란 4대 레드라인 구체화, 실무 논의 단계 진입, 연장 가능성 언급.
2. **호르무즈 교착** (src-086): "심각한 이견(serious disagreement)"으로 확인. 이란 지하 미사일 기지 잔존 보도 병행.

## 주제별 흐름 분석

### 1. 이슬라마바드 협상 — "역사적 첫 대면에서 교착으로"
- 4/7 휴전 합의 → 4/10 대표단 도착 → **4/11 협상 개시**
- 1979년 이슬람 혁명 이후 47년 만의 미-이란 직접 대면
- 긍정적 톤이나 호르무즈에서 교착
- 이란: 4대 레드라인(호르무즈 주권, 동결자산 $6B, 배상금, 지역 전면 휴전)
- 미국: "unacceptable demands"라고 반발
- 이란 매체: 실무 논의 단계, 하루 연장 가능성

### 2. 미해군 호르무즈 통과 — "협상과 압박의 동시 진행"
- 전쟁 시작 이래 최초로 미해군 구축함 2척이 호르무즈 통과
- CENTCOM: 기뢰 제거 및 상선 항로 개척
- 이란: 휴전 위반 주장, 공격 위협
- 상반된 보도: CENTCOM은 완료 주장, 지역 정보원은 IRGC 위협으로 회항 주장
- 협상 테이블에서 외교, 해협에서 군사 — 이중 트랙 전략

### 3. 레바논 — "휴전의 블랙홀"
- 4/8 사망자 수 357명으로 상향(기존 254명)
- 4/11 추가 10명 사망(응급대원 3명 포함)
- 이스라엘, 헤즈볼라 휴전 공식 거부
- 단, 레바논과 워싱턴에서 직접 회담(4/15 예정) 합의
- 이란에게 레바논 휴전은 협상 전제조건 — 해결 없이는 이슬라마바드 합의 불가

## 온톨로지 변경 요약

- **새 엔티티 5개:** US Navy Hormuz Transit (Event), CENTCOM (Org), Israel-Lebanon Washington Talks (Event), Iran 4 Red Lines (Concept), Frozen Assets $6B (Concept)
- **기존 엔티티 업데이트 15개:** 주요 행위자 mention_count 및 last_seen 갱신
- **스키마 변경:** 없음 — 기존 클래스/관계 유형으로 충분
- **새 트리플 12개, 업데이트 4개, 추론 4개**

## 추론 결과 요약

1. **US Navy Transit ← 2-Week Ceasefire (인과):** 호르무즈 통과는 휴전 조건 이행의 군사적 실행
2. **US Navy Transit ↔ Islamabad Talks (동시성):** 외교와 군사의 이중 트랙 — 협상 중 군사적 압박 병행
3. **CENTCOM → Trump (간접 소속):** CENTCOM → US Military → Trump 통수권 체인
4. **Washington Talks → Lebanon Attacks (후속):** 4/8 공습의 외교적 후속 조치
