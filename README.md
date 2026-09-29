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
- `task1-design-patterns/` contains Task 1 starter code and student work.
- `task2-microservices/` contains Task 2 starter code and student work.
- `requirements.txt` lists the Python packages used by the microservice task.

## Task 1

Read `task1-design-patterns/starter/retail_patterns.py`. Record your analysis in `task1-design-patterns/analysis.md`, place UML diagrams in `task1-design-patterns/diagrams/`, and place refactored code in `task1-design-patterns/refactored/`.

## Task 2

Read `task2-microservices/README.md` before changing code. The original monolithic system is in `task2-microservices/starter/monolithic_retail_system.py`. Service responsibilities and required endpoints are described in `task2-microservices/SERVICE_CONTRACTS.md`.

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

