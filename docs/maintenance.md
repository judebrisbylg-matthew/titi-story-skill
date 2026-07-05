# Maintenance

This repository is stable only if the skill rules and the production template stay aligned.

## Safe Update Areas

You can safely update these without changing the repo’s identity:

- README wording
- examples
- story samples
- explanatory docs
- example prompts

## High-Risk Update Areas

Change these carefully because they affect production consistency:

- `skills/titi-story/SKILL.md`
- the fixed section order
- the learning intro block
- shot count
- dialogue summary shape
- character lock rules
- `愿望灯` constraints

## Before Changing The Skill

Ask:

1. is this a real workflow change or just a one-off story preference?
2. does this belong in the permanent skill or only in one episode prompt?
3. will this break old examples or new episodes?

If the change is one-off, keep it out of the skill and place it in the user prompt instead.

## Regression Checklist

After any skill update, test with one known prompt and verify:

- `学习单词提示镜头分解` still appears
- `文字表现建议` still appears
- `正片镜头分解` still appears
- there are exactly `12` main shots
- the story uses only `1` core word
- duration target is still `60-90 seconds`
- there is still no background music
- the ending is still a child-friendly funny twist

## Recommended Test Prompt

```text
Use $titi-story to write a new TiTi story for the core word LIGHT.
```

## Versioning Guidance

Use simple semantic intent for repo versions:

- patch: doc clarifications, examples, wording improvements
- minor: new supporting docs, templates, examples, non-breaking rule clarifications
- major: output format changes, structure changes, command changes, or story-rule changes that alter expected downstream production
