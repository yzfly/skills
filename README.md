<div align="center">

<img src="assets/logo.svg" alt="yzfly skills" width="72">

# 云中江树 Skills

**云中江树（yzfly）的 AI Agent Skills 统一仓库**

一行命令安装，适配 Claude Code、OpenClaw、WorkBuddy、Cursor、Cline 等 17+ 种 Agent 工具

[![Latest Release](https://img.shields.io/github/v/release/yzfly/skills?color=brightgreen)](https://github.com/yzfly/skills/releases/latest)
[![Stars](https://img.shields.io/github/stars/yzfly/skills?style=social)](https://github.com/yzfly/skills)

</div>

---

## Skill 列表

| Skill | 说明 | 安装 | 许可 |
|---|---|---|---|
| [**CTO**](skills/cto/) `cto` | 你不缺 idea，你缺一个把 idea 想清楚的人。一场对话把想法变成可执行的软件设计：brief + arch + specs 直接喂给 coding agent | `npx skills add yzfly/skills@cto -g -y` | CC BY-NC 4.0 |
| [**呼吸感品牌全案**](skills/breathing-brand/) `breathing-brand` | 拒绝廉价感：高纯度色块 + 留白、线条即链接、线条 Emoji、六件物料统一落地，一场对话产出出海品牌视觉全案与生图提示词 | `npx skills add yzfly/skills@breathing-brand -g -y` | CC BY-NC 4.0 |
| [**公众号排版**](skills/mp-layout/) `mp-layout` | 越简单越高级：正文 16px / 行距 1.75 / 两端 16px / 一种品牌色 / 3–5 张图，把文章排成可直接粘贴进公众号编辑器的内联 HTML，附零依赖转换脚本与排版体检 | `npx skills add yzfly/skills@mp-layout -g -y` | MIT |
| [**像素精灵**](skills/pixel-sprite/) `pixel-sprite` | 把参考图里的主体一比一转成 32×32 复古游戏像素图标：不重新设计、不换配色，硬边像素、6–8 色、纯白背景，适合 App 图标 / 吉祥物 / 商品图 | `npx skills add yzfly/skills@pixel-sprite -g -y` | MIT |
| [**王者大师**](skills/wzry-build-advisor/) `wzry-build-advisor` | 王者荣耀出装参谋：报上你的英雄、对面难搞的英雄和当前装备，30 秒内给出下一件装备与成装路线 | `npx skills add yzfly/skills@wzry-build-advisor -g -y` | MIT |

> 每个 skill 目录内有各自的完整介绍（点上方名字进入）。

### 收录中

以下 skills 目前在各自的旗舰仓库维护，将陆续同步收录进本仓库：

| Skill | 旗舰仓库 | 简介 |
|---|---|---|
| LangGPT | [yzfly/LangGPT](https://github.com/yzfly/LangGPT) ⭐12k+ | 结构化提示词，人人都能成为提示词专家 |
| Awesome Design HTML | [yzfly/awesome-design-html](https://github.com/yzfly/awesome-design-html) | 115 个品牌风格 HTML 设计，一句话生成 Linear 风 / 飞书风页面 |
| Structured Prompt Writer | [yzfly/structured-prompt-skill](https://github.com/yzfly/structured-prompt-skill) | 395+ 提示词模板的结构化提示词写作技能 |
| Mind Clone | [yzfly/Mind-Cloning-Engineering](https://github.com/yzfly/Mind-Cloning-Engineering) | 基于 Agent Skills 的心智克隆工程 |
| Taste PM | [yzfly/taste-pm](https://github.com/yzfly/taste-pm) | 有品味的产品设计：从业务需求推导信息架构与交互 |
| Chrome QA Agent | [yzfly/chrome-qa-agent](https://github.com/yzfly/chrome-qa-agent) | 基于 chrome-devtools MCP 的对抗式 UI 测试 |

## 安装方式

**通用（推荐，适配 17+ 种 Agent 工具）：**

```bash
npx skills add yzfly/skills@<skill-name> -g -y
```

**Claude Code 手动安装：**

```bash
git clone https://github.com/yzfly/skills.git
cp -r skills/skills/<skill-name> ~/.claude/skills/
```

**OpenClaw（ClawHub）：**

```bash
clawhub install <skill-name>
```

**WorkBuddy：** 直接对它说「帮我安装 yzfly/skills@\<skill-name\>」，或手动复制到 `~/.workbuddy/skills/`。

## 仓库结构

```
skills/
  <skill-name>/
    SKILL.md        # 技能定义（frontmatter: name + description 触发条件）
    README.md       # 该 skill 的完整介绍与安装说明
    LICENSE         # 各 skill 独立许可（见下）
    references/     # 按需加载的参考资料（纯文本）
```

## 许可

**按 skill 双轨授权**，以各 skill 目录内的 `LICENSE` 为准：

- **工具型** skill 采用 MIT（如 `wzry-build-advisor`）
- **方法论 / 内容型** skill 采用 [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/)（如 `cto`），商用请联系作者

各 skill 内如引用第三方内容，版权归属见其自述文件。

## 作者

**云中江树** · 微信公众号：云中江树

> 关注公众号，看更多 AI Agent 工程实践

---

<div align="center">

**如果这些 skills 帮到你，给个 ⭐ 是最直接的支持。**

</div>
