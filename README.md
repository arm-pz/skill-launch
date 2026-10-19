# skill-launch

**Create, validate, and publish a new skill in one pipeline.**

When you have an idea for a skill and want to take it from concept to published capability, skill-launch orchestrates the entire workflow. It drafts the skill with Draft-Skill (confirming purpose, checking siblings, writing structure), validates and tunes it with Tune-Skill (fixing triggers, resolving overlaps, validating with check_skill.py), then audits discoverability and polishes it with Findable-Polish (improving SEO, refining descriptions). You get a production-ready skill with all three phases handled sequentially.

## Usage

```text
/skill-launch "I want a skill that checks if my code is production-ready"
/skill-launch [paste list of prompts the skill should handle]
Create a skill that audits repos before deployment.
```

## When to use

- You have an idea for a skill and want to build it completely
- Someone says "make me a skill for X" and you want it done end-to-end
- You want triggering, validation, and discoverability all handled
- You're creating multiple skills and want a consistent pipeline
- You need a skill that's ready to publish without manual cleanup

## What it produces

- A drafted SKILL.md with correct frontmatter and structure (from Draft-Skill)
- Validated triggers and resolved sibling overlaps (from Tune-Skill)
- check_skill.py validation (FAIL/WARN/PASS)
- Polished descriptions and improved discoverability (from Findable-Polish)
- A production-ready skill folder ready to commit and push

## Install

```bash
npx skills add arm-pz/skill-launch
```

## Dependencies

Requires `draft-skill`, `tune-skill`, `findable-polish` (which needs `findable` + `wordsmith`) to be installed.

## Not for

- Editing existing skills → use [tune-and-polish](https://github.com/arm-pz/tune-and-polish)
- Just drafting without polishing → use [draft-skill](https://github.com/arm-pz/draft-skill) alone

## Related

- **[draft-skill](https://github.com/arm-pz/draft-skill)** — Create skills from ideas (phase 1)
- **[tune-skill](https://github.com/arm-pz/tune-skill)** — Validate and fix triggers (phase 2)
- **[findable-polish](https://github.com/arm-pz/findable-polish)** — Audit and polish discoverability (phase 3)
- **[tune-and-polish](https://github.com/arm-pz/tune-and-polish)** — Tune + polish existing skills

## License

MIT © Abdul Rahman P Z
