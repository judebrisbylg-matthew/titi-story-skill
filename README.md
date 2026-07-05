# TiTi Story

`TiTi Story` is a Codex skill for writing children's English storyboard scripts for the original character `提提 (TiTi)`.

It is designed for a very specific production workflow:

- fixed `12-shot` vertical storyboard format
- fixed `制作模版3.0` output structure
- built-in `word learning intro sequence`
- bilingual Chinese + English script output
- child-friendly `CEFR A1` English
- `愿望灯` magic system built into story logic
- no background music instructions, only voice and sound effects

This repository packages the skill itself plus documentation that explains what it does, how to use it, and how it fits into a repeatable children’s animation workflow.

## Repository Structure

```text
.
├── README.md
├── docs/
│   ├── overview.md
│   ├── features.md
│   ├── workflow.md
│   └── example-output.md
└── skills/
    └── titi-story/
        ├── SKILL.md
        └── agents/
            └── openai.yaml
```

## What This Skill Is For

Use this skill when you need to write new `TiTi` stories in one stable output format for children’s animation production.

It is especially useful for:

- generating a new episode from a core word such as `LIGHT`, `APPLE`, `RAIN`, or `HOME`
- keeping every output in the exact same production template
- preserving the same character rules for `提提`
- preserving the same `愿望灯` logic
- producing scripts that can move directly into storyboard, image generation, dubbing, and editing

## Output Standard

Every script produced by this skill is expected to include:

1. opening instruction line for the image layout
2. fixed protagonist block
3. fixed style block
4. story summary
5. fixed character block
6. learning word intro breakdown
7. word visual treatment notes
8. main 12-shot storyboard breakdown
9. dialogue summary in Chinese
10. dialogue summary in English
11. continuous English line for smart text matching

## Character Standard

The skill assumes the canonical `提提` version already finalized by the user:

- light wooden puppet boy
- layered brown short hair
- round dark eyes
- beige shirt
- blue-green shorts
- blue-green leaf cape
- brown side bag
- small waist lantern
- night scenes use the `no hat` version

## Wish Lantern Standard

The lantern is not just a prop. It is a magic rule system:

- its formal name is `愿望灯`
- it responds only to kind wishes
- it is only used to help others
- it creates small warm miracles, not unlimited power
- it gives TiTi a chance to act instead of solving everything on its own

## Usage

In Codex, invoke the skill like this:

```text
$titi-story
```

Example prompt:

```text
Use $titi-story to write a new TiTi script for the core word LIGHT.
```

## Why This Skill Exists

Without a skill, story output tends to drift:

- section order changes
- learning intro blocks are omitted
- shot counts change
- dialogue pacing changes
- TiTi’s character rules drift
- the lantern loses narrative consistency

This skill fixes that by enforcing one stable production shape.

## Included Documentation

- [docs/overview.md](./docs/overview.md): high-level summary of the skill
- [docs/features.md](./docs/features.md): what the skill guarantees and controls
- [docs/workflow.md](./docs/workflow.md): how the output fits into a full production workflow
- [docs/example-output.md](./docs/example-output.md): example of the expected script format

