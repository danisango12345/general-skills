# general-skills

Four guardrails for working with AI on anything. Domain-agnostic — nothing here assumes a
particular kind of work.

They exist because the failure modes they prevent are quiet ones: producing something before it
was wanted, writing a file nobody asked for, claiming work is finished without checking, and
explaining something in language the reader doesn't share.

## Skills

| Skill | What it does |
|-------|--------------|
| `permission-before-writing` | Never create a file without being asked; never edit one without checking first. Applies to edits, not just new files. |
| `ask-before-producing` | Pause at the shift from gathering to producing, and confirm the person is ready. |
| `verification-before-completion` | Require evidence before claiming anything is done, correct, or confirmed. |
| `eli5` | Explain a site, screenshot or snippet in plain language, pitched at a named audience. |

## How the first three relate

They cover three different moments in the same failure:

- **`ask-before-producing`** — stops you starting before they've agreed
- **`permission-before-writing`** — stops anything reaching disk without a yes
- **`verification-before-completion`** — stops you finishing before you've checked

The middle one is the hard gate. The other two are about judgement.

## Install

Add this repo as a plugin marketplace, then install `general-skills` from it.

## Updating

1. Edit or add skills under `skills/`.
2. Bump `version` in both `.claude-plugin/plugin.json` and `.claude-plugin/marketplace.json`.
3. `git add . && git commit -m "..." && git push`.
4. Update the plugin on your side — the higher version triggers the sync.

## Versioning

Semantic versioning: `MAJOR.MINOR.PATCH`. Adding a skill is usually a MINOR bump; a small fix is a
PATCH. Any increase over the previously synced version triggers a re-pull.

## Companion

Domain-specific HR and people-operations skills live in
[hr-workbench](https://github.com/danisango12345/hr-workbench).
