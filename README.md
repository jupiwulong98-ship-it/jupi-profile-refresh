# 账号主页重做 Skill

让 AI 根据你的真实经历、账号现状与已有作品，帮你重做名称、简介、头像背景、置顶和近期内容安排。

适合：已有账号但主页表达不清楚；准备调整内容方向；希望多个平台传达同一个关注理由。默认先提供修改方案，实际修改账号需要明确目标和授权。

## 能拿到什么

- 当前主页的问题及依据。
- 一句话定位、一个推荐名称和可复制的简介。
- 头像、背景、置顶与首屏内容安排。
- 已有内容如何支持主页承诺，哪些内容还需要制作。
- 改前后记录、读者理解测试和发布复盘方法。

材料不足时会标注工作假设和缺口，不编个人经历、案例、涨粉结果或真人测试。

## 安装到 Codex

可以将下面这句话直接发给 Codex：

```text
使用 skill-installer 安装这个 Skill：
https://github.com/jupiwulong98-ship-it/jupi-profile-refresh/tree/main/skills/jupi-profile-refresh
```

也可以下载文件手动安装：

[下载 v0.1.0 ZIP 安装包](https://github.com/jupiwulong98-ship-it/jupi-profile-refresh/releases/download/v0.1.0/jupi-profile-refresh-v0.1.0.zip)

下载本仓库后，将 `skills/jupi-profile-refresh` **整个文件夹**放进你的个人 Skill 目录。本项目在 Codex 的 `~/.codex/skills/` 目录使用；配置了 `CODEX_HOME` 时使用对应目录下的 `skills/`。保留 `references/` 和 `agents/`。

安装后的结构：

```text
~/.codex/skills/jupi-profile-refresh/
  SKILL.md
  agents/openai.yaml
  references/article-workflow.md
  references/delivery.md
```

ZIP安装包解压后得到的 `jupi-profile-refresh` 文件夹可直接放入上述位置。若同名版本已经存在，先保留旧版再决定替换，不直接覆盖个人修改。ZIP内附带本项目的MIT许可证。

在新的对话中使用下面的请求。若客户端尚未发现新 Skill，检查它的 Skill 列表和目录配置，必要时重新打开客户端。不同客户端的发现方式可能不同；本项目不声称已测试所有客户端。

## 怎么用

```text
使用 $jupi-profile-refresh，帮我重做账号主页。

这是我的主页链接或当前名称、简介和截图：……
这是我已经做过的事和代表内容：……
我的目标：……

先给我一份完整方案，我看完再调整。
```

也可以把已确定的定位、内容清单或数据文件一起提供。没有链接时可以粘贴主页文字；不要求先购买接口或提供登录密码。

已有定位与素材会复用；需要补充时只问影响方案的关键事实。用户要求按步骤讨论时逐步来，要先看全貌时给完整版本。

## 方法来源

本项目的方法参考 JessiCao（@JessiCao_JC）的三篇文章：

1. [小红书起号第一步，直接抄这个SOP](https://x.com/JessiCao_JC/status/2107674848457843182)
2. [小红书第一批笔记发什么？从定位到选题，手把手列出你的内容清单](https://x.com/JessiCao_JC/status/2110614414890283326)
3. [小红书主页怎么写，别人看了才想关注你](https://x.com/JessiCao_JC/status/2110238620359778473)

Skill作者：橘皮。流程摘要见 `skills/jupi-profile-refresh/references/article-workflow.md`。仓库不分发三篇文章全文，文章作者与 Skill 作者分别署名。

## 版本与验证范围

初版：0.1.0。

已完成结构校验、安装包解压与文件一致性检查，并用 skill-installer 从公开 GitHub 仓库实际安装到临时目录核对。客户端新对话发现与实际调用尚未验收，真人理解与运营效果尚未验证。

实际主页文案是否合适，仍由使用者核对。Skill不会承诺改名或改简介后获得固定的播放、粉丝与收入。

安装与调用不代表AI已替你修改社交账号；实际执行取决于可用工具、登录状态和你明确授权的字段。
