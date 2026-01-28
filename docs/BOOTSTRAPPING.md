# Bootstrapping New Projects with Antigravity SDK

This guide explains how to transfer the skills, workflows, and "agentic brain" from this repository to a new project, ensuring compatibility with both **Claude Code** and **Google Antigravity**.

## 1. Directory Structure

To enable agentic capabilities, your new repository needs the following directory structure:

```text
new-repo/
├── .agent/
│   └── workflows/      # Custom slash commands (/design, /impl, etc.)
├── skills/             # Technical "how-to" guides and scripts
└── CLAUDE.md           # The bridging instruction file (Required)
```

## 2. Transferring Skills & Workflows

### Manual Bootstrapping
1.  **Workflows**: Copy the `.agent/workflows/` folder from this repo to your new repo's root.
2.  **Skills**: Copy the `skills/` folder to your new repo's root.
3.  **Bridge**: Copy the `CLAUDE.md` file to your new repo's root.

## 3. Dual-Agent Compatibility

The `CLAUDE.md` file is the "glue" that allows both agents to understand your project.

### Antigravity (Google)
Uses the `.agent/workflows/` directory to discover and run slash commands. It refers to `CLAUDE.md` for high-level personality and rules.

### Claude Code (Anthropic)
Relies heavily on `CLAUDE.md` to understand your build commands, test patterns, and style preferences.

> [!IMPORTANT]
> Always ensure your `CLAUDE.md` includes a **"Core Skills Reference"** section that links to the `skills/` directory. This tells the agent exactly where to find its domain-specific knowledge.

## 4. Verification

Once files are copied, verify by asking the agent in the new repo:
- "What slash commands do you have available?"
- "Can you summarize the skills you have access to in the /skills directory?"

If the agent can list `/design`, `/brainstorm`, etc., and explain the contents of `skills/`, your bootstrap was successful.
