# Jidoka Skills

Skills for maintaining the [Jidoka](https://github.com/forwardimpact/monorepo/blob/main/JIDOKA.md) instruction architecture with the `jidoka` CLI (installed via `npx @forwardimpact/jidoka` or the platform bootstrap). Renamed from `coaligned-skills` — migrate with `git mv .coaligned .jidoka`, reinstall this pack, and swap the CLI name.

## Install

With [APM](https://microsoft.github.io/apm/):

```bash
apm install forwardimpact/jidoka-skills
```

## Available Skills

| Skill | Description |
| --- | --- |
| **jidoka-audit** | Run the full Jidoka check suite and act on what it finds. Use for a periodic instruction-quality health check, when CI reports a `jidoka` failure, or before a release — to triage every finding and route it to the fix that owns it. |
| **jidoka-invariant** | Author a declarative invariant rule module for `jidoka invariants`. Use when a repository needs to enforce its own architectural rule — a forbidden import, a value that must agree across files, a directory shape — as a `.jidoka/invariants/*.rules.mjs` module the CLI discovers and runs. |
| **jidoka-jtbd** | Author and maintain Jobs To Be Done entries for the Jidoka standard. Use when writing a Big Hire or Little Hire, when adding a `<job>` tag, when `package.json .jobs` blocks are stale, or when `jidoka jtbd` reports a schema or freshness failure. |
| **jidoka-layer** | Author or repair an instruction layer to the Jidoka standard — an agent profile, agent reference, SKILL.md, skill reference, or checklist. Use when adding an agent or skill, when `jidoka instructions` flags a length breach, or when one layer has started restating another. |
| **jidoka-setup** | Bootstrap the Jidoka instruction architecture in a repository. Use when a repo has no layered agent instructions yet, when adopting the Jidoka standard, or when wiring the `jidoka` checks into the repository so the line stops the moment a layer drifts, a job goes stale, or an invariant breaks. |
