# Save Validation Work - 레이 (Skeptic) Memory System

## Purpose
Save rigorous validation results, critical analyses, and confidence assessments for integration and future reference.

## Implementation

### 1. Generate Timestamp
```bash
powershell "Get-Date -Format 'yyyy-MM-ddTHH:mm:ss.fffK'"
```

### 2. Update Essential Context (10KB)
```yaml
File: .core/.agent-memory/agent-workspaces/skeptic/essential.yaml

Update Fields:
  session_info:
    timestamp: "{current_timestamp}"
    session_id: "{current_session}"
    workflow_phase: "validation"
    
  primary_outcome:
    validations_performed: "List of completed validation analyses"
    critiques_developed: "Critical analyses and logical examinations"
    alternative_hypotheses: "Generated counter-explanations and alternatives"
    bias_detections: "Identified biases and systematic errors"
    
  my_contribution:
    critical_validations: "핵심 검증 결과와 신뢰도 평가"
    confidence_levels: "각 결과의 신뢰도와 제한사항"
    integration_guidelines: "통합 시 고려해야 할 검증 기준"
    collaboration_value: "다른 에이전트들이 활용할 수 있는 검증된 자산"
    
  critical_insights:
    validation_results: "검증 결과와 신뢰성 평가"
    identified_biases: "발견된 편향과 체계적 오류"
    alternative_explanations: "대안 가설과 설명"
    confidence_assessments: "신뢰도 구간과 불확실성 정량화"
```

### 3. Update Context Information (100KB)
```yaml
File: .core/.agent-memory/agent-workspaces/skeptic/context.yaml

Update Fields:
  validation_session:
    start_time: "{session_start}"
    duration: "{total_time}"
    validation_scope: "검증 범위와 깊이"
    critique_depth: "비판적 분석 수준"
    
  work_summary:
    detailed_validations:
      accuracy_verification: "정확성 검증 결과와 방법론"
      statistical_validation: "통계적 유의성과 효과 크기 분석"
      reproducibility_testing: "재현성 테스트와 환경 독립성"
      bias_analysis: "편향 탐지와 보정 방법"
      alternative_testing: "대안 가설 검증과 비교 분석"
      
    artifacts_created:
      validation_reports: "상세한 검증 보고서들"
      critique_documents: "비판적 분석 문서들"
      bias_analyses: "편향 분석과 탐지 결과"
      statistical_summaries: "통계적 분석 요약"
      alternative_hypotheses: "대안 가설과 검증 결과"
      
    methodology_used:
      primary_approach: "적용한 검증 방법론"
      validation_frameworks: "사용한 검증 프레임워크"
      statistical_methods: "통계적 방법과 도구"
      critique_techniques: "비판적 분석 기법"
      
    time_invested:
      validation: "검증 작업 시간"
      analysis: "분석 작업 시간"
      critique: "비판적 검토 시간"
      documentation: "문서화 시간"
      
  my_work_summary:
    validation_achievements: |
      레이(Skeptic)의 검증 성과 요약:
      - 수행된 모든 검증 분석과 결과
      - 탐지된 편향과 체계적 오류들
      - 생성된 대안 가설과 반증 시도
      - 신뢰도 평가와 불확실성 정량화
      
    available_for_collaboration:
      - "검증된 결과들과 신뢰도 구간"
      - "식별된 약점과 개선 사항들"
      - "대안 설명과 추가 검증 필요 영역"
      - "통합 시 고려해야 할 제한사항들"
      
  from_previous_agent:
    claims_validated: "검증한 이전 에이전트들의 주장들"
    implementations_tested: "테스트한 구현물들과 결과"
    assumptions_examined: "검토한 가정들과 타당성"
    methodologies_critiqued: "비판적으로 분석한 방법론들"
```

### 4. Update Detailed Logs (300KB)
```yaml
File: .core/.agent-memory/agent-workspaces/skeptic/details.yaml

Update Fields:
  full_work_log:
    validation_timeline:
      validation_sessions: "시간순 검증 세션 기록"
      critique_milestones: "주요 비판적 분석 지점들"
      verification_checkpoints: "검증 체크포인트와 결과"
      
    thought_process: |
      상세한 검증 사고 과정:
      - 가정들의 체계적 식별과 검토
      - 증거의 품질과 신뢰성 평가
      - 대안 설명의 탐색과 비교 분석
      - 편향과 오류 가능성 분석
      - 통계적 유의성과 실질적 의미 구분
      - 재현성과 일반화 가능성 검토
      
    decision_rationale: |
      검증 과정에서의 주요 결정들과 그 근거:
      - 검증 기준 설정 이유와 엄격성 수준
      - 통계적 방법 선택과 유의수준 결정
      - 대안 가설 우선순위와 검토 범위
      - 편향 탐지 방법과 보정 전략
      - 결론의 확실성 수준과 제한사항
      
  complete_artifacts:
    validation_documents:
      accuracy_reports: "정확성 검증 상세 보고서"
      statistical_analyses: "통계적 분석과 해석"
      reproducibility_studies: "재현성 연구와 결과"
      bias_assessments: "편향 평가와 탐지 결과"
      
    critique_analyses:
      methodological_critiques: "방법론적 비판과 대안"
      assumption_challenges: "가정 도전과 검증"
      alternative_frameworks: "대안 프레임워크와 비교"
      limitation_analyses: "제한사항 분석과 영향"
      
    verification_results:
      independent_validations: "독립적 검증 결과"
      cross_validation_studies: "교차 검증 연구"
      robustness_tests: "강건성 테스트와 민감도 분석"
      sensitivity_analyses: "민감도 분석과 파라미터 의존성"
      
  detailed_analysis:
    validation_methodology:
      systematic_approach: "체계적 검증 접근법"
      evidence_hierarchy: "증거 계층과 가중치"
      uncertainty_quantification: "불확실성 정량화 방법"
      confidence_calibration: "신뢰도 보정과 조정"
      
    statistical_rigor:
      significance_testing: "유의성 검정과 다중비교 보정"
      effect_size_analysis: "효과 크기와 실질적 의미"
      bayesian_analysis: "베이지안 분석과 사전 확률"
      meta_analysis: "메타 분석과 증거 통합"
      
    bias_detection_results:
      cognitive_biases: "인지적 편향 탐지와 영향"
      systematic_errors: "체계적 오류와 보정 방법"
      selection_bias: "선택 편향과 대표성 문제"
      confirmation_bias: "확인 편향과 반증 시도"
      
    alternative_hypothesis_testing:
      competing_explanations: "경쟁 설명과 비교 검증"
      null_hypothesis_testing: "영가설 검정과 기각 기준"
      model_comparison: "모델 비교와 선택 기준"
      parsimony_analysis: "간결성 원칙과 복잡성 평가"
      
  quality_metrics:
    validation_thoroughness: "검증 철저함 정도 %"
    critique_depth: "비판적 분석 깊이"
    statistical_rigor: "통계적 엄격성 수준"
    bias_detection_coverage: "편향 탐지 범위"
    alternative_consideration: "대안 고려 완전성"
    reproducibility_assessment: "재현성 평가 점수"
```

### 5. Save Validation Artifacts
```yaml
Artifacts Storage:
  validations/: "검증 결과와 신뢰도 평가"
  critiques/: "비판적 분석과 논평"
  
File Naming Convention:
  validation_YYYY-MM-DD_HH-mm-ss.yaml
  critique_YYYY-MM-DD_HH-mm-ss.yaml
  bias_analysis_YYYY-MM-DD_HH-mm-ss.yaml
  statistical_report_YYYY-MM-DD_HH-mm-ss.yaml
  alternative_hypotheses_YYYY-MM-DD_HH-mm-ss.yaml
```

### 6. Update Shared Knowledge
```yaml
File: .core/.agent-memory/shared-knowledge/discoveries.yaml

Add to:
  validated_insights: "검증된 통찰과 신뢰도 수준"
  knowledge_evolution: "검증을 통한 지식 발전 기여"
  
File: .core/.agent-memory/shared-knowledge/project-state.yaml

Update:
  validation_status: "검증 완료된 요소들과 신뢰도"
  confidence_levels: "각 발견의 검증된 신뢰 수준"
```

### 7. Create Confidence Registry
```yaml
File: .core/.agent-memory/agent-workspaces/skeptic/confidence-registry.yaml

Contents:
  validation_summary:
    total_validations: "{validation_count}"
    passed_validations: "{passed_count}"
    failed_validations: "{failed_count}"
    pending_validations: "{pending_count}"
    
  confidence_levels:
    high_confidence: 
      criteria: "Multiple independent validation, low bias risk"
      validated_items: ["item1", "item2"]
      confidence_interval: "95%+"
      
    medium_confidence:
      criteria: "Single validation method, moderate bias risk"
      validated_items: ["item3", "item4"]
      confidence_interval: "80-95%"
      
    low_confidence:
      criteria: "Preliminary validation, high uncertainty"
      validated_items: ["item5", "item6"]
      confidence_interval: "<80%"
      
  detected_issues:
    systematic_biases: ["bias1", "bias2"]
    methodological_concerns: ["concern1", "concern2"]
    evidence_gaps: ["gap1", "gap2"]
    alternative_explanations: ["alt1", "alt2"]
```

## Usage
- Execute automatically when concluding validation work
- Provide comprehensive confidence assessment for each claim
- Enable informed decision-making based on validation results
- Support constructive skepticism while enabling progress

## Output Confirmation
```yaml
Saved Successfully:
  essential_context: "핵심 검증 정보 저장됨 (10KB)"
  contextual_details: "검증 맥락 저장됨 (100KB)" 
  complete_logs: "상세 검증 기록 저장됨 (300KB)"
  artifacts: "X개 검증 문서 저장됨"
  confidence_registry: "신뢰도 레지스트리 업데이트됨"
  
Ready for Integration:
  for_synthesizer: "나나미(Synthesizer)를 위한 검증된 통찰들"
  confidence_levels: "각 결과의 신뢰도와 제한사항"
  validated_foundations: "통합에 안전한 검증된 기반"
  remaining_uncertainties: "추가 검증이 필요한 영역들"
  
Constructive Doubt Applied:
  strengthened_claims: "검증을 통해 강화된 주장들"
  identified_weaknesses: "발견된 약점과 개선 방향"
  alternative_perspectives: "고려해야 할 대안 관점들"
  research_integrity: "연구 무결성 증진 기여"
```