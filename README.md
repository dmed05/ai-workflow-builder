# AI Workflow Builder

A small, local-first framework for turning a specific business problem into a
reviewable AI-agent workflow.

The framework keeps instructions, operating context, and references separate so
each workflow is portable, testable, and easy to improve. The repository uses
synthetic examples and intentionally excludes production records.

## Why this project exists

AI workflows often fail because requirements, source material, and output rules
are mixed into one large prompt. This project provides a repeatable three-file
contract:

- `AGENT.md` defines role, behavior, and quality standards.
- `CONTEXT.md` defines the operating process and review gates.
- `REFERENCES.md` defines approved sources and boundaries.

```text
problem definition
       ↓
three-file workflow contract
       ↓
dry run with synthetic inputs
       ↓
human review and one measured revision
```

## What I Built

I built a guided framework for converting a real business problem into a small,
portable AI-agent workspace. The framework includes a structured discovery
template, the three-file workflow contract, routing instructions, reusable
examples, security checks, and a repeatable dry-run and revision process.

The included synthetic projects demonstrate how the same framework can support
different operational problems without mixing their rules or source material.

## How It Supports My Operations

I use this framework to move from an informal process idea to a reviewable AI
workflow with clear boundaries. It helps me:

- define the operational problem before choosing tools;
- separate agent behavior, process context, and approved references;
- expose missing information and approval requirements early;
- test workflows with synthetic inputs before operational use;
- preserve a consistent structure across different projects; and
- publish reusable patterns without publishing production records.

The result is a faster, more disciplined way to prototype AI-assisted
operations while keeping humans responsible for consequential actions.

## My Role and Design Decisions

I designed the three-file contract, project-creation questionnaire, routing
conventions, human-review gates, synthetic examples, and public-repository
security policy.

The central design decision was to keep the initial framework deliberately
small. New tools or automation are added only when a repeated workflow failure
justifies the additional complexity.

## Structure

```text
ai-workflow-builder/
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

## Quick start

```bash
git clone https://github.com/dmed05/ai-workflow-builder.git
cd ai-workflow-builder
codex
```

Codex should auto-read `AGENTS.md`, then route through `CONTEXT.md`.

To start a workflow:

```text
New Project
```

Follow the guided questions, generate the three-file contract, then run one dry
test before expanding the structure.

## Included examples

- `customer-email-workflow`: synthetic intake-to-draft workflow with human
  review.
- `cleaning-schedule-management`: synthetic scheduling workflow with explicit
  unknowns and approval gates.

## Security model

This public repository is a clean-room demonstration. It does not accept:

- credentials or environment files;
- customer, employee, or account records;
- production documents, exports, photos, or videos;
- live schedules, pricing, contracts, or private operational notes.

Run the local publication gate before every push:

```bash
bash scripts/security-check.sh
```

Optional pre-commit installation:

```bash
python -m pip install pre-commit
pre-commit install
```

GitHub Actions repeats the policy scan and runs Gitleaks across repository
history.

## Project status

This is a portfolio reference implementation. It is intentionally minimal:
start with the three-file contract and add tooling only when a repeated failure
justifies it.

## License

MIT
