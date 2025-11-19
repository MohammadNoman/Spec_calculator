<!-- Sync Impact Report:
Version change: 1.2.0 -> 1.2.1
List of modified principles:
- Code Quality Standards (Refined)
Added sections: None
Removed sections: None
Templates requiring updates:
- .specify/templates/plan-template.md: ⚠ pending
- .specify/templates/spec-template.md: ⚠ pending
- .specify/templates/tasks-template.md: ⚠ pending
- .specify/templates/commands/*.md: ✅ Not found / N/A
- README.md: ✅ Not found / N/A
Follow-up TODOs: None
-->
# calculator-project Constitution

## Core Principles

### I. Write tests first (TDD approach)
Every new feature or bug fix must be accompanied by tests written before the implementation. This ensures a clear understanding of requirements and validates correctness. The Red-Green-Refactor cycle is strictly enforced.

### II. Use Python 3.12+ with type hints everywhere
All Python code must be written using Python 3.12 or newer. Type hints must be used consistently throughout the codebase to improve readability, maintainability, and enable static analysis.

### III. Keep code clean and easy to read
Code must be self-documenting where possible, adhering to established style guides (e.g., PEP 8). Complexity should be minimized, and readability prioritized to facilitate collaboration and long-term maintenance.

### IV. Document important decisions with ADRs
Architecturally significant decisions, including design choices, technology selections, and major changes, must be documented using Architecture Decision Records (ADRs). ADRs provide context, rationale, and consequences for future reference.

### V. Follow essential Object-Oriented Programming principles: SOLID, DRY, KISS
The codebase must adhere to fundamental Object-Oriented Programming (OOP) principles:
- **SOLID:** Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, Dependency Inversion.
- **DRY:** Don't Repeat Yourself – avoid duplication of code and knowledge.
- **KISS:** Keep It Simple, Stupid – favor simplicity over unnecessary complexity.

## Technical Stack

The project will utilize the following technical stack:
- **Language:** Python 3.12+
- **Package Manager:** UV
- **Testing Framework:** pytest
- **Version Control:** All project files must be managed under Git.

## Quality Requirements

The following quality gates and standards must be met:
- **Test Pass Rate:** All automated tests must pass successfully.
- **Code Coverage:** A minimum of 80% code coverage must be maintained for all new and modified code.
- **Data Structures:** `dataclasses` must be used for defining data structures to ensure clarity and immutability where appropriate.

## Code Quality Standards

To ensure maintainability, readability, and correctness, all code must adhere to the following standards:

- All functions must include type hints on parameters and return types
  - Example: `def add(a: float, b: float) -> float:`
- All functions must include docstrings explaining what they do
  - Example: `"""Add two numbers and return the sum."""`
- Follow PEP 8 naming conventions (lowercase_with_underscores for functions)
- Lines must be under 100 characters
- No magic numbers; use named constants
  - Bad: `if x > 10:`
  - Good: `if x > MAX_POWER_EXPONENT:`

## Governance
This constitution outlines the foundational principles and standards for the `calculator-project`. It supersedes any conflicting practices. Amendments to this constitution require a documented proposal, team approval, and a clear migration plan if existing practices are affected. Compliance with these principles will be reviewed during code reviews and project milestones.

**Version**: 1.2.1 | **Ratified**: 2025-11-10 | **Last Amended**: 2025-11-19