# Architecture Overview

## High Level

```mermaid
graph TD

User --> AIEngineer
AIEngineer --> Planner
Planner --> DatabaseAgent
Planner --> CodeGeneratorAgent
Planner --> GitAgent

DatabaseAgent --> SqlTool
CodeGeneratorAgent --> FileTool
GitAgent --> GitTool
```

## Responsibilities

AIEngineer
- Accept user requests
- Orchestrates execution

Planner
- Creates execution plan

DatabaseAgent
- Reads database metadata

...
