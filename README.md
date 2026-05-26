# CN2EN Name

English name generation skill for Codex.

Suggests thoughtful English names based on a Chinese name, pronunciation, aesthetic preference, and usage context.

## Installation

Clone this repo into your Codex skills directory:

```bash
git clone https://github.com/luck474/CN2EN_Name.git $CODEX_HOME/skills/CN2EN_Name
```

That's it. Codex will load the skill from `SKILL.md`.

Alternative: install from a local folder

```bash
cp -R /path/to/CN2EN_Name $CODEX_HOME/skills/CN2EN_Name
```

## Skill

| Skill | Command | When to use |
| --- | --- | --- |
| English Name Studio | `$english-name-studio` | Choosing an English name that feels natural, distinctive, and aligned with a Chinese name, vibe, or context |

## What It Does

The skill helps with:

- sound-based matching
- mood-based matching
- image-based matching
- literary, modern, scholarly, neutral, or design-forward directions
- daily-use, work, social, signature, or pen-name contexts

## Example

```text
Use $english-name-studio to suggest a literary, neutral English name for my Chinese name.
```

```text
Use $english-name-studio to make the options more modern and closer to my pronunciation.
```

## Files

- `SKILL.md` defines the core workflow, heuristics, and output format
- `agents/openai.yaml` defines display metadata and default invocation behavior
- `references/style-directions.md` provides tighter style directions for refinement
