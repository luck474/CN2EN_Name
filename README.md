# CN2EN Name

一个给 Codex 使用的英文名生成 skill。

它会根据中文名、发音、风格偏好和使用场景，生成更自然、更贴切的英文名建议。

## 安装

把这个仓库克隆到 Codex 的 skills 目录：

```bash
git clone https://github.com/luck474/CN2EN_Name.git $CODEX_HOME/skills/CN2EN_Name
```

也可以直接复制本地目录：

```bash
cp -R /path/to/CN2EN_Name $CODEX_HOME/skills/CN2EN_Name
```

Codex 会从 `SKILL.md` 自动加载这个 skill。

## 调用方式

这个 skill 的触发词是：

```text
$english-name-studio
```

使用时只要在请求里带上它，再补充你的需求即可。

## 适用场景

| Skill | 指令 | 适用场景 |
| --- | --- | --- |
| English Name Studio | `$english-name-studio` | 想根据中文名、气质风格或使用场景，挑选一个自然、好用、有辨识度的英文名时使用 |

## 能做什么

这个 skill 适合用来：

- 根据中文名做发音匹配
- 根据气质或意象匹配英文名
- 生成文学感、现代感、学术感、中性风格或设计感更强的名字
- 为工作、社交、日常使用、署名或笔名场景挑选英文名

## 示例

```text
Use $english-name-studio to suggest a literary, neutral English name for a Chinese name.
```

```text
Use $english-name-studio to give me 5 modern English names that feel clean and professional.
```

```text
Use $english-name-studio to make the options closer to my Chinese pronunciation.
```

## 文件说明

- `SKILL.md`：核心规则、工作流、命名启发和输出格式
- `agents/openai.yaml`：Codex 展示名称、默认提示词和调用配置
- `references/style-directions.md`：更细的风格方向参考
