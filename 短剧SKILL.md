# shuohao-extension-skills

两套相互隔离的真人短剧创作 Skill：

- `skill-western`：欧美真人短剧全题材创作。
- `skill-live`：国内真人短剧全题材创作。

每个目录都是独立 Skill Bundle，包含一个 `SKILL.md`、基础提示词和两份输出模板。不得在一个项目中混用两套 Skill 的摄影机、场景库、调色、禁用词或人物审美词汇。

## 使用

安装或扫描仓库后，明确指定一个 Skill：`@shuohao-western` 或 `@shuohao-live`。若客户端采用 Codex 的技能选择语法，则使用 `$shuohao-western` 或 `$shuohao-live`。一次请求只指定一个；需要双版本改编时，分两次独立调用。

## 风格隔离约定

1. 先锁定 `skill_id`，全程只读取该目录内的文件。
2. 不继承另一 Skill 的默认摄影机、色彩、场景、禁用词和模板字段。
3. 每个视觉提示词都要写入本 Skill 的风格锚点和排除词；不得用“同上”代替。
4. 发现用户给出的参考与当前 Skill 冲突时，先说明冲突并以当前 Skill 的风格合同为准，或要求用户切换 Skill。

## 目录

```text
skill-live/       国内真人短剧
skill-western/    欧美真人短剧
```

本仓库不绑定特定生成模型。Seedance 2.5 提示词是可直接复制的镜头级文本；具体参数以调用环境实际支持项为准。
