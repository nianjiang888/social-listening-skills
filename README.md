# 中文社媒舆情监听技能

1 个自包含 Agent 技能：围绕品牌/产品/事件在小红书、抖音、知乎、微博、B站、头条六端做近 30 天舆情研究，输出带引用、按声量排序的中文简报。

共 **1** 个技能包，全部自包含（包内即可跑通，无需额外依赖）。

## 技能一览

| # | 技能包 | 名称 | 做什么 |
|---|---|---|---|
| 1 | `cn-social-listening` | 中文舆情监听助手 | 中文社媒舆情研究简报。触发词：舆情监听/口碑研究/品牌舆情/舆情分析/舆情简报/社媒监测/小红书舆情/抖音舆情/知乎… |

## 目录结构

```
social/
├── cn-social-listening/
├── ...（共 1 个技能目录）
```

本技能包结构：`SKILL.md`（技能定义与工作流）、`references/sources.md`（六端查询模板与评分卡）。为纯工作流型技能，不含脚本与二进制文件，Agent 按 SKILL.md 指引调用环境内的网页搜索/读取能力即可运行。

## 本地使用

```
git clone <仓库地址>
```

把 `cn-social-listening/` 目录整体复制到你的 Agent skills 目录即可。这是一个纯指令型技能（无脚本引擎），Agent 读取 `SKILL.md` 后按六步工作流执行，按需加载 `references/sources.md` 作为六端查询模板与评分卡依据。

## 从 GitHub 导入到 SkillHub

每个技能独立目录，目录根即 `SKILL.md`，不含二进制文件。在 SkillHub 发布页选「从 GitHub 导入」，绑定账号后会自动扫出候选技能。

**注意：平台单次最多导入 5 个技能，1 个需要分 1 批。**

## 许可

MIT

## 出品方与更多工具

本技能系列由墨金格团队出品。主产品[墨金格](https://www.mojinge.cloud)（mojinge.cloud）——把故事变成短剧：一句想法进来，一部能拍的剧本出去，分集剧情、人物 / 场景 / 道具资产、每集分镜提示词一次给齐；导入小说可走全流程改编（导入 → 故事中枢 → 分集大纲 → 改编剧本 → 分镜脚本）。按次付费，生成失败不扣费，邮箱即账号。

Made by the team behind [Mojinge](https://www.mojinge.cloud) — turn a story into a shootable screenplay: episode breakdowns, character/scene/prop assets, and per-shot prompts in one pass.

配套开源件 [ShotLock](https://github.com/nianjiang888/shotlock)：分镜脚本一致性校验引擎，十五条规则专抓角色漂移、越轴、语速超载，可作生成流程的卡口。
