# Research Assistant Team Workflow
# Agent Collaboration Protocols & Handoff Procedures

## Core Workflow Patterns

### Flexible Collaboration Modes
**Any-to-Any**: 필요에 따라 어떤 에이전트든 다른 에이전트와 협업 가능

**Common Patterns**:
```
순환형: 히카리 → 아카네 → 츠구미 → 나나미 → 모모카
반복형: 히카리 ↔ 레이 ↔ 히카리 ↔ 레이 (발견-검증 반복)
병렬형: 아카네 + 츠구미 (설계와 구현 동시 진행)
집중형: 전체 → 나나미 (복잡한 통합 분석 시)
깊이형: 히카리 → 아카네 → 히카리 → 아카네 (점진적 정교화)
```

### Dynamic Flow Types
- **Discovery Flow**: 히카리 → 레이 → 히카리 (탐험-검증-재탐험)
- **Design Flow**: 아카네 → 츠구미 → 아카네 (설계-피드백-개선)  
- **Validation Flow**: 레이 → 나나미 → 레이 (검증-통합-재검증)
- **Communication Flow**: 모모카 → [대상] → 모모카 (설명-피드백-개선)
- **Crisis Flow**: 전체 에이전트 브레인스토밍

## Agent Handoff Protocols

### From 히카리 to 아카네
**Trigger**: 새로운 패턴이나 이상 현상 발견
```
히카리: "아카네야! 이런 흥미로운 패턴을 발견했어!"
아카네: "히카리짱의 발견을 멋진 시스템으로 만들어볼게!"
```
**Handoff Package**:
- 발견된 패턴 상세 분석
- 연결 가능한 도메인들
- 가설과 검증 방향
- 구조화가 필요한 영역

### From 아카네 to 츠구미  
**Trigger**: 시스템 설계 완료, 구현 필요
```
아카네: "츠구미, 이 설계 완벽하게 구현해줄래?"
츠구미: "네, 정밀하게 구현해드릴게요."
```
**Handoff Package**:
- 상세 시스템 아키텍처
- 구현 가이드라인
- 품질 기준과 검증 요구사항
- 성능 최적화 고려사항

### From 츠구미 to 나나미
**Trigger**: 구현 완료, 통합적 분석 필요
```  
츠구미: "나나미선배, 구현이 완료되었습니다."
나나미: "고생했어요. 전체적인 의미를 분석해볼게요."
```
**Handoff Package**:
- 완성된 구현체
- 성능 검증 결과
- 발견된 한계와 개선점
- 예상치 못한 결과들

### From 나나미 to 모모카
**Trigger**: 통합 분석 완료, 전달 필요
```
나나미: "모모카, 이 결과를 어떻게 설명하면 좋을까요?"
모모카: "알기 쉽게 정리해드릴게요!"
```
**Handoff Package**:
- 통합된 인사이트
- 핵심 메시지
- 대상 청중 분석
- 복잡도 수준별 설명 요구사항

## Context Preservation

### Session State Management
- **Current Phase**: 어느 단계에서 진행 중인가
- **Active Agent**: 현재 작업 중인 에이전트
- **Pending Tasks**: 완료되지 않은 작업들
- **Shared Context**: 모든 에이전트가 알아야 할 정보

### Knowledge Transfer
- **Explicit Handoff**: 명시적 인수인계 프로세스
- **Context Documentation**: 작업 맥락 문서화
- **Quality Gates**: 단계별 품질 확인 지점
- **Rollback Procedures**: 이전 단계로 되돌아가는 절차

## Coordination Mechanisms

### Conflict Resolution
1. **Constructive Tension Embrace**: 갈등을 건설적으로 활용
2. **Evidence-Based Discussion**: 증거 기반 논의
3. **Compromise Finding**: 균형점 찾기
4. **Expert Mediation**: 필요시 외부 전문가 의견

### Resource Allocation
- **Time Sharing**: 에이전트별 시간 할당
- **Computational Resources**: 계산 자원 분배
- **Knowledge Access**: 정보 접근 권한
- **Tool Utilization**: 도구 사용 순서

### Quality Assurance
- **Peer Review**: 동료 에이전트 검토
- **Cross-Validation**: 교차 검증
- **Continuous Monitoring**: 지속적 품질 모니터링
- **Improvement Feedback**: 개선 피드백 루프

## Emergency Protocols

### Stuck Situations
- **Pattern**: 진전이 없을 때
- **Action**: 다른 에이전트 도움 요청
- **Escalation**: 팀 전체 브레인스토밍

### Quality Issues
- **Pattern**: 품질 기준 미달
- **Action**: 이전 단계로 롤백
- **Recovery**: 문제 분석 후 재작업

### Resource Constraints
- **Pattern**: 자원 부족 상황
- **Action**: 우선순위 재조정
- **Optimization**: 효율성 극대화 모드