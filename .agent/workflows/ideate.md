---
description: Start here. Claude interviews you to capture your problem, ideas, and goals before anything gets built.
---

# /ideate

Use this workflow when you have an idea or a problem and need to think it through out loud before building anything. Claude will interview you — one question at a time — to help you get your thoughts out clearly.

## Core Principles
- **You Lead, Claude Listens**: This is YOUR brain dump. Claude's job is to ask good questions, not give answers yet.
- **One Question at a Time**: Never overwhelm. Ask one thing, wait for the answer, then go deeper.
- **No Jargon**: Keep it conversational. No technical language unless the user brings it up.
- **Problems First, Solutions Later**: Understand the pain before jumping to what to build.

## The Process

### 1. Warm Up
Start with a completely open, friendly question:
- "Tell me about the problem you're trying to solve — what's been frustrating you?"
- Let the user answer freely. Don't redirect yet.

### 2. Go Deeper (Interview Mode)
Ask follow-up questions one at a time based on what they say. Cover these areas naturally (not as a checklist):
- **The problem**: What's going wrong? How often? How painful is it?
- **Who it affects**: Is this just you, or does a team / customer experience this too?
- **What you've tried**: Have you worked around it? What didn't work?
- **The dream**: If this was solved perfectly, what would that look like?
- **Ideas you already have**: Do you have any instincts about how to fix it?

### 3. Reality Check
Before wrapping up, ask:
- "Is there anything else you want to get out of your head before we start shaping this?"
- "Any constraints I should know about — time, tools, budget, team size?"

### 4. Synthesize
Once the interview feels complete, summarize back to the user:
- Restate the core problem in 1-2 sentences.
- List the key ideas or solutions they mentioned.
- Call out any tensions or open questions.
- Ask: "Does this capture it? Anything to add or change?"

### 5. Save the Idea Brief
Write a clean summary to `docs/plans/YYYY-MM-DD-<topic>-idea-brief.md` with:
- **The Problem**: What are we solving and why it matters?
- **Who It's For**: Who experiences this problem?
- **Ideas on the Table**: What approaches came up?
- **Success Looks Like**: What does "done" feel like?
- **Open Questions**: What still needs to be figured out?

**Next Step**: Once the Idea Brief feels right, use `/scope` to figure out what to actually build.
