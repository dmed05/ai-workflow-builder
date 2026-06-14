# Builder Development Workflow

This is a GitHub-safe, sanitized version of the Builder Development Workflow workspace.

It contains the reusable workflow-building system and sanitized example project workflows. It intentionally excludes customer documents, account folders, private notes, live schedules, PDFs, photos, videos, email exports, and other sensitive materials.

## Structure

```text
Builder Development Workflow/
├── AGENTS.md
├── CONTEXT.md
├── AI Agent Problem Workflow Template.md
├── README.md
├── md-preview.html
├── workspace-skills/
└── portable-skool-workflow/
    ├── builder/
    └── projects/
        ├── customer-email-workflow/
        └── cleaning-schedule-management/
```

## Start

```bash
codex
```

Codex should auto-read `AGENTS.md`, then route through `CONTEXT.md`.

To start a new workflow project:

```text
New Project
```

## Safety Rule

Keep private customer materials local. Do not commit:

- customer/account folders
- PDFs, W-9s, insurance documents, contracts, or vendor forms
- photos or videos
- email exports or mailbox contents
- live customer schedules
- account briefs with private details

Use sanitized examples when publishing to GitHub.
