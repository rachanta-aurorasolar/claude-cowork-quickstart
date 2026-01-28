---
name: reducing-entropy
description: Manual-only skill for minimizing total codebase size. Focuses on deletion and minimalism.
---

# Reducing Entropy

More code begets more code. Entropy accumulates. This skill biases toward the smallest possible codebase.

**Core question:** "What does the codebase look like *after*?"

## The Goal
The goal is **less total code in the final codebase** - not less code to write right now.
- Writing 50 lines that delete 200 lines = net win.
- Keeping 14 functions to avoid writing 2 = net loss.

## Three Questions
1. **What's the smallest codebase that solves this?** Not the smallest change, but the smallest result.
2. **Does the proposed change result in less total code?** Count lines before and after. If after > before, reconsider.
3. **What can we delete?** Every change is an opportunity to remove obsolete code.

## Red Flags
- "Keep what exists" (Status quo bias).
- "This adds flexibility" (YAGNI).
- "Better separation of concerns" (separation isn't free, it costs lines).
