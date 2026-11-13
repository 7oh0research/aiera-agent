# Repository Ruleset

This repository uses the active **main rules** ruleset

## Scope and status

- **Target:** Branches matching the repository's default branch (`~DEFAULT_BRANCH`).
- **Enforcement:** Active.
- **Bypass actors:** None are configured.

## Branch protections

- Branch deletion is blocked.
- Non-fast-forward updates are blocked, preventing force-pushes.

## Pull requests

- At least **1 approving review** is required before merging.
- All three merge methods are allowed: merge commits, squash merging, and rebase merging.
- A new push does not automatically dismiss stale approvals.
- Code-owner approval, approval of the latest push, and resolution of all review threads are not required by this ruleset.
- An extra approval is required for unattributed changes.

## Copilot code review

- Automatic Copilot review after new pushes is enabled.
- Review of draft pull requests is disabled.
- Copilot approvals require additional repository settings and are not configured by this ruleset file. In the repository's Copilot code review settings, enable both **Allow Copilot to approve pull requests** and **Allow Copilot approvals to count toward merge requirements**. Organization or enterprise policy must also permit Copilot approvals.
