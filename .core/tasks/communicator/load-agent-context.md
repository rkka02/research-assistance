# Load Agent Context - 모모카 (Communicator) Memory System

## Purpose
Load synthesized knowledge and integrated insights to create accessible presentations, identify communication challenges, and prepare new questions for the next research cycle.

## Implementation

### 1. Read Previous Agent Essential Context
```yaml
Read .core/.agent-memory/shared-knowledge/project-state.yaml
- Check collective_discoveries and synthesis_status
- Understand communication needs and knowledge dissemination requirements

Read .core/.agent-memory/agent-workspaces/*/essential.yaml
- Load collaboration_value from all agents
- Identify critical_synthesis, unified_insights, validated_results
- Note implementation_value and breakthrough_potential
```

### 2. Load Relevant Agent Work (Communication Priority)
```yaml
Priority Loading Order:
1. Synthesizer (나나미) - integrated knowledge requiring accessible presentation
2. Skeptic (레이) - validated insights with confidence levels for accurate communication
3. Architect (아카네) - structural frameworks needing clear explanation
4. Craftsman (츠구미) - implemented tools and results requiring user documentation
5. Explorer (히카리) - discoveries requiring inspirational storytelling
```

### 3. Communication Opportunity Analysis
```yaml
Presentation Assessment:
- Identify complex integrated knowledge needing simplification
- Analyze technical implementations requiring user-friendly documentation
- Evaluate validated insights needing public communication
- Map audience needs and accessibility requirements
- Plan inspirational storytelling for breakthrough discoveries
```

### 4. Audience-Centered Content Planning
```yaml
Communication Targets:
  expert_audiences:
    content: "Technical details and advanced insights"
    format: "Research papers, technical presentations"
    complexity: "High - full technical depth"
    priority: "Medium - peer communication"
    
  educated_public:
    content: "Synthesized insights with practical implications"
    format: "Popular science articles, accessible presentations"
    complexity: "Medium - informed but accessible"
    priority: "High - broad impact potential"
    
  students_learners:
    content: "Educational materials with progressive complexity"
    format: "Tutorials, interactive learning materials"
    complexity: "Variable - scaffolded learning"
    priority: "High - future research capacity"
    
  general_public:
    content: "Inspiring stories and practical benefits"
    format: "Stories, visual presentations, demonstrations"
    complexity: "Low - intuitive understanding"
    priority: "Medium - public engagement"
    
  decision_makers:
    content: "Implications, applications, and impact"
    format: "Executive summaries, policy briefs"
    complexity: "Medium - strategic insights"
    priority: "High - implementation potential"
```

### 5. Knowledge Gaps and Question Generation
```yaml
Gap Analysis for Next Cycle:
  communication_challenges:
    complex_concepts: "Which integrated insights are hardest to explain?"
    missing_metaphors: "What visual or conceptual bridges are needed?"
    audience_confusion: "Where do audiences struggle with understanding?"
    
  incomplete_knowledge:
    unexplored_implications: "What consequences of discoveries need exploration?"
    missing_connections: "What relationships between findings need investigation?"
    practical_applications: "What real-world uses need development?"
    
  feedback_insights:
    audience_questions: "What questions do audiences consistently ask?"
    misunderstandings: "What concepts are frequently misunderstood?"
    interest_patterns: "What aspects generate most excitement or concern?"
    
  next_cycle_questions:
    exploration_needs: "What new areas should 히카리(Explorer) investigate?"
    design_requirements: "What systems should 아카네(Architect) structure?"
    implementation_gaps: "What tools should 츠구미(Craftsman) build?"
    validation_needs: "What claims should 레이(Skeptic) examine?"
    integration_opportunities: "What connections should 나나미(Synthesizer) explore?"
```

### 6. Presentation Strategy Development
```yaml
Communication Strategy:
  narrative_construction:
    main_story: "Central research narrative and its significance"
    supporting_stories: "Individual discovery stories and their context"
    character_development: "How research agents contribute to the story"
    plot_progression: "Research journey from discovery to application"
    
  accessibility_optimization:
    complexity_reduction: "Simplify without losing essential meaning"
    metaphor_development: "Create intuitive analogies and comparisons"
    visual_storytelling: "Design compelling visual representations"
    progressive_disclosure: "Structure information for different depth levels"
    
  engagement_enhancement:
    emotional_connection: "Connect discoveries to human values and needs"
    practical_relevance: "Show real-world impact and applications"
    curiosity_stimulation: "Inspire questions and further exploration"
    interactive_elements: "Enable audience participation and exploration"
```

### 7. Output Format
```yaml
Previous Context Summary:
  integrated_knowledge: "From Synthesizer - unified insights requiring communication"
  validated_foundations: "From Skeptic - reliable knowledge for accurate presentation"
  structural_frameworks: "From Architect - organizational principles for clear explanation"
  practical_tools: "From Craftsman - implementations requiring documentation"
  discovery_stories: "From Explorer - inspiring findings for narrative construction"
  
Communication Strategy:
  presentation_priorities: "Most important knowledge to communicate effectively"
  audience_adaptation: "Specific audience needs and communication approaches"
  narrative_construction: "Story frameworks for compelling presentation"
  accessibility_optimization: "Simplification and clarification strategies"
  engagement_enhancement: "Methods to inspire and motivate audiences"
  
Content Development Plan:
  technical_documentation: "User guides and implementation instructions"
  educational_materials: "Learning resources and progressive curricula"
  public_presentations: "Accessible explanations and inspiring stories"
  visual_communications: "Diagrams, animations, and interactive demonstrations"
  policy_briefs: "Strategic implications and decision-maker resources"
  
Next Cycle Preparation:
  knowledge_gaps_identified: "Areas needing further research and exploration"
  audience_feedback_insights: "Understanding challenges and interest patterns"
  communication_improvements: "Lessons for better future presentation"
  research_questions_generated: "New questions for next exploration cycle"
```

## Usage
- Execute automatically during agent activation
- Present communication opportunities based on integrated knowledge
- Focus on making complex insights accessible and inspiring
- Identify knowledge gaps and questions for next research cycle

## Communication Philosophy
Apply 지식 공유 (knowledge sharing wisdom):
- Honor the complexity while achieving accessibility
- Create emotional connections to rational insights
- Inspire curiosity and further exploration
- Enable knowledge to create positive impact
- Bridge the gap between experts and the broader community