# TiTi Story

`TiTi Story` is a reusable Codex skill repository for writing children's English storyboard scripts around the original puppet character `提提 (TiTi)`.

This repository is not just a single `SKILL.md` backup. It is organized as a reusable skill template repo with:

- the production skill itself
- the fixed writing standard
- installation guidance
- reuse and customization guidance
- example outputs
- maintenance notes
- source project documents used to define the standard

## What This Repository Solves

This skill exists to stop output drift in serialized children's animation writing.

Without a fixed skill, story results tend to break in predictable ways:

- template sections get omitted
- shot counts become unstable
- learning word intros disappear
- dialogue pacing changes from episode to episode
- character settings drift
- magic rules become inconsistent
- production handoff gets messy

`TiTi Story` fixes that by enforcing one stable story-writing shape.

## What The Skill Does

The skill writes scripts for a very specific workflow:

- fixed `12-shot` vertical storyboard format
- fixed `制作模版3.0` section order
- built-in `学习单词提示镜头分解`
- bilingual Chinese + English output
- child-friendly `CEFR A1` English
- fixed TiTi character lock
- fixed `愿望灯` rule system
- no background music instructions, only voice and sound effects
- funny twist ending suitable for children

## Best Use Cases

Use this skill when you need to:

- generate a new episode from a single core word such as `LIGHT`, `RAIN`, `HOME`, or `APPLE`
- keep every episode in exactly the same production format
- preserve TiTi's fixed world rules
- produce scripts that can move directly into storyboard, image generation, dubbing, and editing
- build a repeatable children's English listening series instead of one-off stories

## Quick Start

In Codex, invoke the skill like this:

```text
$titi-story
```

Example:

```text
Use $titi-story to write a new TiTi script for the core word LIGHT.
```

Installation and setup details:

- [docs/install.md](./docs/install.md)

## Repository Structure

```text
.
├── README.md
├── CHANGELOG.md
├── docs/
│   ├── example-output.md
│   ├── features.md
│   ├── install.md
│   ├── maintenance.md
│   ├── overview.md
│   ├── template-repo.md
│   └── workflow.md
├── examples/
│   ├── example-prompt.md
│   └── example-use-cases.md
├── templates/
│   └── story-brief-template.md
├── skills/
│   └── titi-story/
│       ├── SKILL.md
│       └── agents/
│           └── openai.yaml
├── TiTi_人物设定补充_愿望灯.md
├── TiTi_儿童英语动画制作SOP.md
├── 第一集_愿望灯正式脚本_会发光的小路.md
└── 第一集_愿望灯逐镜头画面提示词_会发光的小路.md
```

## Skill Output Standard

Every script produced by this skill is expected to include:

1. opening instruction line for image layout
2. fixed protagonist block
3. fixed style block
4. story summary
5. fixed character block
6. learning word intro breakdown
7. word visual treatment notes
8. main 12-shot storyboard breakdown
9. dialogue summary in Chinese
10. dialogue summary in English
11. continuous English line for smart matching

See:

- [docs/example-output.md](./docs/example-output.md)
- [examples/example-prompt.md](./examples/example-prompt.md)

## TiTi Canonical Rules

The skill assumes the canonical `提提` version already finalized in this project:

- light wooden puppet boy
- layered brown short hair
- round dark eyes
- beige shirt
- blue-green shorts
- blue-green leaf cape
- brown side bag
- small waist lantern
- night scenes use the `no hat` version

The lantern is not just a prop. It is a narrative rule system:

- formal name: `愿望灯`
- responds only to kind wishes
- only helps others
- creates small warm miracles
- gives TiTi a chance to act instead of solving everything directly

Source references:

- [TiTi_人物设定补充_愿望灯.md](./TiTi_%E4%BA%BA%E7%89%A9%E8%AE%BE%E5%AE%9A%E8%A1%A5%E5%85%85_%E6%84%BF%E6%9C%9B%E7%81%AF.md)
- [TiTi_儿童英语动画制作SOP.md](./TiTi_%E5%84%BF%E7%AB%A5%E8%8B%B1%E8%AF%AD%E5%8A%A8%E7%94%BB%E5%88%B6%E4%BD%9CSOP.md)

## If You Want To Reuse This As A Template

This repository is structured so you can clone it and adapt it to another IP or another education format.

Typical adaptation path:

1. duplicate the skill directory
2. rename the skill
3. replace the character lock
4. replace the world rules
5. replace the fixed output format
6. update the example prompts and docs

Detailed guide:

- [docs/template-repo.md](./docs/template-repo.md)

## Included Documentation

- [docs/overview.md](./docs/overview.md): project summary and intent
- [docs/features.md](./docs/features.md): what the skill controls
- [docs/workflow.md](./docs/workflow.md): production pipeline fit
- [docs/install.md](./docs/install.md): how to install and use the skill
- [docs/template-repo.md](./docs/template-repo.md): how to reuse this repo as a template
- [docs/maintenance.md](./docs/maintenance.md): how to update the skill without breaking the format

## Example Material

- [examples/example-prompt.md](./examples/example-prompt.md)
- [examples/example-use-cases.md](./examples/example-use-cases.md)
- [第一集_愿望灯正式脚本_会发光的小路.md](./%E7%AC%AC%E4%B8%80%E9%9B%86_%E6%84%BF%E6%9C%9B%E7%81%AF%E6%AD%A3%E5%BC%8F%E8%84%9A%E6%9C%AC_%E4%BC%9A%E5%8F%91%E5%85%89%E7%9A%84%E5%B0%8F%E8%B7%AF.md)

## Current Version

See [CHANGELOG.md](./CHANGELOG.md) for repository evolution and the current template baseline.
