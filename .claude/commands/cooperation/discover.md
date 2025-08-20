# Workflow
User Input -> Cycle [ Explore -> Criticize ] -> Orchestraor

가장먼저 TODO list를 다음과 같이 만들어 : Phase 0 - Cycle (Phase 1) - Cycle (Phase 2) - Decision - Phase 3 

## Phase 0 : Understand user question
- Understand user question and make TODO List which iterates cycle 10 times. 이 task의 목적은 explorer와 skeptic이 모험적 탐구와 엄밀한 비판을 반복하며 결론을 도출하는 반복과정이야. 한번에 통과하기 어려운 엄밀한 체크리스트 만들고, .core/tools/checklists/discover-checklist.md로 작성해. // Think

## Cycle - Phase 1 : Explore
- Load '.claude/commands/explorer.md' and explore user's question successively. 'think'
## Cycle - Phase 2 : Criticize
- Load '.claude/commands/skeptic.md' and criticize Phase 1's exploration result. 'think
## Decision
- Repeat Phase 1 and 2 if the checklist in .core/tools/checklists/discover-checklist.md is not satisfied.  최대한 보수적으로 : (think)

## Phase 3 : Synthesize
- Load '.claude/commands/synthesizer.md' and synthesize the discussions and discoveries