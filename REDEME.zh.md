# 超能力

超能力是一套完整的软件开发方法论，专为您的编程智能体构建，基于一组可组合的技能和初始指令，确保您的智能体能有效运用这些能力。

## 工作原理

从您启动编程智能体的那一刻开始。当它发现您正在构建某些东西时，它*不会*立即尝试编写代码，而是先退一步，询问您真正想要实现的目标。

通过对话明确需求后，它会将设计规范分成易于阅读和理解的小块呈现给您。

在您确认设计方案后，您的智能体会制定一个足够清晰的实施计划，即使是一个品味不佳、缺乏判断力、不了解项目背景且讨厌测试的初级工程师也能遵循。该计划强调真正的红/绿测试驱动开发（TDD）、YAGNI（你不会需要它）和DRY原则。

接下来，一旦您说"开始"，它会启动一个*子智能体驱动开发*流程，让多个智能体协作完成每个工程任务，检查并评审彼此的工作，持续推进。Claude通常能够在不偏离您制定的计划的情况下，自主工作数小时。

虽然还有更多细节，但这是该系统的核心。由于技能会自动触发，您无需进行任何特殊操作。您的编程智能体只需拥有"超能力"即可。

## 赞助

如果"超能力"帮助您完成了能赚钱的项目，并且您愿意支持，我将非常感谢您考虑[赞助我的开源工作](https://github.com/sponsors/obra)。

谢谢！

- Jesse

## 安装

**注意：** 安装方法因平台而异。

### Claude Code 官方市场

可通过[官方Claude插件市场](https://claude.com/plugins/superpowers)获取"超能力"。

从Anthropic官方市场安装插件：

```bash
/plugin install superpowers@claude-plugins-official
```

### Claude Code（超能力市场）

超能力市场为Claude Code提供"超能力"和一些相关插件。

在Claude Code中，先注册市场：

```bash
/plugin marketplace add obra/superpowers-marketplace
```

然后从该市场安装插件：

```bash
/plugin install superpowers@superpowers-marketplace
```

### OpenAI Codex CLI

- 打开插件搜索界面

```bash
/plugins
```

搜索超能力

```bash
superpowers
```

选择`安装插件`

### OpenAI Codex 应用

- 在Codex应用中，点击侧边栏的"插件"。
- 您应在"编程"部分看到`超能力`。
- 点击超能力旁边的`+`并按照提示操作。

### Cursor（通过插件市场）

在Cursor Agent聊天中，从市场安装：

```text
/add-plugin superpowers
```

或在插件市场中搜索"superpowers"。

### OpenCode

告诉OpenCode：

```
从 https://raw.githubusercontent.com/obra/superpowers/refs/heads/main/.opencode/INSTALL.md 获取并遵循说明
```

**详细文档：** [docs/README.opencode.md](docs/README.opencode.md)

### GitHub Copilot CLI

```bash
copilot plugin marketplace add obra/superpowers-marketplace
copilot plugin install superpowers@superpowers-marketplace
```

### Gemini CLI

```bash
gemini extensions install https://github.com/obra/superpowers
```

更新：

```bash
gemini extensions update superpowers
```

## 基本工作流程

1. **头脑风暴** - 在编写代码前激活。通过提问完善初步想法，探索替代方案，分节呈现设计以供确认。保存设计文档。

2. **使用Git工作树** - 设计确认后激活。在新分支上创建独立工作区，运行项目设置，验证干净的测试基线。

3. **编写计划** - 设计确认后激活。将工作分解为小块任务（每个2-5分钟）。每个任务包含确切文件路径、完整代码和验证步骤。

4. **子智能体驱动开发**或**执行计划** - 计划制定后激活。为每个任务分配新的子智能体，进行两阶段评审（规范符合性，然后代码质量），或分批执行并设置人工检查点。

5. **测试驱动开发** - 实施过程中激活。强制执行红-绿-重构循环：编写失败测试，观察失败，编写最少代码，观察通过，提交。删除在测试前编写的代码。

6. **请求代码评审** - 任务间激活。对照计划进行评审，按严重程度报告问题。关键问题会阻止进度。

7. **完成开发分支** - 任务完成后激活。验证测试，提供选项（合并/拉取请求/保留/丢弃），清理工作树。

**智能体在任何任务前都会检查相关技能。** 这是强制性的工作流程，而非建议。

## 内容概览

### 技能库

**测试**
- **测试驱动开发** - 红-绿-重构循环（包含测试反模式参考）

**调试**
- **系统化调试** - 4阶段根本原因分析流程（包含根本原因追踪、深度防御、基于条件的等待技术）
- **完成前验证** - 确保问题真正修复

**协作**
- **头脑风暴** - 苏格拉底式设计完善
- **编写计划** - 详细实施计划
- **执行计划** - 带检查点的批量执行
- **调度并行智能体** - 并发子智能体工作流程
- **请求代码评审** - 预评审检查清单
- **接收代码评审** - 响应反馈
- **使用Git工作树** - 并行开发分支
- **完成开发分支** - 合并/拉取请求决策工作流程
- **子智能体驱动开发** - 带两阶段评审的快速迭代（规范符合性，然后代码质量）

**元技能**
- **编写技能** - 遵循最佳实践创建新技能（包含测试方法）
- **使用超能力** - 技能系统介绍

## 理念

- **测试驱动开发** - 始终先写测试
- **系统化而非临时性** - 流程优于猜测
- **降低复杂性** - 以简洁为主要目标
- **证据优于断言** - 在宣布成功前先验证

阅读[原始发布公告](https://blog.fsck.com/2025/10/09/superpowers/)。

## 贡献

以下是"超能力"的一般贡献流程。请注意，我们通常不接受新技能的贡献，且对技能的任何更新必须在我们支持的所有编程智能体上都能工作。

1. 复刻代码库
2. 切换到'dev'分支
3. 为您的工作创建分支
4. 遵循`编写技能`技能来创建和测试新的及修改后的技能
5. 提交拉取请求，务必填写拉取请求模板。

完整指南请参见`skills/writing-skills/SKILL.md`。

## 更新

"超能力"的更新方式因编程智能体而异，但通常是自动的。

## 许可证

MIT许可证 - 详见LICENSE文件

## 社区

"超能力"由[Jesse Vincent](https://blog.fsck.com)和[Prime Radiant](https://primeradiant.com)的团队构建。

- **Discord**：[加入我们](https://discord.gg/35wsABTejz)获取社区支持、提问并分享您使用"超能力"构建的项目
- **问题反馈**：https://github.com/obra/superpowers/issues
- **版本发布公告**：[注册](https://primeradiant.com/superpowers/)获取新版本通知
