---
name: spec-checklist
description: Extract every concrete requirement from a task spec into an explicit checklist, implement against it, and re-verify each item against real output before finishing.
source: "Adapted from addyosmani/agent-skills (spec-driven-development) (MIT), https://github.com/addyosmani/agent-skills — see ATTRIBUTION.md"
---

# Spec Checklist

Code without a checklist is guessing. Before writing code, and again before claiming done,
turn the task spec into an explicit, checkable list.

## 1. Extract the checklist

Re-read the task spec and pull out every concrete, testable requirement:

- Exact strings the output must contain (error messages, log lines, flag names)
- File paths that must exist or be modified
- Formats (JSON shape, CLI output layout, exit codes)
- Named flags, env vars, and their exact spelling
- Commands the spec says must run (build, test, lint) and what "pass" means for each

Write these as a literal checklist, one line per requirement:

```markdown
- [ ] Exact string "..." appears in output of `command`
- [ ] File path/to/thing.go exists and contains X
- [ ] Flag --foo accepts value bar
- [ ] `make test` exits 0
```

Do not paraphrase requirements into vaguer language — keep the spec's exact strings, paths,
and names in the checklist so verification can match them literally.

## 2. Implement against it

Work through the checklist in order. Each item is done only when there is concrete evidence
for it, not when it seems implemented.

## 3. Re-verify before finishing

Before writing a final answer, go back through the checklist and, for each item, find the
actual command output or diff line that proves it — not your memory of having written the
code:

```
✅ Re-read spec → checklist item → run the command / grep the output → confirmed
❌ "I implemented that" without pointing at output
```

Report the checklist with each item checked or explicitly marked unfinished with the reason.
Never report done while an item lacks evidence.

## Red Flags

- Skipping straight to code because "the spec is obvious"
- A checklist item marked done with no command output or diff to back it up
- Paraphrasing an exact string/path/flag from the spec instead of copying it verbatim
- Claiming done without walking the full checklist one more time against real output
