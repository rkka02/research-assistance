# Workflow
User Input을 보면 1. {agent1} : 작업 A를 해줘. 2. {agent2} : 작업 B를 해줘. 3. {agent3} : 작업 C를 해줘, 4. ~
이런식으로 있을거야.

그러면 너의 역할은 순차적으로 1번 2번 3번, 4번, ...을 불러와서 순차적으로 일을 시키는거지.



가장먼저 TODO list를 다음과 같이 만들어 : (1) Task1 -> (2) Task2 -> (3) Task3 -> ...

For each task-i:
    Load .claude/commands/{agent-i}.md & 개인 기억과 팀 기억을 로드.
    각자의 워크플로우를 따라 {task-i}를 수행.
    각각의 {agent-i}가 개인 기억과 팀 기억을 저장하며 마무리.
    TODO list - i를 완료했다고 체크 후 다음 task로 진행

모든 작업이 끝나고 TODO 리스트가 완성되면 마지막으로 팀 기억을 저장하고 마무리.