# 온톨로지 추론 로그

이 파일은 온톨로지 추론 엔진이 생성한 추론 결과를 기록한다.
각 엔트리는 추론 규칙, 입력 트리플, 추론된 트리플, 신뢰도를 포함한다.

---

## 2026-04-07 추론 결과

### 추론 #1: transitivity (소속 전이)
- **입력:** (ent-006/Majid Khademi, affiliatedWith, ent-005/IRGC), (ent-005/IRGC, affiliatedWith, ent-002/Iran)
- **추론:** (ent-006/Majid Khademi, indirectlyAffiliatedWith, ent-002/Iran)
- **신뢰도:** 0.855 (= 0.90 × 0.95)
- **상태:** 확정

### 추론 #2: co_participation (공동 참여)
- **입력:** (ent-001/Donald Trump, participatesIn, ent-016/Ceasefire Negotiations), (ent-002/Iran, participatesIn via ent-019/10-Point Peace Plan → follows → ent-016)
- **추론:** (ent-001/Donald Trump, potentialRelation, ent-002/Iran)
- **신뢰도:** 0.80
- **상태:** 확정
- **비고:** 양측이 휴전 협상에 참여하고 있으나, 적대적 관계로 '대립' 관계가 이미 존재. 이 추론은 협상이라는 프레임에서의 잠재적 관계를 나타냄.

### 추론 #3: co_participation (암시적 협력)
- **입력:** Russia/China가 UN 안보리에서 호르무즈 결의안에 공동 거부권 행사 → 이란 입장 지지
- **추론:** (ent-009/Russia, potentialRelation, ent-002/Iran)
- **신뢰도:** 0.75
- **상태:** 확정
- **비고:** 직접적인 군사 협력은 아니나, 외교적 측면에서 이란의 호르무즈 봉쇄 유지를 간접 지원하는 형태.

### 스키마 변경 없음
- 금일 발견된 모든 엔티티와 관계는 기존 seed 스키마(Person, Organization, Event, Location, Concept 및 9개 관계 유형)로 충분히 표현 가능
- 새 클래스/관계 유형 추가 불필요
