# Context

## What We Are Solving

This portable workflow folder exists to help create simple AI-agent workflow systems from specific problems. The current challenge is making the process easy to start from the command prompt and easy to follow inside Codex.

The system should guide the user from an unclear problem to a working first version of a problem-specific workflow folder.

## Current Process

Without this folder, the user has to remember how to structure the workflow, what files to create, and what to ask Codex first. That creates friction and makes the system harder to use consistently.

## Desired Outcome

The user can open the root Codex workspace, type `New Project`, and be guided through creating a simple problem-specific workflow.

The result should be a new problem folder containing:

- `AGENT.md`
- `CONTEXT.md`
- `REFERENCES.md`

Generated problem folders should be created under `portable-skool-workflow/projects/`.

## What Good Looks Like

- Codex asks only the questions needed for version one.
- The workflow stays small and practical.
- The created files are clear enough to use immediately.
- The user can run a dry test against the new workflow.
- Expansion is suggested only when there is a real repeated need.

## What To Avoid

- Do not overbuild the system.
- Do not create `WORKFLOW.md` by default.
- Do not add routing tables, tools, skills, or automation by default.
- Do not ask abstract strategy questions before the practical basics are known.
- Do not create a complex folder structure before a simple test works.

## Simple Workflow

1. Intake: ask what specific problem the user wants to solve.
2. Organize: define the desired output, done state, and bad output.
3. Draft: create the simplest possible `AGENT.md`, `CONTEXT.md`, and `REFERENCES.md`.
4. Review: run one dry test and improve the files once based on what breaks.
