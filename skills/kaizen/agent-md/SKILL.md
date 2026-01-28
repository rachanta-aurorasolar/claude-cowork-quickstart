---
name: agent-md-refactor
description: Refactor bloated agent instruction files using progressive disclosure principles.
---

# Agent MD Refactor

Refactor bloated agent instruction files (CLAUDE.md, etc.) to follow **progressive disclosure principles** - keeping essentials at root and organizing the rest into linked, categorized files.

## Triggers
Use this skill when:
- Instruction files (like CLAUDE.md) exceed 500 lines.
- There are contradictions in the instructions.
- The root file is difficult to navigate.

## Process
1. **Analyze**: Find contradictions and redundant instructions.
2. **Extract**: Identify core instructions that *must* stay in the root file.
3. **Categorize**: Group remaining instructions into logical categories.
4. **Structure**: Create a file hierarchy (Root + linked files in `.agent/instructions/`).
5. **Prune**: Flag vague or obsolete instructions for deletion.

## Quick Reference
| Phase | Action | Output |
| :--- | :--- | :--- |
| 1. Analyze | Find contradictions | List of conflicts to resolve |
| 2. Extract | Identify essentials | Core instructions for root file |
| 3. Categorize | Group remaining instructions | Logical categories |
| 4. Structure | Create file hierarchy | Root + linked files |
| 5. Prune | Flag for deletion | Redundant/vague instructions |
