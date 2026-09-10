# Attribution

Provenance for skills in this hub that originate outside it. Each entry records
the upstream source, the upstream commit it was taken from, the licence, what
was changed, and the date it was added here.

## skills/verification-before-completion

- **Upstream:** [obra/superpowers](https://github.com/obra/superpowers),
  `skills/verification-before-completion/SKILL.md`
- **Upstream commit:** `3be5aad3dd2400ef23b15680969f4bcd3b6d7b8b` (HEAD of `main` for that
  path as of 2026-09-10)
- **Licence:** MIT — Copyright (c) 2025 Jesse Vincent (full text below)
- **Modified:** nothing. The instruction body is vendored verbatim. Only a
  `source:` field was added to the existing frontmatter.
- **Added:** 2026-09-10

## skills/spec-checklist

- **Upstream:** [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills),
  `skills/spec-driven-development/SKILL.md`
- **Upstream commit:** `cda4542ade0f3c532494b9a48837eb01d39925f1` (HEAD of `main` for that
  path as of 2026-09-10)
- **Licence:** MIT — Copyright (c) 2025 Addy Osmani (full text below)
- **Modified:** substantially. Upstream is a 245-line four-phase gated PRD
  workflow (Scope Check → Specify → Plan → Tasks → Implement) with human review
  gates between phases. This skill is a rewrite that keeps only the checklist
  idea and upstream's "code without a spec is guessing" framing, reduced to a
  single extract → implement → re-verify loop with no PRD artefact and no
  review gates. Renamed `spec-driven-development` → `spec-checklist`, and the
  name/description frontmatter rewritten to match.
- **Added:** 2026-09-10

---

## MIT License — obra/superpowers

```
MIT License

Copyright (c) 2025 Jesse Vincent

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## MIT License — addyosmani/agent-skills

```
MIT License

Copyright (c) 2025 Addy Osmani

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
