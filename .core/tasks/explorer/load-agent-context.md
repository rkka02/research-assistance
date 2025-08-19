# Load Agent Context - 히카리 (Explorer) Memory System

## Purpose
Load previous agent work to understand what has been discovered, implemented, verified, or synthesized before starting new exploration.

## Implementation

### 1. Read Previous Agent Essential Context
```yaml
Read .core/.agent-memory/shared-knowledge/project-state.yaml
- Check current_phase and collective_discoveries
- Understand overall project direction

Read .core/.agent-memory/agent-workspaces/*/essential.yaml
- Load critical findings from other agents
- Identify collaboration_value and breakthrough_potential
- Note available resources for building upon
```

### 2. Load Relevant Agent Work
```yaml
Priority Loading Order:
1. Skeptic (레이) - validated insights and confidence levels
2. Synthesizer (나나미) - integrated knowledge and unified patterns  
3. Architect (아카네) - structural frameworks and design insights
4. Craftsman (츠구미) - implemented tools and scripts in /scripts/ and /executables/
5. Communicator (모모카) - presentation insights and knowledge gaps
```

### 3. Context Integration
```yaml
Integration Process:
- Synthesize previous findings into exploration starting points
- Identify unexplored territories and research gaps
- Build upon validated patterns with new discovery angles
- Connect to available tools from Craftsman workspace
- Note areas requiring validation or verification
```

### 4. Output Format
```yaml
Previous Context Summary:
  validated_insights: "From Skeptic validation work"
  available_tools: "From Craftsman implementations" 
  structural_frameworks: "From Architect designs"
  knowledge_gaps: "From all agents' open questions"
  exploration_opportunities: "New discovery potential"
  
Exploration Strategy:
  build_upon: "Specific previous findings to extend"
  investigate_gaps: "Unexplored territories to explore"
  validate_hypotheses: "Unverified patterns to examine"
  connect_domains: "Cross-domain opportunities to pursue"
```

## Usage
- Execute automatically during agent activation
- Present concise summary to user showing previous work
- Use insights to guide discovery strategy and priorities
- Ensure exploration builds on team's collective knowledge