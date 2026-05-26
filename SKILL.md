---
name: english-name-studio
description: Generate distinctive English names based on a person's Chinese name, pronunciation, aesthetic preferences, and gender expression. Use when the user wants an English name that feels literary, modern, neutral, professional, memorable, or culturally natural; when they want ranked name options with rationale; or when they want to refine names for social, creative, or work contexts.
---

# English Name Studio

Help the user choose an English name that feels intentional rather than random.

## Workflow

1. Gather the minimum inputs:
- Chinese name or pronunciation
- Desired vibe, such as literary, modern, restrained, elegant, bold, scholarly, or creative
- Gender expression: neutral by default unless the user specifies otherwise
- Usage context if relevant: daily use, work, social profile, signature, pen name

2. Decide what should be preserved:
- Sound echo from the original name
- Semantic imagery or mood from the original name
- Social ease: easy to spell, easy to pronounce, culturally natural

3. Produce a compact shortlist:
- Default to 5 names
- Expand to 10 only if the user asks for more breadth
- Rank the options instead of presenting them as a flat list

4. For each candidate, include:
- The name
- A one-line reason it fits
- A short vibe label, such as "quiet literary" or "modern scholar"

5. Finish with a recommendation:
- Name the strongest overall option
- If useful, include 2 alternates for different moods

## Naming Heuristics

- Prefer names that exist in real usage and do not feel invented unless the user explicitly wants something unusual.
- Keep spelling readable. A distinctive name should still be easy to use in real life.
- Default to subtlety over gimmicks.
- For Chinese names, preserve either sound, mood, or imagery. Do not force all three if the result feels unnatural.
- Avoid stereotypes, novelty spellings, and names that sound like characters unless the user wants a theatrical effect.
- For neutral names, favor names that feel balanced rather than aggressively masculine or feminine.
- For literary naming, prefer restraint, atmosphere, and clarity over ornate symbolism.
- For modern naming, prefer clean, current, internationally legible names over dated classics.

## Style Directions

Use these style anchors when the user gives a broad aesthetic:

- `literary`: quiet, reflective, textured, bookish
- `modern`: clean, concise, current, globally usable
- `scholarly`: composed, intelligent, restrained, slightly austere
- `design-forward`: elegant, minimal, tasteful, memorable
- `soft classic`: timeless, warm, polished, unobtrusive
- `rare but natural`: distinctive without sounding fabricated

If the user wants finer distinctions, read [references/style-directions.md](references/style-directions.md).

## Refinement Rules

- If the user says "more literary," shift toward names with poetic or essayistic texture.
- If the user says "more modern," simplify the shape and increase everyday usability.
- If the user says "more neutral," remove names with strong gender coding.
- If the user says "closer to my Chinese name," increase phonetic similarity without becoming awkward.
- If the user says "more character," keep the name readable but allow slightly rarer choices.

Refine along one axis at a time so the differences stay legible.

## Output Patterns

Choose the lightest format that fits the request.

For quick suggestions:
- Give 3 to 5 ranked names with one-line rationale.

For comparison requests:
- Group names into 2 or 3 clusters, such as safer, more literary, and more distinctive.

For final selection:
- Recommend one primary name and show how it looks in use, such as `Rowan Lin`.

## Example Requests

- "Use $english-name-studio to suggest a literary, neutral English name for a Chinese name."
- "Use $english-name-studio to make the options more modern and less delicate."
- "Use $english-name-studio to give me 5 English names that fit a designer-writer vibe."
