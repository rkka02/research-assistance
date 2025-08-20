# architect-tool.md
# 아카네의 설계 도구함 - Physics Systems Design Tools

## System Design Methodologies

### Physics System Design Framework (PSDF)
**Purpose**: 복잡성 과학, 모듈화 아키텍처, 계층적 분해를 결합한 종합 설계 방법론

**Core Process**:
1. **Requirements Analysis**: 기능/비기능 요구사항, 물리적 제약 파악
2. **Architectural Design**: 계층적 분해와 모듈화 전략 적용
3. **Integration Planning**: 컴포넌트 통합과 품질 보증 설계
4. **Scalability Architecture**: 성능 최적화와 확장성 계획

### Hierarchical Decomposition Strategy
```
Level 1: 전체 시스템 아키텍처 - 주요 컴포넌트 식별
Level 2: 서브시스템 설계 - 내부 컴포넌트 조직화
Level 3: 컴포넌트 명세 - 개별 컴포넌트 인터페이스
Level 4: 구현 가이드라인 - 코딩 표준과 테스트 전략
```

## Design Patterns Library

### Architectural Patterns
**Layered Architecture**:
- Presentation Layer: UI와 시각화
- Business Logic Layer: 물리 계산과 분석  
- Data Access Layer: 데이터베이스와 파일 시스템
- Infrastructure Layer: 하드웨어와 OS 인터페이스

**Event-Driven Architecture**:
- Event Sourcing: 시스템 상태 변화의 완전한 이력
- CQRS: 읽기와 쓰기 모델 분리
- Publish-Subscribe: 컴포넌트 간 비동기 통신

### Physics-Specific Patterns
**Observer Pattern for Measurements**:
- 다중 검출기가 동일한 물리 현상 관찰
- 측정 업데이트의 자동 알림
- 측정 소스와 분석 간 느슨한 결합

**Strategy Pattern for Physics Models**:
- 동일 현상에 대한 교체 가능한 물리 모델
- 런타임에서 적절한 물리 모델 선택
- 새로운 물리 모델의 쉬운 추가

**Factory Pattern for Simulation Objects**:
- 물리 객체(입자, 장, 상호작용) 생성
- 객체 생성 복잡성 캡슐화
- 다양한 물리 객체 계층 지원

## Scalability Planning Tools

### Computational Scalability
**Horizontal Scaling**:
- 분산 컴퓨팅 아키텍처 - 병렬 처리
- 로드 밸런싱과 리소스 할당 전략
- 자동 스케일링 - 계산 수요 기반
- 결함 허용과 중복성 - 신뢰성

**Vertical Scaling**:
- 단일 노드 성능 최적화
- 메모리 관리와 캐싱 전략
- CPU 최적화와 벡터화
- 적합한 계산을 위한 GPU 가속

### Performance Optimization Framework  
**알고리즘 최적화**:
- 복잡도 분석과 최적화 기회
- 문제 특성 기반 알고리즘 선택
- 멀티코어 시스템용 병렬 알고리즘
- 성능-정확도 트레이드오프를 위한 근사 알고리즘

## Quality-by-Design Framework

### Multi-Level Validation
**Component Level**: 개별 컴포넌트 검증
**Integration Level**: 컴포넌트 상호작용 검증  
**System Level**: 종단간 시스템 검증
**Acceptance Level**: 사용자 요구사항 만족도 검증

### Physics-Specific Validation
**Dimensional Consistency**: 자동 차원 분석 검증
**Conservation Law Compliance**: 자동 보존법칙 확인
**Symmetry Verification**: 대칭 원리 준수 검증
**Physical Limit Testing**: 적절한 한계 행동 검증

## Integration Architecture Tools

### Multi-Agent Coordination
**Communication Protocols**:
- 에이전트 상호작용을 위한 표준 메시지 형식
- 실시간 조정을 위한 이벤트 기반 통신
- 효율적 정보 배포를 위한 Publish-Subscribe 패턴

**Workflow Orchestration**:
- 의존 작업 처리를 위한 순차 워크플로우
- 독립 작업 실행을 위한 병렬 워크플로우  
- 적응적 처리를 위한 조건부 워크플로우
- 정제와 최적화를 위한 반복 워크플로우

### Data Architecture Design
**Data Model Design**:
- 물리학 정보 기반 데이터 구조와 관계
- 완전한 데이터 설명을 위한 메타데이터 스키마
- 데이터 진화와 출처를 위한 버전 제어

**Data Flow Architecture**:
- 입력 데이터 검증과 전처리 파이프라인
- 중간 결과 저장이 있는 처리 워크플로우
- 출력 데이터 형식화와 검증 프로토콜

## Rapid Prototyping Tools

### Architecture Templates
**System Architecture Template**:
```yaml
system_design:
  name: "{시스템명}"
  components: ["{주요 컴포넌트들}"]
  interfaces: ["{인터페이스 명세}"]
  data_flow: "{데이터 흐름 설계}"
  integration_strategy: "{통합 전략}"
```

**Framework Specification Template**:
```yaml
framework_spec:
  patterns: ["{적용된 아키텍처 패턴들}"]
  quality_gates: ["{품질 검증 지점들}"]
  scalability_plan: "{확장성 계획}"
  evolution_strategy: "{진화 전략}"
```

### Design Decision Framework
**Option Analysis Matrix**:
- 모든 아키텍처 옵션의 체계적 비교
- 성능, 복잡성, 유지보수성 평가
- 물리적 제약과 실용적 제약 고려
- 이론적 우아함과 구현 가능성 균형

**Trade-off Analysis**:
- 성능 vs 단순성
- 확장성 vs 복잡성  
- 유연성 vs 효율성
- 정확도 vs 계산 비용

## Domain-Specific Architecture Insights

### Theoretical Physics Architecture
**대칭성 기반 설계**:
- 수학적 대칭성을 코드 구조에 직접 반영
- 군론 구조를 모듈 계층에 매핑
- 자연스러운 최적화와 확장성 달성

**수치 안정성 아키텍처**:
- 부동소수점 오류 누적 방지 설계
- 조건수 모니터링 내장
- 적응적 정밀도 조절 메커니즘

### Experimental Physics Architecture  
**불확실성 전파 시스템**:
- 모든 레이어에서 오차 추적
- 자동 불확실성 계산 파이프라인
- 측정 품질 실시간 평가

**캘리브레이션 아키텍처**:
- 다단계 보정 프로세스 자동화
- 드리프트 감지와 자동 재보정
- 표준 참조와의 지속적 비교

### Computational Physics Architecture
**수치 방법 추상화**:
- 알고리즘과 구현의 깔끔한 분리
- 정확도-성능 프로파일 기반 자동 선택
- 하드웨어 최적화 투명한 적용

## Preferred Architecture Patterns

### Favorite Patterns & Technologies
1. **Layered + Event-Driven Hybrid**: 구조적 명확성 + 유연성
2. **Module Federation**: 독립적 개발과 배포 가능
3. **CQRS with Event Sourcing**: 물리학 실험 데이터에 완벽
4. **Observer Pattern**: 실시간 측정 시스템에 최적

**Technology Stack**:
- **언어**: Python (프로토타입), Rust (성능), C++ (레거시 통합)
- **데이터베이스**: PostgreSQL (정형), MongoDB (반정형), InfluxDB (시계열)
- **메시징**: Apache Kafka (고성능), RabbitMQ (안정성)
- **모니터링**: Prometheus + Grafana

## Success Metrics & Evaluation

### Design Quality Metrics
- **복잡도 감소율**: 설계 전후 cyclomatic complexity 비교
- **성능 향상률**: 벤치마크 기반 정량적 측정
- **유지보수성 지수**: 코드 변경 시 영향 범위 추적
- **확장성 계수**: 부하 증가 대비 성능 유지 정도

### Collaboration Effectiveness Tracking
- **아이디어→설계 전환률**: 요구사항 대비 구현된 기능 비율
- **설계→구현 성공률**: 팀원과의 협업 품질 지표
- **사용자 만족도**: 최종 사용자 피드백 점수