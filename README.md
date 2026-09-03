# gongwen-dsh — 智能公文写作 / Official Document Writing Skill (DSH)

[![DSH Market](https://raw.githubusercontent.com/2BingLing/dsh-market/master/assets/readme/badge-listed-zh.svg)](https://dsh.market/?q=Yourtsao%2Fgongwen-dsh)

**中文**：秘书材料星 · 妙笔公文写作——面向办公室文秘岗位的 AI 公文写作插件，覆盖 38 类常用公文文种（请示、报告、总结、讲话稿、纪要、通知、函、意见、通报、批复、决定、方案、计划、述职、调研、党课、简报、致辞、主持词、贺信、倡议、申请、检讨、制度等）。体制内资深办公室主任（管理学博士）开发，模板化引导 + 受众画像定制文风 + GB/T 9704 规范排版 + 防杜撰〔待补〕机制，全部写作知识在线调取（0 知识库打包，克隆即用）。

**English**: MiaoBi Official Document Writing — an AI skill for Chinese official documents (38 types: request, report, notice, meeting minutes, speech, etc.). Built by a senior office director with a PhD in management. Template-guided Q&A, audience profiling, GB/T 9704 formatting, no-fabrication ([待补]) policy. All knowledge fetched via online API — zero KB bundled, clone & use.

---

## ✨ 能力一览 / Capabilities

| 能力 Capability | 说明 Description |
|---|---|
| 📋 38 类文种全覆盖 | 请示/报告/总结/讲话稿/纪要/通知/函/意见/批复/述职/调研/党课/简报等，识别文种自动匹配结构框架 |
| 🧭 模板化引导 | 每文种专属填写模板（受众画像选择题/案例上传/核心目的/补充信息），填完即出高质量初稿 |
| 🎯 受众画像定制 | 给集团高层讲站位、给分管领导讲重点、给检查组讲依据、给职代会讲数据——"看人下菜碟" |
| 📚 知识在线全量调取 | 43.8 万字结构化公文知识库在线调取（包内 0 知识库），结构/标题/金句/句式一次用全 |
| 📐 GB/T 9704 格式 | 字体/字号/行距/页边距全对齐，可直接走 OA 系统 |
| 🚫 防杜撰机制 | 缺失数字/文号/人名/日期一律〔待补〕标注，绝不编造 |

## 💰 计费 / Pricing（服务端强制执行）

| 档位 Tier | 价格 Price | 说明 Notes |
|---|---|---|
| 免费 Free | 注册送 **10 次 / 7 天** | 简报/请示/报告/纪要/通知/函 6 文种全量 + 其他文种 2 次体验 |
| 按次 Per-call | **2 元/次** | 即买即用，plan=per_call |
| 包年 Yearly | **399 元/年** | 38 类不限次，plan=yearly |

## 🚀 快速开始 / Quick Start

1. **注册 / Register**：用户提供邮箱 → `node scripts/register.mjs register --email <邮箱>` 发验证码 → `node scripts/register.mjs verify --email <邮箱> --code <验证码>`（送 10 次免费额度）
2. **写作 / Write**：直接说"写一份请示/通知/总结……"，自动走 `/consume` → `/search` 在线取骨架生成
3. **付款 / Pay**：微信扫码支付，二维码由网关 `/api/pay/qrcode` 实时生成（2元/次 plan=per_call；399元/年 plan=yearly）

## 🤖 调用环境适配 / Environment Guide

| 环境 Environment | 使用方式 Usage |
|---|---|
| ① 可执行代码的 Agent（WorkBuddy / DSH / Claude Code） | 插件自动加载，按 SKILL.md 走注册→/consume→/search→生成 |
| ② 纯对话 LLM（豆包/Kimi 等） | 引导用户手动执行 `scripts/register.mjs` 完成注册后，在对话中直接提写作需求 |

## 📦 目录结构 / Structure

```
gongwen-dsh/
├── package.json            # DSH 插件声明（dsh.bundle.patch）
├── cordis.patch.yml        # 插件挂载层
├── dsh/index.js            # 插件 Host（系统提示注入 + 注册引导）
├── skills/gongwen-writting/
│   ├── SKILL.md            # 技能本体（0 知识库，v1.0.64）
│   └── config.json         # GATEWAY_URL / USER_TOKEN（注册后写入）
└── scripts/register.mjs    # 注册/验证码/状态查询
```

## 📄 许可 / License

MIT License。知识库内容著作权归作者所有，仅在线调取，禁止转存传播。
