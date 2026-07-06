# TiTi Story

中文说明在前，英文说明在后。  
Chinese section first, English section below.

---

## 中文说明

`TiTi Story` 是一个可复用的 Codex skill 仓库，用来围绕原创角色 `提提 (TiTi)` 产出固定格式的儿童英语动画故事脚本。

这个仓库不是单独备份一个 `SKILL.md`，而是一个完整的 skill 模板仓库，包含：

- 正式 skill 文件
- 固定写作标准
- 安装说明
- 模板复用说明
- 示例 prompt
- 维护规范
- 角色与项目源设定文档

### 这个仓库解决什么问题

在系列化儿童内容生产里，如果没有固定 skill，结果通常会漂：

- 模板段落漏掉
- 分镜数量不稳定
- 学习单词提示镜头被省略
- 台词节奏每集不一致
- 角色设定越写越偏
- 魔法规则越写越乱
- 后续出图、配音、剪辑衔接成本升高

这个仓库的目的，就是把这些容易漂的部分固定下来。

### Skill 的核心能力

这个 skill 专门服务于一条明确的生产链路：

`核心词 -> 脚本 -> 分镜 -> 画面提示词 -> 配音 -> 剪辑`

固定能力包括：

- 固定 `12 镜头` 正片分镜
- 固定 `9:16` 竖构图设定
- 固定 `制作模版3.0` 输出结构
- 固定 `学习单词提示镜头分解`
- 中英双语脚本输出
- 面向儿童启蒙的 `CEFR A1` 英文难度
- 固定主角 `提提`
- 固定 `愿望灯` 规则
- 固定“不要背景音乐，只保留人声和特效音效”
- 固定“结尾要有轻松搞笑反转”

### 适用场景

适合用于：

- 围绕单个核心词生成一集新故事
- 保持每一集输出结构完全一致
- 做系列化儿童英语磨耳朵内容
- 直接给后续分镜、出图、配音、剪辑使用
- 把提提世界观和角色规则稳定下来

### 快速使用

在 Codex 中调用：

```text
$titi-story
```

示例：

```text
Use $titi-story to write a new TiTi script for the core word LIGHT.
```

安装说明：

- [docs/install.md](./docs/install.md)

### 仓库结构

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

### 输出标准

这个 skill 产出的每份故事脚本，默认都应包含：

1. 开头总说明行
2. 主人公固定说明
3. 风格说明
4. 情节概要
5. 角色固定说明
6. 学习单词提示镜头分解
7. 文字表现建议
8. 12 镜头正片分镜
9. 台词总汇
10. 中文版
11. 英文版
12. 智能文稿匹配（英文）

参考：

- [docs/example-output.md](./docs/example-output.md)
- [examples/example-prompt.md](./examples/example-prompt.md)

### 提提固定设定

当前 skill 默认绑定以下角色规则：

- 主角是 `提提 (TiTi)`
- 木质感小男孩木偶
- 棕色层次短发
- 圆润深色眼睛
- 米色上衣
- 蓝绿色短裤
- 蓝绿色叶片斗篷
- 棕色斜挎小包
- 腰间挂小提灯
- 夜晚默认使用 `不戴帽版`

### 愿望灯规则

`愿望灯` 是提提的核心叙事道具，不只是普通提灯。

固定规则：

- 只响应善良愿望
- 只用于帮助别人
- 只能实现温暖的小奇迹
- 不直接替提提解决一切
- 重点是让提提获得行动机会

源文档参考：

- [TiTi_人物设定补充_愿望灯.md](./TiTi_%E4%BA%BA%E7%89%A9%E8%AE%BE%E5%AE%9A%E8%A1%A5%E5%85%85_%E6%84%BF%E6%9C%9B%E7%81%AF.md)
- [TiTi_儿童英语动画制作SOP.md](./TiTi_%E5%84%BF%E7%AB%A5%E8%8B%B1%E8%AF%AD%E5%8A%A8%E7%94%BB%E5%88%B6%E4%BD%9CSOP.md)

### 如果你要把它当模板复用

这个仓库已经按模板仓库方式组织好了。  
后面如果你要做新的儿童故事 skill，通常只需要替换：

1. skill 名称
2. 角色锁定规则
3. 世界观规则
4. 示例 prompt
5. 相关说明文档

详细说明：

- [docs/template-repo.md](./docs/template-repo.md)

### 文档索引

- [docs/overview.md](./docs/overview.md)：项目定位
- [docs/features.md](./docs/features.md)：功能与约束
- [docs/workflow.md](./docs/workflow.md)：生产流程
- [docs/install.md](./docs/install.md)：安装说明
- [docs/template-repo.md](./docs/template-repo.md)：模板复用说明
- [docs/maintenance.md](./docs/maintenance.md)：维护规范

### 示例材料

- [examples/example-prompt.md](./examples/example-prompt.md)
- [examples/example-use-cases.md](./examples/example-use-cases.md)
- [第一集_愿望灯正式脚本_会发光的小路.md](./%E7%AC%AC%E4%B8%80%E9%9B%86_%E6%84%BF%E6%9C%9B%E7%81%AF%E6%AD%A3%E5%BC%8F%E8%84%9A%E6%9C%AC_%E4%BC%9A%E5%8F%91%E5%85%89%E7%9A%84%E5%B0%8F%E8%B7%AF.md)

### 当前版本

版本记录见：

- [CHANGELOG.md](./CHANGELOG.md)

---

## English

`TiTi Story` is a reusable Codex skill repository for generating fixed-format children's English animation story scripts around the original character `提提 (TiTi)`.

This repository is not just a backup of one `SKILL.md`. It is organized as a complete reusable skill template repository with:

- the production skill itself
- the fixed writing standard
- installation guidance
- template reuse guidance
- example prompts
- maintenance rules
- source documents for character and project constraints

### What This Repository Solves

In serialized children's content production, outputs drift quickly if the skill rules are not fixed:

- sections get omitted
- shot counts change
- word-learning intro blocks disappear
- dialogue pacing becomes inconsistent
- character rules drift
- magic rules become unstable
- downstream image, dubbing, and editing work becomes harder

This repository exists to lock those unstable parts down.

### Core Skill Capability

The skill is designed for one clear production chain:

`core word -> script -> storyboard -> image prompts -> dubbing -> editing`

The fixed capabilities include:

- fixed `12-shot` main storyboard
- fixed `9:16` vertical composition
- fixed `制作模版3.0` output structure
- fixed `学习单词提示镜头分解`
- bilingual Chinese + English script output
- `CEFR A1` level English for young children
- fixed TiTi protagonist rules
- fixed `Wish Lantern` rules
- fixed `no background music, voice and sound effects only`
- fixed light funny twist ending

### Best Use Cases

Use this repository when you want to:

- generate a new episode from one core word
- keep every episode in the exact same production structure
- build a serialized children's English listening series
- hand scripts directly into storyboard, image generation, dubbing, and edit workflows
- preserve TiTi's world and rule consistency

### Quick Start

Invoke the skill in Codex with:

```text
$titi-story
```

Example:

```text
Use $titi-story to write a new TiTi script for the core word LIGHT.
```

Install guide:

- [docs/install.md](./docs/install.md)

### Repository Structure

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

### Output Standard

Each generated story script is expected to include:

1. opening instruction line
2. fixed protagonist block
3. style block
4. story summary
5. fixed character block
6. word-learning intro breakdown
7. word visual treatment notes
8. 12-shot main storyboard
9. dialogue summary
10. Chinese version
11. English version
12. smart English matching line

References:

- [docs/example-output.md](./docs/example-output.md)
- [examples/example-prompt.md](./examples/example-prompt.md)

### TiTi Canonical Rules

The current skill is tied to the following character rules:

- protagonist: `TiTi`
- wooden puppet boy
- layered brown short hair
- round dark eyes
- beige shirt
- blue-green shorts
- blue-green leaf cape
- brown side bag
- small waist lantern
- night scenes default to the `no-hat` version

### Wish Lantern Rules

The `Wish Lantern` is TiTi's core narrative prop, not just a normal lamp.

Fixed rules:

- responds only to kind wishes
- can only be used to help others
- creates only small warm miracles
- does not solve everything for TiTi
- mainly creates a chance for TiTi to act

Source references:

- [TiTi_人物设定补充_愿望灯.md](./TiTi_%E4%BA%BA%E7%89%A9%E8%AE%BE%E5%AE%9A%E8%A1%A5%E5%85%85_%E6%84%BF%E6%9C%9B%E7%81%AF.md)
- [TiTi_儿童英语动画制作SOP.md](./TiTi_%E5%84%BF%E7%AB%A5%E8%8B%B1%E8%AF%AD%E5%8A%A8%E7%94%BB%E5%88%B6%E4%BD%9CSOP.md)

### Reusing This Repository As A Template

This repository is already organized as a template repo.  
If you want to build a new children's story skill from it, you usually only need to replace:

1. the skill name
2. the character lock rules
3. the world rules
4. the example prompts
5. the related docs

Detailed guide:

- [docs/template-repo.md](./docs/template-repo.md)

### Documentation Index

- [docs/overview.md](./docs/overview.md): project overview
- [docs/features.md](./docs/features.md): features and constraints
- [docs/workflow.md](./docs/workflow.md): production workflow
- [docs/install.md](./docs/install.md): installation guide
- [docs/template-repo.md](./docs/template-repo.md): template reuse guide
- [docs/maintenance.md](./docs/maintenance.md): maintenance guidance

### Example Materials

- [examples/example-prompt.md](./examples/example-prompt.md)
- [examples/example-use-cases.md](./examples/example-use-cases.md)
- [第一集_愿望灯正式脚本_会发光的小路.md](./%E7%AC%AC%E4%B8%80%E9%9B%86_%E6%84%BF%E6%9C%9B%E7%81%AF%E6%AD%A3%E5%BC%8F%E8%84%9A%E6%9C%AC_%E4%BC%9A%E5%8F%91%E5%85%89%E7%9A%84%E5%B0%8F%E8%B7%AF.md)

### Current Version

Version history:

- [CHANGELOG.md](./CHANGELOG.md)
