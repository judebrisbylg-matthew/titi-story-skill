---
name: titi-story
description: Write TiTi children's English story scripts in the fixed 制作模版3.0 format. Use when the user wants a new TiTi story, storyboard script, bilingual children's script, 12-shot vertical storyboard, word-learning intro sequence, or asks to keep the exact TiTi template format with 学习单词提示镜头分解, 正片镜头分解, 台词总汇, and 智能文稿匹配（英文）.
---

# TiTi Story

Use this skill to produce new `提提 TiTi` story scripts in the exact fixed format the user standardized on with `制作模版3.0.docx`.

## Core Rules

Always keep these fixed unless the user explicitly changes them:

- Output `12` main storyboard shots
- Every shot is `vertical 9:16`
- Include `学习单词提示镜头分解`
- Include `文字表现建议`
- Include `正片镜头分解 (Scene Breakdown)`
- Include `台词总汇 (Dialogue Summary)`
- Include `智能文稿匹配（英文）`
- Do not omit sections

## Character Lock

Treat these as canonical:

- Main character: `提提 (TiTi)`
- Night scenes use `不戴帽版`
- TiTi is a light-wood puppet boy with layered brown short hair, round dark eyes, gentle expression
- Costume: beige shirt, blue-green shorts, blue-green leaf cape, brown side bag
- Prop: small waist lantern
- The lantern is `愿望灯`

## Wish Lantern Rules

When the lantern appears in story logic:

- It responds only to kind wishes
- It is used to help others
- It creates small warm miracles, not unlimited power
- It gives TiTi a chance to act; it does not solve everything by itself
- Its glow should feel gentle, warm, and safe

## Story Rules

Always follow these unless the user overrides them:

- Target audience: children age roughly 3-6
- English level: `CEFR A1`
- Keep sentences short and speakable
- Use exactly `1` core word per story
- Keep `1-2` core sentence patterns
- Story duration target: `60-90 seconds`
- No background music; use only voice and sound effects
- End with a gentle funny twist

## Required Output Format

Output in this exact section order:

1. Opening instruction line:
   `请结合图1的主体形象，主人公（固定不变），画面中不能出现文字，输出12宫格的分镜，每一个分镜的都是竖构图（9:16）。`
2. `主人公（固定不变）：`
3. `风格：`
4. `情节概要：`
5. `角色 (Characters)（固定不变）`
6. Separator line:
   `--------------------------------------------------------------------------------------------------`
7. `学习单词提示镜头分解`
8. `文字表现建议`
9. Separator line:
   `--------------------------------------------------------------------------------------------------`
10. `正片镜头分解 (Scene Breakdown)（镜头的内容要以表格的形式呈现）`
11. `台词总汇 (Dialogue Summary)`
12. Separator line:
   `--------------------------------------------------------------------------------------------------`
13. `中文版 (Chinese Version)`
14. `英文版 (English Version)`
15. `智能文稿匹配（英文）：`

## Learning Intro Block

Always include an 8-second learning intro before the main story.

Use this structure:

- `时间	画面与动作	台词与字幕`
- 0.0–1.0秒
- 1.0–3.3秒
- 3.3–4.5秒
- 4.5–6.0秒
- 6.0–6.8秒
- 6.8–8.0秒

Customize the Chinese and English word display to the current core word.

Keep these constraints:

- TiTi appears like a small teacher
- The word is spoken in Chinese first, then English
- The frame fades to full black at the end
- Keep the final black frame around 0.5 seconds

## Main Storyboard Block

For the `正片镜头分解` section:

- Write `12` shots
- Each shot must have:
  - shot title line like `镜头 1：... (对应图1)`
  - table header line `镜号	景别	画面	台词	时长`
  - one row of content
- Keep durations around `5-8s`
- Use dialogue with `（语速是0.8倍速）` when spoken
- Use `(不要背景音乐，只要求有人声和特效音效)` where appropriate
- If a shot has no spoken dialogue, use sound effect notes only

## Dialogue Summary Rules

At the end:

- List Chinese dialogue lines only under `中文版 (Chinese Version)`
- List English dialogue lines only under `英文版 (English Version)`
- Then produce one continuous English line under `智能文稿匹配（英文）：`

## Writing Style

- Write in Chinese with embedded English lines
- Keep the tone warm, clear, visual, and child-friendly
- Make each shot easy to picture
- Avoid dense explanation outside the fixed template
- Do not add extra sections unless the user explicitly asks

## Fast Checklist

Before finishing, verify:

- The template matches `制作模版3.0`
- `学习单词提示镜头分解` is present
- The story uses `12` shots
- Core word count is `1`
- Vertical `9:16` is mentioned in the opening line
- No background music instruction is preserved
- The ending has a funny twist
