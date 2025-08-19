# Load Agent Context - 츠구미 (Craftsman) Memory System

## Purpose
Load previous agent work to understand designs, frameworks, discoveries, and validated insights that need precise implementation.

## Implementation

### 1. Read Previous Agent Essential Context
```yaml
Read .core/.agent-memory/shared-knowledge/project-state.yaml
- Check current_phase and collective_discoveries
- Understand implementation requirements and quality standards

Read .core/.agent-memory/agent-workspaces/*/essential.yaml
- Load collaboration_value from all agents
- Identify critical_designs, key_patterns, validated_insights
- Note implementation_value and collaboration_assets
```

### 2. Load Relevant Agent Work (Priority Order)
```yaml
Priority Loading Order:
1. Architect (아카네) - detailed designs and frameworks requiring implementation
2. Explorer (히카리) - discovered patterns needing computational tools
3. Skeptic (레이) - validated insights requiring systematic implementation
4. Synthesizer (나나미) - integrated knowledge needing operational tools
5. Communicator (모모카) - presentation tools and automation needs
```

### 3. Implementation Planning
```yaml
Implementation Assessment:
- Identify architectural designs requiring coding implementation
- Analyze discovered patterns needing computational tools
- Evaluate validated results requiring automated processing
- Map integration requirements to script organization
- Plan testing and quality assurance protocols
```

### 4. Scripts/Executables Organization Check
```yaml
Current Assets Inventory:
  scripts/:
    data/: "Data processing scripts"
    analysis/: "Analysis and computation scripts" 
    utils/: "Utility and helper scripts"
    automation/: "Workflow automation scripts"
    
  executables/:
    apps/: "Standalone applications"
    tools/: "Specialized tools"
    libs/: "Library binaries"
    packages/: "Deployment packages"
    
  tests/:
    unit/: "Unit test suites"
    integration/: "Integration tests"
    performance/: "Performance benchmarks"
    validation/: "Validation protocols"
    
  documentation/:
    technical/: "Technical documentation"
    user_guides/: "User documentation"
    api_docs/: "API documentation"
```

### 5. Output Format
```yaml
Previous Context Summary:
  designs_to_implement: "From Architect - frameworks requiring coding"
  patterns_to_automate: "From Explorer - discoveries needing tools"
  validated_requirements: "From Skeptic - verified implementation needs"
  integration_needs: "From Synthesizer - unified tools requirements"
  presentation_automation: "From Communicator - display and export tools"
  
Implementation Strategy:
  priority_implementations: "Highest priority coding tasks"
  quality_requirements: "Precision and reproducibility standards"
  testing_protocols: "Validation and verification needs"
  organization_plan: "Scripts/executables categorization strategy"
  existing_assets: "Available tools and scripts for building upon"
```

## Usage
- Execute automatically during agent activation
- Present implementation priorities based on previous agent work
- Show current assets available in scripts/ and executables/
- Focus on systematic implementation of validated designs