# 工具与资料

## 教材

| 资源 | 链接 | 用途 |
|---|---|---|
| modern-web-guidance（发布版） | https://github.com/GoogleChrome/modern-web-guidance | 安装说明、最新版 |
| modern-web-guidance-src（源仓库） | https://github.com/GoogleChrome/modern-web-guidance-src | 255 篇指南原文 |
| 官方文档 | https://developer.chrome.com/docs/modern-web-guidance | 使用说明 |
| 评测面板 | https://googlechrome.github.io/modern-web-guidance-src/ | 看各 Agent 学习效果 |

## 查证（遇到不懂的 API）

| 资源 | 链接 | 用途 |
|---|---|---|
| MDN Web Docs | https://developer.mozilla.org | API 权威参考 |
| web.dev | https://web.dev | 最佳实践文章 |
| Can I Use | https://caniuse.com | 兼容性 |
| Baseline | https://web.dev/baseline | 特性成熟度（跨浏览器支持等级） |

> 指南里反复出现的 "Baseline Widely available"，判断依据就是 Baseline 标准。

## 练习

| 资源 | 链接 | 用途 |
|---|---|---|
| Frontend Mentor | https://www.frontendmentor.io/challenges | 真实设计稿还原，练 HTML/CSS |
| CSS Battle | https://cssbattle.dev | 游戏化练 CSS，每日挑战 |
| 本地跑 demo | 直接双击 `demo.html`，或 `npx serve` | 看指南自带的示例 |

## 工具

| 工具 | 用途 | 安装 |
|---|---|---|
| Obsidian | 笔记编辑器，直接打开本仓库 | https://obsidian.md/ |
| Spaced Repetition（Obsidian 插件） | 间隔重复复习卡片 | 社区插件市场搜索 |
| Obsidian Git（可选） | 自动 commit/push 笔记 | 社区插件市场搜索 |
| Chrome DevTools | 性能面板、无障碍面板 | Chrome 自带 |

## AI 辅助（可选）

- **CLI 直接查**：
  ```bash
  npx modern-web-guidance@latest search "锚点定位 tooltip"
  npx modern-web-guidance@latest retrieve "animate-to-from-top-layer"
  ```
- **Obsidian MCP**：可以让 Claude 直接读写 vault（需要 MCP 客户端）
  - 参考实现：https://github.com/MarkusPfundstein/mcp-obsidian
  - 用途：让 AI 帮你整理笔记、生成复习卡

## 学习法

- **主动回忆** > 重读：合上笔记，用 `问题::答案` 卡片自测
- **费曼技巧**：每篇笔记都要有一个"给外行讲"的段落
- **间隔重复**：每天 10 分钟复习，比周末突击 2 小时有效
- **最小可跑**：任何概念都要落到一个能双击打开的 `demo.html`