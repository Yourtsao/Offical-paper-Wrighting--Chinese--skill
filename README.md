# 秘书材料星 · 智能公文写作 Agent Skill 🇨🇳📝

**Developed by a senior office director in China's state-owned system with a PhD in management who taught himself coding.** This intelligent gongwen (Chinese official document) writing Skill models the full pipeline of 38 document types, uses template-guided Q&A, a reviewer-profiling mechanism, marks all missing info as `[待补]` — never fabricates — and aligns precisely with **GB/T 9704** via a knowledge base of hundreds of thousands of characters plus 6,500 lines of core code.

Less hair loss, less pointless overtime — documents pass on the first draft, approval rate up to 10x faster. Save time and enjoy life. **Wanna know how Chinese official writing works? Just try!**
**Keywords:** `Chinese official document writing` · `gongwen` · `公文写作` · `国企公文` · `机关公文` · `Agent Skill` · `Claude Code skill` · `GB/T 9704` · `请示` · `报告` · `总结` · `讲话稿` · `会议纪要` · `通知` · `函` · `意见` · `批复` · `述职报告` · `调研报告`

---

## ✨ 能力概览 / Capabilities

| 中文 | English |
|------|---------|
| 覆盖 **38 类** 常用公文文种（请示、报告、总结、讲话稿、纪要、通知、函、意见、批复、决定、方案、计划、述职、调研、简报、党课、党建…） | Covers **38 categories** of official documents (requests, reports, summaries, speeches, meeting minutes, notices, letters, opinions, approvals, plans, briefings…) |
| 服务端 **43.8 万字** 全量写作知识库，实时更新，包内不内置 | Server-side **438K-character** writing knowledge base, always up to date, zero knowledge bundled |
| 按 GB/T 9704 生成 **Word（docx）** 公文，可直接走 OA | Generates **Word (docx)** documents per GB/T 9704, OA-ready |
| **防杜撰机制**：缺失数字/文号/人名一律 `〔待补〕` 标注 | **Anti-hallucination**: missing data is always marked `〔待补〕`, never fabricated |
| 受众画像 + 一键切换行文风格（向上管理） | Audience profiling + one-click style switching |
| 免费试用：注册送 10 次（7 天内有效） | Free trial: 10 calls on registration (valid 7 days) |

## 🚀 快速上手 / Quick Start

1. **安装 / Install**: 在 Claude Code / WorkBuddy / Dify / 魔搭等平台导入本 Skill（仓库根目录即标准 Agent Skills 包：`SKILL.md` + `references/`）
   - *Import this repo as an Agent Skill (SKILL.md at repo root + references/)*
2. **配置 / Configure**: 在 `config.json` 填入有效的 `GATEWAY_SECRET`（联系作者获取）
   - *Fill a valid `GATEWAY_SECRET` in `config.json` (contact author)*
3. **使用 / Use**: 直接说「帮我写一份关于XX的请示 / 报告 / 通知 / 总结…」，按引导提供邮箱注册即可
   - *Just say "write a gongwen request/report/summary about X…" and follow the guided flow*

## 📦 包含文件 / Files

| 文件 / File | 说明 / Description |
|-------------|-------------------|
| `SKILL.md` | Skill 主文件：调用流程与配额说明 / Main skill file: flow & quota |
| `references/word-export.md` | 公文 Word 版式导出指引（GB/T 9704）/ Word export guide |
| `config.json` | 网关配置（`GATEWAY_SECRET` 需联系作者）/ Gateway config (secret from author) |

## 💰 付费模式 / Pricing

- 免费试用：注册送 **10 次**（7 天有效）/ Free: 10 calls on signup
- 按次：**2 元/次** / Pay-per-call: ¥2
- 包年：**399 元/年**，不限次 / Yearly: ¥399, unlimited
- 机构定制 / API 接入 / 私有化部署：联系作者 / Custom & on-prem: contact author

## 📧 联系 / Contact

- 邮箱 / Email: 804652586@qq.com
- 电话 / Phone: 17019921000

## ⚖️ 版权 / Copyright

本技能包为版权产品，受中国版权保护，未经许可不得复制、转售、抄袭。
Licensed product. Reproduction, resale or plagiarism prohibited.
