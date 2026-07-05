# Install

This repository contains a Codex skill in:

`skills/titi-story/`

## Install Into Local Codex Skills

Copy the skill folder into your local Codex skills directory:

```bash
cp -R skills/titi-story ~/.codex/skills/
```

If a previous version already exists, replace it intentionally:

```bash
rm -rf ~/.codex/skills/titi-story
cp -R skills/titi-story ~/.codex/skills/
```

## Validate The Skill

If your local Codex environment includes the bundled validator used during creation, validate it with:

```bash
python3 ~/.codex/skills/.system/skill-creator/scripts/quick_validate.py ~/.codex/skills/titi-story
```

Expected result:

```text
Skill is valid!
```

## Invoke The Skill

Use the skill in Codex with:

```text
$titi-story
```

Example prompt:

```text
Use $titi-story to write a new TiTi story for the core word LIGHT.
```

## What To Check After Installing

- the skill name resolves as `titi-story`
- the output contains `学习单词提示镜头分解`
- the main storyboard contains exactly `12` shots
- the output keeps the `制作模版3.0` section order
- the ending includes a light funny twist
- no background music is introduced

## Upgrade Path

When this repository changes:

1. pull the newest repo version
2. replace the local `~/.codex/skills/titi-story` directory
3. re-run validation
4. test with a known core word such as `LIGHT`
