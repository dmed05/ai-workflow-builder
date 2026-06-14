# AI Agent Problem Workflow Template

Use this template to turn one specific problem into a simple workflow an AI agent can help you run.

The goal is not to build a complex system. The goal is to make one problem easier to understand, repeat, and improve.

Start with one problem, one folder, and three files:

```text
portable-skool-workflow/projects/problem-name/
├── AGENT.md
├── CONTEXT.md
└── REFERENCES.md
```

---

## Fast Start With Codex

From a terminal, open this folder:

```bash
cd "/home/dm/Builder Development Workflow"
codex
```

Then send this first message:

```text
New Project

Use the Skool-style system from AI Agent Problem Workflow Template.md.

Ask me one question at a time and help me create a working first version as fast as possible.

The output should be one problem folder under portable-skool-workflow/projects/ with:
- AGENT.md
- CONTEXT.md
- REFERENCES.md

Do not add extra files or complexity unless I ask.
```

Codex should then guide you through the setup by asking only the questions needed to create the first working version.

---

## Guided Setup Flow

Codex should walk through these steps:

1. Ask what specific problem you want to solve.
2. Ask what the agent should produce when the workflow works.
3. Ask what bad or annoying output looks like.
4. Draft the simplest possible `AGENT.md`.
5. Draft the simplest possible `CONTEXT.md`.
6. Draft a minimal `REFERENCES.md`.
7. Create the problem folder and files.
8. Run one dry test using the new files.
9. Make one improvement pass based on the dry test.

The goal is a usable first version, not a perfect system.

---

## 1. Pick One Specific Problem

### Problem Name

[Name the problem in plain language.]

Example:

```text
Missed Follow-Ups After Sales Calls
```

### The Problem

[Describe what is currently hard, slow, inconsistent, or easy to forget.]

Example:

```text
After sales calls, follow-up messages are inconsistent. Some leads get a clear next step, some get a late response, and some are forgotten entirely. Notes are spread across call transcripts, email, and memory.
```

### Why It Matters

[Explain the cost of not fixing this.]

Example:

```text
Missed follow-ups create lost deals, weaker trust, and extra mental load because every call has to be remembered manually.
```

---

## 2. Define The Desired Result

### Desired Outcome

When this workflow works, the agent should help me:

- [Outcome 1]
- [Outcome 2]
- [Outcome 3]

Example:

```text
When this workflow works, the agent should help me turn every sales call into a clear follow-up email, a next-step checklist, and a reminder of what still needs human review.
```

### Definition Of Done

The workflow is complete when:

- [Done condition 1]
- [Done condition 2]
- [Done condition 3]

Example:

```text
The workflow is complete when:
- A follow-up email draft exists.
- Missing information is clearly marked.
- Next steps are listed.
- Anything requiring human judgment is flagged.
```

---

## 3. Create The Three Core Files

Create a folder named after the problem under `portable-skool-workflow/projects/`.

Example:

```text
portable-skool-workflow/projects/sales-call-follow-up/
```

Then create:

```text
portable-skool-workflow/projects/sales-call-follow-up/
├── AGENT.md
├── CONTEXT.md
└── REFERENCES.md
```

---

## 4. AGENT.md

`AGENT.md` is the map. Keep it short.

Copy this into `AGENT.md` and fill in the brackets.

```markdown
# [Problem Name]

## Identity

You are helping [YOUR NAME / TEAM] solve [SPECIFIC PROBLEM].

## Goal

Help turn [MESSY CURRENT PROCESS] into [CLEAR USEFUL OUTPUT].

## Read First

1. Read AGENT.md first.
2. Read CONTEXT.md before doing the work.
3. Read REFERENCES.md only when examples, links, or background are needed.

## Rules

- Use plain, clear language.
- Ask when required information is missing.
- Do not invent facts. If something is missing, mark it as missing.
- Keep the workflow simple unless I ask to expand it.
- Put final answers in the format I request.
```

---

## 5. CONTEXT.md

`CONTEXT.md` explains the actual work.

Copy this into `CONTEXT.md` and fill in the brackets.

```markdown
# Context

## What We Are Solving

[Describe the problem in 2-5 sentences.]

## Current Process

[Describe how the work happens now. Include what is slow, confusing, inconsistent, or easy to miss.]

## Desired Outcome

[Describe what should be easier when this workflow works.]

## What Good Looks Like

- [Success condition 1]
- [Success condition 2]
- [Success condition 3]

## What To Avoid

- [Mistake or behavior to avoid]
- [Mistake or behavior to avoid]
- [Mistake or behavior to avoid]

## Simple Workflow

1. Intake: review the available information.
2. Organize: separate useful information from noise.
3. Draft or execute: create the useful output.
4. Review: check the output against what good looks like and what to avoid.
```

---

## 6. REFERENCES.md

`REFERENCES.md` holds examples and background.

Copy this into `REFERENCES.md` and fill in only what is useful.

```markdown
# References

## Good Examples

[Paste examples or describe what good output looks like.]

## Bad Examples

[Optional: describe examples or mistakes to avoid.]

## Useful Links

- [Link or file path]
- [Link or file path]

## Notes

[Any extra context the agent may need sometimes.]
```

---

## 7. First Prompt To Run The Workflow

Use this after the three files exist.

```text
Read AGENT.md and CONTEXT.md first.

I want to work on this task:
[SPECIFIC TASK]

Use the simple workflow in CONTEXT.md:
1. Intake
2. Organize
3. Draft or execute
4. Review

Before doing the task, tell me if anything important is missing.

Output format:
[LIST / TABLE / DRAFT / CHECKLIST / SUMMARY]
```

---

## 8. Filled Example

This is what the system looks like when filled in for one real problem.

### Problem Folder

```text
sales-call-follow-up/
├── AGENT.md
├── CONTEXT.md
└── REFERENCES.md
```

### AGENT.md Example

```markdown
# Sales Call Follow-Up

## Identity

You are helping me turn sales call notes into clear follow-up actions.

## Goal

Help turn scattered call notes into a follow-up email draft, a next-step checklist, and a list of missing information.

## Read First

1. Read AGENT.md first.
2. Read CONTEXT.md before doing the work.
3. Read REFERENCES.md only when examples, links, or background are needed.

## Rules

- Do not invent details from the call.
- Mark missing information clearly.
- Keep follow-up emails short and direct.
- Separate facts from suggested next steps.
```

### CONTEXT.md Example

```markdown
# Context

## What We Are Solving

After sales calls, follow-up is inconsistent. Notes may be in a transcript, a notebook, or a short memory dump. The agent should help convert those notes into a clear follow-up email and next-step checklist.

## Current Process

I finish a call, then manually remember what was discussed, what was promised, and what needs to happen next. This causes delays and missed follow-ups.

## Desired Outcome

Each call should produce a follow-up draft, a list of action items, and a short list of missing details that need human review.

## What Good Looks Like

- The email sounds professional and specific.
- The next steps are clear.
- Missing details are marked instead of guessed.

## What To Avoid

- Do not overpromise.
- Do not include internal notes in the client email.
- Do not make up deadlines, pricing, or commitments.

## Simple Workflow

1. Intake: read the call notes or transcript.
2. Organize: identify facts, requests, promises, objections, and next steps.
3. Draft: create the follow-up email and action checklist.
4. Review: flag missing information and risky claims.
```

### REFERENCES.md Example

```markdown
# References

## Good Examples

A good follow-up email is short, specific, and ends with a clear next step.

## Notes

Use a direct but helpful tone. Avoid hype.
```

### First Agent Prompt Example

```text
Read AGENT.md and CONTEXT.md first.

I want to turn these call notes into a follow-up email and next-step checklist:

[PASTE CALL NOTES]

Use the simple workflow in CONTEXT.md:
1. Intake
2. Organize
3. Draft
4. Review

Before doing the task, tell me if anything important is missing.

Output format:
1. Missing information
2. Organized call summary
3. Follow-up email draft
4. Next-step checklist
```

---

## 9. When To Expand

Only expand when the simple version starts breaking.

Add a `WORKFLOW.md` only if:

- the process has many steps
- the agent keeps skipping steps
- multiple people need to run the process
- the workflow needs checkpoints or approvals

Add folders only if:

- you have more than 8-10 files
- drafts and finals are getting mixed together
- raw inputs need to stay untouched

Do not add complexity because it seems impressive. Add it only when there is a repeated problem the current structure cannot solve.

---

## 10. Final Rule

Use the system first. Improve it second.

The first version should be small enough to build in 15 minutes.
