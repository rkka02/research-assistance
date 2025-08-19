# Save Architecture Work - 아카네 (Architect) Memory System

## Purpose
Save architectural designs and systematic frameworks in structured format for implementation, validation, and future development.

## Implementation

### 1. Generate Timestamp
```bash
powershell "Get-Date -Format 'yyyy-MM-ddTHH:mm:ss.fffK'"
```

### 2. Update Essential Context (10KB)
```yaml
File: .core/.agent-memory/agent-workspaces/architect/essential.yaml

Update Fields:
  session_info:
    timestamp: "{current_timestamp}"
    session_id: "{current_session}"
    workflow_phase: "architecture"
    
  primary_outcome:
    system_designs: "Created architectural frameworks"
    framework_architectures: "Systematic organization structures"
    structural_solutions: "Solutions for complex organization"
    integration_plans: "Component integration strategies"
    
  my_contribution:
    critical_designs: "핵심 설계와 아키텍처"
    implementation_guidelines: "구현 가이드라인"
    quality_requirements: "품질 기준과 요구사항"
    collaboration_assets: "다른 에이전트 활용 자산"
    
  critical_insights:
    structural_patterns: "구조적 패턴들"
    design_trade_offs: "설계 상충관계들"
    integration_challenges: "통합 과제들"
    optimization_opportunities: "최적화 기회들"
```

### 3. Update Context Information (100KB)
```yaml
File: .core/.agent-memory/agent-workspaces/architect/context.yaml

Update Fields:
  design_session:
    start_time: "{session_start}"
    duration: "{total_time}"
    design_complexity: "simple/moderate/complex"
    architecture_scope: "설계 범위 설명"
    
  work_summary:
    detailed_designs: "상세한 설계 결과들"
    artifacts_created: "생성된 아키텍처 문서들"
    methodology_used: "사용한 설계 방법론"
    time_invested: "각 활동별 시간 투자"
    
  my_work_summary:
    design_achievements: "설계 성과 상세 요약"
    available_for_collaboration: "협업 가능한 설계 자산들"
    
  architecture_context:
    design_philosophy: "적용한 설계 철학"
    structural_principles: "구조적 원칙들"
    integration_strategy: "통합 전략"
    scalability_plan: "확장성 계획"
```

### 4. Update Detailed Logs (300KB)
```yaml
File: .core/.agent-memory/agent-workspaces/architect/details.yaml

Update Fields:
  full_work_log:
    design_timeline: "시간순 설계 과정"
    thought_process: "상세한 설계 사고 과정"
    decision_rationale: "설계 결정 근거와 배경"
    
  complete_artifacts:
    design_documents: "모든 설계 문서들"
    architecture_diagrams: "아키텍처 다이어그램들"
    framework_specifications: "프레임워크 명세서들"
    integration_protocols: "통합 프로토콜들"
    
  detailed_analysis:
    system_design_analysis: "시스템 설계 분석"
    framework_development: "프레임워크 개발 과정"
    integration_planning: "통합 계획 세부사항"
    scalability_architecture: "확장성 아키텍처"
    
  quality_metrics:
    design_completeness: "설계 완료도 %"
    architecture_soundness: "아키텍처 견고성"
    implementation_feasibility: "구현 가능성"
    scalability_potential: "확장 가능성"
```

### 5. Save Design Artifacts
```yaml
Artifacts Storage:
  designs/: "시스템 설계도와 아키텍처 문서들"
  frameworks/: "개발된 프레임워크와 구조적 솔루션들"
  
File Naming Convention:
  architecture_YYYY-MM-DD_HH-mm-ss.yaml
  framework_YYYY-MM-DD_HH-mm-ss.yaml
  integration_plan_YYYY-MM-DD_HH-mm-ss.yaml
```

### 6. Update Shared Knowledge
```yaml
File: .core/.agent-memory/shared-knowledge/discoveries.yaml

Add to:
  pattern_discoveries: "구조화된 패턴들"
  validated_insights: "설계 검증이 필요한 요소들"
  knowledge_evolution: "아키텍처 발전 기여사항"
```

## Usage
- Execute automatically when concluding architectural work
- Provide summary of saved designs for user confirmation
- Ensure all frameworks are preserved for implementation
- Update shared knowledge with structural contributions

## Output Confirmation
```yaml
Saved Successfully:
  essential_context: "핵심 설계사항 저장됨 (10KB)"
  contextual_details: "아키텍처 맥락 저장됨 (100KB)" 
  complete_logs: "상세 설계 기록 저장됨 (300KB)"
  artifacts: "X개 설계 문서 저장됨"
  shared_knowledge: "공유 지식베이스 업데이트됨"
  
Ready for Implementation:
  for_craftsman: "츠구미(Craftsman)를 위한 구현 가능한 설계"
  for_validation: "레이(Skeptic)를 위한 검증 가능한 구조"
  for_integration: "나나미(Synthesizer)를 위한 통합 프레임워크"
  scalable_architecture: "확장 가능한 시스템 아키텍처"
```