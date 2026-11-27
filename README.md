# learn_p · 现代 Web 平台学习仓库

以 [GoogleChrome/modern-web-guidance](https://github.com/GoogleChrome/modern-web-guidance) 的 **255 篇指南**为教材，系统学习现代 Web 平台能力。

面向对象：以 TypeScript / Next.js / React 为主的后端开发者，目标是知道**什么时候该用原生 Web API，而不是手写 JS 或引入第三方库**。

## 目标

- 读懂并内化与自己相关的 40+ 篇指南
- 建立"这个需求现在有没有原生做法"的判断力
- 用间隔重复（spaced repetition）把关键 API 记牢
- 全部笔记、demo、卡片在本仓库中可检索、可复习、可版本回溯

## 周期

**8 周，每周 2 次 × 90 分钟，约 30 小时。**

详细安排见 [PLAN.md](./PLAN.md)，逐周打勾见 [progress.md](./progress.md)。

## 怎么用

### 1. 打开仓库

用 [Obsidian](https://obsidian.md/) 打开本文件夹（它就是一个普通 Markdown vault）：

```
Obsidian → Open folder as vault → 选择本仓库目录
```

装两个插件（设置 → 第三方插件）：

- **Spaced Repetition** — 复习卡片（识别 `问题::答案` 格式）
- 可选：**Obsidian Git** — 自动提交笔记

### 2. 每个指南的学习闭环

| 步骤 | 动作 | 时间 |
|---|---|---|
| 1 | 读 `guide.md`（原文链接见 PLAN.md） | 10–15 min |
| 2 | 打开同目录的 `demo.html` 看效果 | 5 min |
| 3 | 改 demo，或用自己的方式复现 | 20 min |
| 4 | 按 [notes/TEMPLATE.md](./notes/TEMPLATE.md) 写笔记 | 15 min |
| 5 | 提炼 1–2 张复习卡 | 5 min |

> 合计每个指南约 1 小时。一周 5–6 个指南 ≈ 2 次 90 分钟的学习。

### 3. 复习

- 卡片统一放在笔记末尾，`问题::答案` 一行一张
- 每天打开 Obsidian 复习 10 分钟，由 Spaced Repetition 插件调度
- 每周日回顾本周笔记，把没记住的卡片补到 `cards/`

### 4. 目录结构

```
learn_p/
├── README.md          ← 你在这里
├── PLAN.md            ← 8 周学习计划（具体到每篇指南）
├── progress.md        ← 进度追踪表
├── resources.md       ← 工具、网站、参考资料
├── notes/             ← 每周笔记（一个主题一个文件）
│   ├── TEMPLATE.md
│   └── w00-setup.md
├── cards/             ← 集中复习卡片（可选，也可放在笔记里）
├── demos/             ← 自己写的 demo 和改造实验
└── .gitignore
```

## 教材说明

- 指南原文在 [modern-web-guidance-src/guides](https://github.com/GoogleChrome/modern-web-guidance-src/tree/main/guides)
- 文档内容 CC-BY 4.0，代码 Apache 2.0
- 本仓库只保存自己的笔记、卡片和 demo，不复制原文

## 进度

见 [progress.md](./progress.md)。当前：**第 0 周 · 准备中**