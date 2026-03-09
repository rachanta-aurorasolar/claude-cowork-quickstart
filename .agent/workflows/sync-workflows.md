---
description: Synchronize global agent workflows to the claude-code-quickstart repository.
---

# /sync-workflows

Use this workflow to synchronize gold-standard agent workflows between this repo and the `claude-code-quickstart` repository.

## The Process

1.  **Ask for Direction**: 
    - Ask the user: "Do you want to **PULL** the latest workflows from the global quickstart repo, or **PUSH** your current repo's updated workflows to the global repo?"

2.  **Execute Sync**:
    - **IF PULL**:
      - Run `chmod +x scripts/sync-workflows.sh`
      - Run `./scripts/sync-workflows.sh --pull`
    - **IF PUSH**:
      - Run `chmod +x scripts/sync-workflows.sh`
      - Run `./scripts/sync-workflows.sh --push`

3.  **Verify**:
    - Check `.agent/workflows/` or the quickstart repo to see that files are updated.

**Note**: This assumes `claude-code-quickstart` is located at `../claude-code-quickstart`.
// turbo-all