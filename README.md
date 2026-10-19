# skill-launch

Launch a new skill end-to-end: create it with Draft-Skill, validate and tune it with Tune-Skill, then audit its discoverability and polish it with Findable-Polish. Use when the user has an idea for a skill and wants to go from zero to published — with triggering, validation, and discovery surfaces all handled in one pipeline.

## Usage

```text
/skill-launch "I want a skill that checks if my code is production-ready"
/skill-launch [paste list of prompts the skill should handle]
Create a skill that audits repos before deployment.
```

## Workflow

1. **Draft-Skill** creates initial skill from idea
2. **Tune-Skill** validates and fine-tunes triggering/boundaries
3. **Findable-Polish** audits discoverability and generates polished alternatives
4. Returns creation report + validation status + discovery alternatives + publication checklist

## Dependencies

Requires `draft-skill`, `tune-skill`, `findable-polish` (which needs `findable` + `wordsmith`) to be installed.

## License

MIT © Abdul Rahman P Z
