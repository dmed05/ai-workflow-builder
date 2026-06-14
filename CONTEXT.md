# Workspace Context

## What This Workspace Is

This is a GitHub-safe Builder Development Workflow workspace. It helps create portable Skool-style AI-agent workflow projects without publishing private customer data.

## Routing Rules

- If the user types `New Project` or wants to create a new workflow, use `AI Agent Problem Workflow Template.md`.
- If the user wants to work on a sanitized example, route to `portable-skool-workflow/projects/`.
- If the user wants to improve the workflow-building process, route to `portable-skool-workflow/builder/`.
- If the user mentions a reusable repeated process, check `workspace-skills/`.

## Privacy Rules

Do not commit or publish customer documents, account folders, private notes, live schedules, PDFs, photos, videos, email exports, or personally identifying operational details.

Use placeholders and sanitized examples in published workflows.

## Project Shape

New workflow projects should start with:

```text
AGENT.md
CONTEXT.md
REFERENCES.md
```

Create them under:

```text
portable-skool-workflow/projects/<problem-name>/
```

## GitHub Publishing Rule

This sanitized export is safe to push. The private local workspace history is not safe to push because it may contain sensitive files in commit history.
