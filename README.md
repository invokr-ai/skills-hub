# skill hub

A collection of skills. Each skill is a `SKILL.md` instruction pack an agent
loads on demand.

## Layout

Each skill is a directory under `skills/` containing a `SKILL.md` with
`name` and `description` frontmatter followed by the instructions:

```
skills/<name>/SKILL.md
```

## Skills

- `code-review` — review a diff or branch for correctness, clarity, scope creep.
- `commit` — write a clean conventional commit, splitting unrelated work.
- `debugging` — reproduce, hypothesize, instrument, confirm, then fix.
- `grilling` — interview the user until every open branch is resolved.
- `plan` — research, then write an implementation plan, then stop.
- `ponytail` — force the laziest solution that works.
- `skill-authoring` — write a new skill.
- `spec-checklist` — turn a task spec into an explicit checklist and verify each item.
- `spike` — validate an idea with a throwaway experiment first.
- `tdd` — test-first red-green-refactor.
- `verification-before-completion` — run the verification command before claiming done.

## Drafts

`drafts/` holds candidate skills as `SKILL.draft.md` files, not yet promoted
to `skills/`.

## Sources

Some skills are adapted from other public skill collections rather than
written from scratch here. Each adapted skill carries a `source:` field in
its frontmatter; the collections referenced so far:

- [mattpocock/skills](https://github.com/mattpocock/skills) — `grilling`,
  `tdd`, `code-review`, `drafts/handoff`, `drafts/merge-conflicts`.
- [DietrichGebert/ponytail](https://github.com/DietrichGebert/ponytail) (MIT) — `ponytail`.
- Claude Code's own built-in `/simplify` skill (Anthropic) — `drafts/simplify`.
- [obra/superpowers](https://github.com/obra/superpowers) (MIT) — `verification-before-completion`.
- [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) (MIT) — `spec-checklist`.

`ATTRIBUTION.md` records upstream commit, licence text, and what was changed
for each vendored or adapted skill.

Checked but not attributed for lack of a single confident match: `commit`,
`debugging`, `plan`, `skill-authoring`, `spike`, `drafts/pr-workflow`,
`drafts/humanizer`, `drafts/grounded-citations` — each shares a name/concept
with several independently-written public skills, but none matched closely
enough to credit one over the others.
