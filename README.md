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

## 中文说明

`CN2EN Name` 是一个给 Codex 使用的英文名生成 skill。

它会根据中文名、发音、风格偏好和使用场景，生成更自然、更有气质的英文名建议。

## 中文安装

把这个仓库克隆到 Codex 的 skills 目录：

```bash
git clone https://github.com/luck474/CN2EN_Name.git $CODEX_HOME/skills/CN2EN_Name
```

或者直接复制本地目录：

```bash
cp -R /path/to/CN2EN_Name $CODEX_HOME/skills/CN2EN_Name
```

Codex 会从 `SKILL.md` 自动加载这个 skill。

## 中文用法

这个 skill 的触发词是：

```text
$english-name-studio
```

使用时只要在请求里带上它，再补充你的需求即可。

示例：

```text
Use $english-name-studio to suggest a literary, neutral English name for a Chinese name.
```

```text
Use $english-name-studio to give me 5 modern English names that feel clean and professional.
```

```text
Use $english-name-studio to make the options closer to my Chinese pronunciation.
```

## 中文功能

这个 skill 适合用来：

- 根据中文名做发音匹配
- 根据气质或意象匹配英文名
- 生成文学感、现代感、学术感、中性风格或设计感更强的名字
- 为工作、社交、日常使用、署名或笔名场景挑选英文名

## 中文文件说明

- `SKILL.md`：核心规则、工作流、命名启发和输出格式
- `agents/openai.yaml`：Codex 展示名称、默认提示词和调用配置
- `references/style-directions.md`：更细的风格方向参考
