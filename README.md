# Co-Aligned Skills

Skills for maintaining the [Co-Aligned](https://github.com/forwardimpact/monorepo/blob/main/COALIGNED.md) instruction architecture with the `coaligned` CLI.

## Install

With [APM](https://microsoft.github.io/apm/):

```bash
apm install forwardimpact/coaligned-skills
```

## Available Skills

| Skill | Description |
| --- | --- |
| **coaligned-audit** | Run the full Co-Aligned check suite and act on what it finds. Use for a periodic co-alignment health check, when CI reports a `coaligned` failure, or before a release — to triage every finding and route it to the fix that owns it. |
| **coaligned-invariant** | Author a declarative invariant rule module for `coaligned invariants`. Use when a repository needs to enforce its own architectural rule — a forbidden import, a value that must agree across files, a directory shape — as a `.coaligned/invariants/*.rules.mjs` module the CLI discovers and runs. |
| **coaligned-jtbd** | Author and maintain Jobs To Be Done entries for the Co-Aligned standard. Use when writing a Big Hire or Little Hire, when adding a `<job>` tag, when `package.json .jobs` blocks are stale, or when `coaligned jtbd` reports a schema or freshness failure. |
| **coaligned-layer** | Author or repair an instruction layer to the Co-Aligned standard — an agent profile, agent reference, SKILL.md, skill reference, or checklist. Use when adding an agent or skill, when `coaligned instructions` flags a length breach, or when one layer has started restating another. |
| **coaligned-setup** | Bootstrap the Co-Aligned instruction architecture in a repository. Use when a repo has no layered agent instructions yet, when adopting the Co-Aligned standard, or when wiring the `coaligned` checks into the repository so instruction layers, jobs, and invariants stay enforced. |
