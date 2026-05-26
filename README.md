# CN2EN Name

`CN2EN Name` is a Codex skill for generating thoughtful English names from a Chinese name, pronunciation, personal vibe, and usage context.

它不是随便“翻译”一个英文名，而是尽量在以下几件事之间取得平衡：

- 保留中文名的发音、气质或意象
- 让名字在真实英语语境里自然、好读、好记
- 根据使用场景给出更文学、更现代、更中性或更职业的选择

## What This Skill Does

This skill helps users:

- generate 3 to 5 ranked English name options
- match a Chinese name by sound, mood, or imagery
- refine results toward a more literary, modern, scholarly, neutral, or design-forward direction
- choose a final name for daily use, work, social media, signature, or pen-name contexts

## Core Features

- Ranked shortlist instead of a flat dump of names
- One-line rationale for every candidate
- Style-aware refinement
- Neutral by default unless gender expression is specified
- Real-world usability over novelty spellings

## Repository Structure

```text
.
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    └── style-directions.md
```

## Files

### `SKILL.md`

Defines the main behavior of the skill, including:

- required user inputs
- naming heuristics
- refinement rules
- output format
- example requests

### `agents/openai.yaml`

Provides the Codex UI metadata:

- display name
- short description
- default prompt
- implicit invocation policy

### `references/style-directions.md`

Used when the user wants tighter stylistic iteration, such as:

- more literary
- more modern
- more scholarly
- more design-forward
- closer to the original Chinese name

## How It Works

The skill follows a simple workflow:

1. Collect the minimum inputs.
2. Decide what to preserve from the Chinese name.
3. Generate a compact ranked shortlist.
4. Explain why each name fits.
5. Recommend one strongest option and a few alternates.

By default, it optimizes for names that feel intentional and natural, not quirky or overly invented.

## Input Dimensions

The skill is best when the user provides some of the following:

- Chinese name or pronunciation
- desired vibe
- gender expression
- usage context

Example vibes:

- literary
- modern
- scholarly
- soft classic
- rare but natural
- design-forward

## Example Prompts

```text
Use $english-name-studio to suggest a literary, neutral English name for 夏一凡.
```

```text
Use $english-name-studio to give me 5 modern English names for 林然 that feel clean and professional.
```

```text
Use $english-name-studio to make the options closer to my Chinese pronunciation but still natural in English.
```

```text
Use $english-name-studio to recommend one final English name for work and two more expressive alternatives.
```

## Example Output Style

```text
1. Rowan
   Quiet literary, balanced, and easy to use internationally.

2. Ellis
   Clean and thoughtful, with a restrained modern feel.

3. Arden
   Slightly more distinctive, with a calm and design-forward texture.
```

## Design Principles

This skill prefers:

- subtlety over gimmicks
- names in real usage over fabricated names
- readability over decorative spelling
- preserving either sound, mood, or imagery instead of forcing all three

It avoids:

- stereotype-heavy choices
- awkward transliterations
- names that feel too theatrical unless explicitly requested

## Installation

Place this folder in your Codex skills directory so the `SKILL.md` file can be discovered by Codex.

Typical layout:

```text
$CODEX_HOME/skills/CN2EN_Name/
```

If you are organizing skills manually, make sure these files stay together:

- `SKILL.md`
- `agents/openai.yaml`
- `references/style-directions.md`

## Best Use Cases

- Chinese users choosing a first English name
- writers or designers looking for a name with a specific aesthetic
- people refining an existing English name to feel more natural
- professionals who want a name that works well in email, resumes, and introductions

## Customization Ideas

You can extend the skill by adding:

- more style references
- region-specific naming preferences
- workplace-safe vs creative-mode output paths
- stricter phonetic matching rules
- optional surname pairing suggestions

## License

Add a license file if you want to make reuse terms explicit.
