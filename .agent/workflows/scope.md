---
description: Decide what to actually build and create a lightweight action plan. Picks the right format — UI mockup, workflow, feature, or doc.
---

# /scope

Use this workflow AFTER `/brainstorm` — once you have an approved design and need to decide exactly what to build and in what format. Claude will help you pick the right output type and create a simple, clear action plan.

## Core Principles
- **Right Tool for the Job**: Not everything needs code. Some ideas need a mockup. Some need a workflow diagram. Some need a simple document. Pick the right format first.
- **Start Small**: Scope the smallest version that still solves the core problem.
- **Clear Deliverable**: By the end of this workflow, you should know exactly what you're building and what "done" looks like.

## The Process

### 1. Load the Design Doc
- Read the approved design doc from `docs/plans/`.
- Summarize the core goal back to the user in one sentence.

### 2. Pick the Build Format
Ask the user: "What format makes most sense for this?"
- **UI Mockup** — You need to see what it looks like before building it. Claude creates a clickable HTML prototype.
- **Workflow / Process** — You need to map out the steps, decisions, or automation. Claude creates a flow diagram or step-by-step process doc.
- **Feature / App** — You're ready to build something functional. Claude creates an implementation plan.
- **Document / Template** — The output is a reusable doc, report, or template. Claude creates it directly.
- **Not sure** — If unclear, Claude recommends the best format based on the design.

### 3. Define the Scope
Once the format is chosen, get crisp on what's IN and OUT:

Ask:
- "What are the 3 most important things this needs to do?"
- "What can we leave out of the first version?"
- "Who needs to see or use this when it's done?"

### 4. Create the Action Plan
Write a lightweight, plain-language action plan:
- **What we're building**: 1-2 sentence description
- **Format**: UI mockup / workflow / feature / document
- **Steps**: numbered list of what needs to happen, in order
- **Done looks like**: specific, concrete description of the final output
- **Estimated effort**: small (< 1 hour), medium (half day), large (multiple sessions)

Save to `docs/plans/YYYY-MM-DD-<topic>-action-plan.md`.

### 5. Confirm Before Starting
Show the user the action plan and ask: "Ready to build? Use `/build` to start."

**Next Step**: Once the action plan is approved, use `/build` to execute it.
