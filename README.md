# Cinematic Realism Image Prompt Skill

一个用于把简短画面想法扩展为**真实摄影感、电影级构图、专业镜头、物理光影和低 AI 感**图像提示词的 Agent Skill。

适合：

- 人物、古代人物与中式审美；
- 老虎、狼、鹿等野生动物；
- 异兽、奇幻生物与荒诞现实；
- 纯风景、建筑、雨夜与水中动作；
- 优化已有提示词；
- 修复 AI 味、油画感、塑料感、CG 感、假景深和无来源光效。

## 仓库结构

```text
cinematic-realism-image-prompt-skill/
├── README.md
├── LICENSE
├── EVALS.md
├── CHANGELOG.md
└── .github/
    └── skills/
        └── cinematic-realism-image-prompts/
            ├── SKILL.md
            ├── assets/
            │   └── prompt-template.md
            ├── examples/
            │   └── EXAMPLES.md
            └── references/
                ├── camera-lighting.md
                ├── prompt-architecture.md
                ├── realism-and-negative.md
                └── subject-guides.md
```

## 使用方式

### GitHub Copilot 项目级 Skill

保留仓库中的以下目录：

```text
.github/skills/cinematic-realism-image-prompts/
```

Copilot 在相关任务中会根据 `SKILL.md` 的 `description` 判断是否加载。

### 其他支持 Agent Skills 的工具

将 `cinematic-realism-image-prompts` 整个目录复制到工具支持的 Skills 路径，例如：

```text
.agents/skills/
.claude/skills/
```

不同客户端的路径可能不同，请以其当前文档为准。


## 上传到 GitHub

在仓库目录中运行：

```bash
git init
git add .
git commit -m "feat: add cinematic realism image prompt skill"
git branch -M main
git remote add origin <你的 GitHub 仓库地址>
git push -u origin main
```

也可以直接在 GitHub 网页新建仓库，然后上传压缩包解压后的全部文件。请确保 `.github` 隐藏目录一并上传。

建议仓库名称：

```text
cinematic-realism-image-prompt-skill
```

建议首次发布标签：

```text
v1.0.0
```


## 示例调用

```text
请使用 cinematic-realism-image-prompts skill，
把这个想法完善成电影级真实图像提示词：

一只老虎在浅水中戏水，身体肌肉线条自然显现，
表情淡然，不要攻击感，不要 AI 油感，横屏 4K。
```

```text
请诊断下面提示词为什么生成结果像游戏 CG，
然后按真实摄影、物理光影和电影构图重写。
```

```text
给我三个不同构图版本：
红墙杏花下只有一位古代东亚女子，
人物漂亮、大气、御姐感，但不摆拍。
```

## Skill 的输出逻辑

默认给出：

1. 一句场景定位；
2. 完整提示词；
3. 针对当前主题的负面提示词；
4. 必要时附精简版。

它不会只堆叠 “8K、masterpiece、photorealistic”，而会重点描述：

- 主体解剖和动作；
- 光源与影子；
- 毛发、皮肤、衣料和水体；
- 地面接触、倒影和环境交互；
- 前中后景；
- 镜头高度、焦段和景深；
- 真实的不完美；
- 当前主题最容易产生的 AI 错误。

## 设计原则

- 一个提示词锁定一个具体画面；
- 抽象气质必须转化为可观察细节；
- 真实感来自物理关系，而非质量词；
- 光线必须有来源；
- 构图服务于情绪；
- 相机参数与场景一致；
- 负面提示针对具体失败原因；
- 不为增加篇幅重复同义句。

## 验证

可使用 Agent Skills 官方参考验证器：

```bash
skills-ref validate ./.github/skills/cinematic-realism-image-prompts
```

## License

MIT
