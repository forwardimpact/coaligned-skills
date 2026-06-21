# Co-Aligned Skills

Skills for maintaining the [Co-Aligned](https://github.com/forwardimpact/monorepo/blob/main/COALIGNED.md) instruction architecture with the `coaligned` CLI.

## Install

With [APM](https://microsoft.github.io/apm/):

```bash
apm install forwardimpact/coaligned-skills
```

With [npx skills](https://github.com/vercel-labs/skills):

```bash
npx skills add forwardimpact/coaligned-skills
```

## Available Skills

| Skill | Description |
| --- | --- |
| **coaligned-audit** | Run the full Co-Aligned check suite and act on what it finds. Use for a periodic co-alignment health check, when CI reports a `coaligned` failure, or before a release — to triage every finding and route it to the fix that owns it. |
| **coaligned-invariant** | Author a declarative invariant rule module for `npx coaligned invariants`. Use when a repository needs to enforce its own architectural rule — a forbidden import, a value that must agree across files, a directory shape — as a `.coaligned/invariants/*.rules.mjs` module the CLI discovers and runs. |
| **coaligned-jtbd** | Author and maintain Jobs To Be Done entries for the Co-Aligned standard. Use when writing a Big Hire or Little Hire, when adding a `<job>` tag, when `package.json .jobs` blocks are stale, or when `npx coaligned jtbd` reports a schema or freshness failure. |
| **coaligned-layer** | Author or repair an instruction layer to the Co-Aligned standard — an agent profile, agent reference, SKILL.md, skill reference, or checklist. Use when adding an agent or skill, when `npx coaligned instructions` flags a length breach, or when one layer has started restating another. |
| **coaligned-setup** | Bootstrap the Co-Aligned instruction architecture in a repository. Use when a repo has no layered agent instructions yet, when adopting the COALIGNED.md standard, or when wiring `npx coaligned` into the checks so instruction layers, jobs, and invariants stay enforced. |
