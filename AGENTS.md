# Agent instructions

This repo holds Eidriahn's personal agent skills, shipped as one Plugin (`eidriahn`) through this repo's own Marketplace (`eidriahn-skills`). It is installed on every machine Eidriahn uses, in Claude Code and Codex. See [GLOSSARY.md](./GLOSSARY.md) for the vocabulary.

## Layout

- Every skill lives flat at `skills/<skill-name>/SKILL.md`. No category folders: the Plugin discovers skills one level deep, so anything nested is silently not shipped.
- Every skill folder under `skills/` ships. To keep a skill out of the Plugin, keep it outside `skills/`.
- The folder name is the skill name, in kebab-case, and must match the `name` in the `SKILL.md` frontmatter. Users invoke it as `/eidriahn:<skill-name>`.

## Manifests

- `.claude-plugin/plugin.json` defines the Plugin. `.claude-plugin/marketplace.json` defines the Marketplace. Codex reads the same Marketplace file.
- Never add a `version` field to `plugin.json`. Without it, every push to `main` counts as a new release, which is how installed machines pick up changes.
- Run `claude plugin validate .` after touching either manifest or adding a skill.

## README

When you add, rename, or remove a skill, update the skills list in `README.md`.
