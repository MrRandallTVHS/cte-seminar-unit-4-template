# Unit 4: Software Design and Architecture

This repository contains the starter materials for the Unit 4 seminar tasks.

## Before You Begin

1. Create your own repository from the instructor's template repository by selecting **Use this template**.
2. Clone your personal repository to your computer.
3. Complete Task 1 on the `main` branch.
4. Create a branch named `task-2` before beginning Task 2.
5. Commit meaningful changes and push them to your personal repository.

Do not push work to the instructor's template repository.

## Repository Organization

- `reference/` contains materials used by both tasks. Do not edit these files.
- `task1-design-patterns/starter/` contains the original Task 1 code.
- `task1-design-patterns/refactored/` is where the refactored Task 1 code belongs.
- `task2-microservices/starter/` contains the original monolithic code.
- `task2-microservices/services/` is where the Task 2 service code belongs.
- `requirements.txt` lists the Python packages used by the microservice task.

## Submission Locations

Use GitHub for code development and commit history. Upload the written work and evidence to Canvas.

### GitHub Deliverables

- Refactored Task 1 code
- Task 2 microservice code
- Orchestrator code
- Required runtime files
- Commit history for the work

### Canvas Deliverables

- Task 1 pattern analysis
- UML diagrams
- Task 1 design explanations
- Task 1 commit-history screenshot
- Task 2 architecture analysis
- Cloud or on-premises discussion
- Monolithic and microservices explanation
- README documentation
- Test results or screenshots
- Task 2 commit-history screenshot
- GitHub repository URL

## Task 1

Read `task1-design-patterns/starter/retail_patterns.py`. Place only your refactored code in `task1-design-patterns/refactored/`. Complete the written analysis and UML diagrams separately for Canvas.

## Task 2

Read `task2-microservices/README.md` before changing code. The original monolithic system is in `task2-microservices/starter/monolithic_retail_system.py`. Service responsibilities and required endpoints are described in `task2-microservices/SERVICE_CONTRACTS.md`. Place only your Python service code in `task2-microservices/services/`. Submit the written architecture analysis, README documentation, test evidence, and screenshots through Canvas.

## Python Environment

Create and activate a virtual environment before installing the requirements:

```text
python -m venv .venv
```

Windows PowerShell activation:

```text
.venv\Scripts\Activate.ps1
```

macOS or Linux activation:

```text
source .venv/bin/activate
```

Install packages:

```text
python -m pip install -r requirements.txt
```
