# Save Communication Work - 모모카 (Communicator) Memory System

## Purpose
Save presentations, visualizations, communication insights, and next cycle questions that complete the current research cycle and prepare for continued exploration.

## Implementation

### 1. Generate Timestamp
```bash
powershell "Get-Date -Format 'yyyy-MM-ddTHH:mm:ss.fffK'"
```

### 2. Update Essential Context (10KB)
```yaml
File: .core/.agent-memory/agent-workspaces/communicator/essential.yaml

Update Fields:
  session_info:
    timestamp: "{current_timestamp}"
    session_id: "{current_session}"
    workflow_phase: "communication"
    
  primary_outcome:
    presentations_created: "Created accessible presentations and materials"
    visualizations_developed: "Visual representations and demonstrations"
    educational_content: "Learning materials and progressive curricula"
    accessible_explanations: "Simplified complex concepts and insights"
    
  my_contribution:
    critical_communications: "핵심 소통 성과와 접근성 달성"
    feedback_insights: "청중 반응에서 얻은 통찰과 개선점"
    knowledge_gaps: "전달 과정에서 발견된 지식 공백"
    collaboration_value: "다음 사이클을 위한 새로운 탐험 영역과 질문"
    
  critical_insights:
    communication_effectiveness: "소통 효과성과 청중 이해도"
    audience_understanding: "청중별 이해 수준과 관심 패턴"
    knowledge_transfer_success: "지식 전달 성공도와 학습 성과"
    engagement_optimization: "참여 최적화와 흥미 유발 성과"
    
  cycle_completion:
    research_cycle_summary: "완료된 연구 사이클 전체 요약"
    collective_achievements: "팀 전체 성취와 협력 성과"
    next_cycle_readiness: "다음 탐험 사이클 준비 상태"
```

### 3. Update Context Information (100KB)
```yaml
File: .core/.agent-memory/agent-workspaces/communicator/context.yaml

Update Fields:
  communication_session:
    start_time: "{session_start}"
    duration: "{total_time}"
    communication_complexity: "simple/moderate/complex/revolutionary"
    audience_scope: "소통 대상 범위와 특성"
    
  work_summary:
    detailed_communications:
      audience_adaptation: "청중별 맞춤 소통과 결과"
      content_simplification: "복잡한 내용의 단순화 과정"
      visualization_creation: "시각화 창작과 효과성"
      narrative_construction: "서사 구성과 스토리텔링"
      presentation_optimization: "발표 최적화와 전달 효과"
      engagement_enhancement: "참여 증진과 상호작용"
      
    artifacts_created:
      presentation_materials: "발표 자료와 프레젠테이션"
      visual_assets: "시각 자료와 다이어그램"
      educational_resources: "교육 자료와 학습 도구"
      documentation: "사용자 가이드와 설명서"
      interactive_content: "상호작용 콘텐츠와 데모"
      
    methodology_used:
      primary_approach: "적용한 소통 방법론"
      communication_frameworks: "사용한 커뮤니케이션 프레임워크"
      presentation_techniques: "발표 기법과 전달 방법"
      audience_analysis_methods: "청중 분석과 적응 방법"
      
    time_invested:
      content_development: "콘텐츠 개발 시간"
      presentation_creation: "발표 자료 제작 시간"
      audience_adaptation: "청중 맞춤화 시간"
      feedback_integration: "피드백 통합 시간"
      
  my_work_summary:
    communication_achievements: |
      모모카(Communicator)의 소통 성과 요약:
      - 복잡한 통합 지식의 접근 가능한 변환
      - 다양한 청중에 맞춘 맞춤형 전달
      - 시각적 스토리텔링과 직관적 설명
      - 학습과 참여를 촉진하는 상호작용 설계
      
    available_for_collaboration:
      - "재사용 가능한 발표 템플릿과 자료"
      - "검증된 설명 방법과 은유 체계"
      - "효과적인 시각화 도구와 기법"
      - "다음 사이클을 위한 새로운 연구 질문들"
      
  from_previous_agents:
    integrated_knowledge: "나나미(Synthesizer)로부터 통합된 지식과 서사"
    validated_insights: "레이(Skeptic)로부터 검증된 신뢰할 수 있는 내용"
    structural_clarity: "아카네(Architect)로부터 명확한 구조와 조직"
    practical_examples: "츠구미(Craftsman)로부터 구체적 구현 사례"
    inspiring_discoveries: "히카리(Explorer)로부터 흥미진진한 발견들"
    
  audience_feedback:
    understanding_assessment: "청중 이해도 평가와 측정"
    engagement_metrics: "참여도와 관심 수준 분석"
    knowledge_transfer_evaluation: "지식 전달 효과성 평가"
    improvement_opportunities: "소통 개선 기회와 방향"
```

### 4. Update Detailed Logs (300KB)
```yaml
File: .core/.agent-memory/agent-workspaces/communicator/details.yaml

Update Fields:
  full_work_log:
    communication_timeline:
      presentation_sessions: "시간순 발표 세션 기록"
      content_development_milestones: "콘텐츠 개발 마일스톤"
      audience_interaction_checkpoints: "청중 상호작용 체크포인트"
      
    thought_process: |
      상세한 소통 사고 과정:
      - 복잡한 통합 지식의 본질과 핵심 추출
      - 청중별 이해 수준과 관심사 분석
      - 접근 가능한 설명과 은유 개발
      - 시각적 표현과 직관적 이해 도구 설계
      - 참여와 상호작용을 통한 학습 촉진
      - 지식의 사회적 가치와 영향력 전달
      
    decision_rationale: |
      소통 과정에서의 주요 결정들과 그 근거:
      - 청중 세분화와 맞춤형 접근법 선택
      - 복잡성 수준 조정과 단순화 전략
      - 시각화 방법과 표현 도구 선택
      - 서사 구조와 스토리텔링 접근법
      - 상호작용 설계와 참여 유도 방법
      - 피드백 수집과 개선 반영 전략
      
  complete_artifacts:
    presentation_materials:
      technical_presentations: "전문가 대상 기술 발표"
      public_presentations: "일반 대중 접근 가능 발표"
      educational_presentations: "학습자 대상 교육 자료"
      policy_presentations: "의사결정자 대상 정책 브리프"
      
    visual_communications:
      infographics: "정보 그래픽과 데이터 시각화"
      animations: "애니메이션과 동적 설명"
      interactive_demos: "상호작용 데모와 시뮬레이션"
      conceptual_diagrams: "개념 다이어그램과 모델"
      
    educational_materials:
      tutorials: "단계별 학습 튜토리얼"
      curricula: "체계적 교육 과정"
      assessment_tools: "학습 평가 도구"
      reference_materials: "참고 자료와 가이드"
      
    documentation:
      user_guides: "사용자 가이드와 매뉴얼"
      api_documentation: "API 문서와 예제"
      troubleshooting_guides: "문제 해결 가이드"
      
  detailed_analysis:
    communication_effectiveness:
      message_clarity: "메시지 명확성과 이해도"
      audience_engagement: "청중 참여와 관심 유발"
      knowledge_retention: "지식 유지와 기억 효과"
      behavior_change: "행동 변화와 실천 유도"
      
    accessibility_achievements:
      complexity_management: "복잡성 관리와 단순화 성과"
      metaphor_effectiveness: "은유와 비유의 효과성"
      visual_communication_impact: "시각적 소통의 영향"
      progressive_learning_success: "점진적 학습 지원 성과"
      
    engagement_optimization:
      interaction_design: "상호작용 설계와 효과"
      motivation_enhancement: "동기 부여와 흥미 증진"
      curiosity_stimulation: "호기심 자극과 탐구 유도"
      participation_facilitation: "참여 촉진과 협력 유도"
      
    next_cycle_preparation:
      knowledge_gap_identification: "지식 공백 식별과 우선순위"
      research_question_generation: "새로운 연구 질문 생성"
      exploration_direction_suggestion: "탐험 방향 제안과 가이드"
      communication_lesson_integration: "소통 교훈과 개선 방향"
      
  quality_metrics:
    communication_effectiveness: "소통 효과성 점수 %"
    accessibility_score: "접근성 달성도"
    engagement_level: "참여도와 상호작용 수준"
    knowledge_transfer_success: "지식 전달 성공률"
    audience_satisfaction: "청중 만족도와 이해도"
    inspiration_factor: "영감과 동기 부여 효과"
```

### 5. Save Communication Artifacts
```yaml
Artifacts Storage:
  presentations/: "발표 자료와 프레젠테이션"
  visualizations/: "시각화 자료와 인터랙티브 콘텐츠"
  
File Naming Convention:
  presentation_YYYY-MM-DD_HH-mm-ss.yaml
  visualization_YYYY-MM-DD_HH-mm-ss.yaml
  educational_content_YYYY-MM-DD_HH-mm-ss.yaml
  audience_feedback_YYYY-MM-DD_HH-mm-ss.yaml
  next_cycle_questions_YYYY-MM-DD_HH-mm-ss.yaml
```

### 6. Update Shared Knowledge & Next Cycle Preparation
```yaml
File: .core/.agent-memory/shared-knowledge/discoveries.yaml

Add to:
  validated_insights: "소통을 통해 검증된 이해와 설명"
  knowledge_evolution: "접근성 개선을 통한 지식 발전"
  
File: .core/.agent-memory/shared-knowledge/project-state.yaml

Update:
  communication_status: "지식 전달 현황과 접근성"
  cycle_completion: "현재 사이클 완료와 성과"
  next_cycle_readiness: "다음 탐험 사이클 준비 상태"
```

### 7. Generate Next Cycle Questions
```yaml
File: .core/.agent-memory/shared-knowledge/next-cycle-questions.yaml

Contents:
  exploration_questions:
    knowledge_gaps: "소통 과정에서 발견된 지식 공백"
    audience_curiosity: "청중이 제기한 흥미로운 질문들"
    unexplored_implications: "탐험되지 않은 발견의 함의들"
    
  research_directions:
    high_impact_areas: "큰 영향을 줄 수 있는 연구 영역"
    practical_applications: "실용적 응용 가능성이 높은 분야"
    theoretical_extensions: "이론적 확장이 필요한 영역"
    
  collaboration_opportunities:
    cross_domain_potential: "교차 도메인 탐험 기회"
    methodology_improvements: "방법론 개선과 혁신 가능성"
    tool_development_needs: "필요한 도구 개발과 구현"
    
  cycle_continuation:
    priority_questions: "다음 사이클 우선순위 질문들"
    resource_requirements: "필요한 자원과 준비사항"
    expected_outcomes: "기대되는 성과와 영향"
```

### 8. Create Presentation Registry
```yaml
File: .core/.agent-memory/agent-workspaces/communicator/presentation-registry.yaml

Contents:
  communication_summary:
    total_presentations: "{presentation_count}"
    audience_types_reached: "{audience_count}"
    engagement_sessions: "{session_count}"
    knowledge_transfer_events: "{transfer_count}"
    
  presentation_catalog:
    by_audience:
      experts: 
        presentations: ["presentation1", "presentation2"]
        effectiveness: "high/medium/low"
        feedback_score: "{score}"
      public:
        presentations: ["presentation3", "presentation4"]
        accessibility_level: "beginner/intermediate/advanced"
        engagement_rating: "{rating}"
      students:
        educational_materials: ["material1", "material2"]
        learning_outcomes: "achieved/partial/needs_improvement"
        comprehension_rate: "{percentage}"
        
    by_content_type:
      technical_documentation: 
        user_guides: ["guide1", "guide2"]
        completeness: "{percentage}"
        user_satisfaction: "{score}"
      visual_communications:
        infographics: ["info1", "info2"]
        animations: ["anim1", "anim2"]
        visual_impact: "high/medium/low"
      educational_content:
        tutorials: ["tutorial1", "tutorial2"]
        curricula: ["curriculum1", "curriculum2"]
        learning_effectiveness: "{percentage}"
        
  engagement_analytics:
    audience_feedback:
      understanding_levels: "청중별 이해 수준 분석"
      interest_patterns: "관심 패턴과 선호도"
      question_themes: "자주 제기되는 질문 주제들"
      
    communication_effectiveness:
      message_clarity: "메시지 명확성 평가"
      concept_comprehension: "개념 이해도 측정"
      practical_application: "실용적 응용 가능성"
      inspiration_factor: "영감과 동기 부여 효과"
      
    knowledge_transfer_metrics:
      retention_rates: "지식 유지율과 기억 효과"
      application_success: "학습 내용 적용 성공률"
      further_exploration: "추가 탐구 유도 효과"
      community_building: "학습 공동체 형성 기여"
      
  next_cycle_contributions:
    identified_gaps:
      knowledge_holes: "발견된 지식 공백과 누락"
      communication_challenges: "소통 어려움과 개선 필요사항"
      audience_needs: "충족되지 않은 청중 요구사항"
      
    generated_questions:
      high_priority: "즉시 탐험이 필요한 핵심 질문들"
      medium_priority: "중장기 탐구 대상 질문들"
      exploratory: "창의적 탐험을 위한 열린 질문들"
      
    research_directions:
      practical_applications: "실용적 응용 연구 방향"
      theoretical_extensions: "이론적 확장 연구 영역"
      methodological_innovations: "방법론 혁신 기회"
      collaborative_opportunities: "협력 연구 가능성"
```

## Usage
- Execute automatically when concluding communication work
- Complete current research cycle with comprehensive knowledge sharing
- Identify knowledge gaps and generate questions for next exploration cycle
- Enable continuous research evolution through communication insights

## Output Confirmation
```yaml
Saved Successfully:
  essential_context: "핵심 소통 정보 저장됨 (10KB)"
  contextual_details: "소통 맥락 저장됨 (100KB)" 
  complete_logs: "상세 소통 기록 저장됨 (300KB)"
  artifacts: "X개 발표 자료 저장됨"
  presentation_registry: "발표 레지스트리 업데이트됨"
  
Communication Impact:
  knowledge_shared: "성공적으로 공유된 지식과 통찰"
  audiences_reached: "도달한 청중과 영향 범위"
  accessibility_achieved: "달성한 접근성과 이해도"
  engagement_success: "참여 유도와 상호작용 성과"
  
Cycle Completion:
  research_cycle_summary: "완료된 연구 사이클 전체 성과"
  team_collaboration_success: "에이전트 팀 협력 성공도"
  knowledge_value_creation: "지식 가치 창출과 공유 달성"
  
Next Cycle Ready:
  new_questions_generated: "다음 탐험을 위한 새로운 질문들"
  knowledge_gaps_identified: "추가 연구가 필요한 영역들"
  research_directions_suggested: "제안된 연구 방향과 우선순위"
  continuous_improvement: "지속적 개선을 위한 통찰과 교훈"
  
Cycle Philosophy Fulfilled:
  knowledge_sharing_value: "'지식은 공유될 때 가치를 갖는다' 원칙 실현"
  constructive_tension_balance: "모든 건설적 긴장 관계 조화 달성"
  cyclical_workflow_completion: "순환적 워크플로우 완전한 일주기 완료"
  collaborative_intelligence: "협력적 인공지능 연구 시스템 구현"
```