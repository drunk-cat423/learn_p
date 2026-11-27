# 8 周学习计划

**节奏**：每周 2 次 × 90 分钟。每次学 2–3 篇指南。
**原则**：不追求覆盖 255 篇，只学与"后端 + React 前端"强相关的 43 篇。
**每篇指南固定动作**：读原文 → 看 demo → 改 demo → 写笔记 → 出卡片。

原文链接前缀：`https://github.com/GoogleChrome/modern-web-guidance-src/tree/main/guides/`

---

## 第 0 周 · 准备（本周）

- [ ] 安装 Obsidian，打开本仓库作为 vault
- [ ] 安装 Spaced Repetition 插件并启用
- [ ] 跑通第一篇 demo：`ui-behaviors/animate-to-from-top-layer`（直接双击 `demo.html`）
- [ ] 读 [guides/README.md](https://github.com/GoogleChrome/modern-web-guidance-src/blob/main/guides/README.md) 了解指南的组织方式
- [ ] 在 `notes/w00-setup.md` 记下自己的起点和目标

**验收**：能用 Obsidian 打开仓库、能看到 demo 动效、能新建一篇笔记。

---

## 第 1 周 · HTML 语义与 Web Components

**目标**：理解原生组件模型，知道 React 之外还有一条路，以及什么时候值得用。

| 指南 | 链接 |
|---|---|
| HTML 总览 | `html/html` |
| Web Components | `html/web-components` |
| Custom Elements | `html/custom-elements` |
| Shadow DOM | `html/shadow-dom` |
| 表单关联的自定义元素 | `html/form-associated-custom-elements` |

**练习**：用原生 Web Components 写一个 `<user-card>`，放进 `demos/`。
**产出**：`notes/w01-html-webcomponents.md`

---

## 第 2 周 · CSS 布局与响应式

**目标**：把"布局靠 JS 算"换成"布局靠 CSS 声明"。

| 指南 | 链接 |
|---|---|
| CSS 布局总览 | `css/css-layout` |
| 响应式设计（容器查询） | `css/responsive-design` |
| 尺寸感知样式 | `css/size-aware-styling` |
| `:has()` 父级选择 | `css/style-parent-with-has` |
| 流体缩放 | `css/fluid-scaling` |
| 设计令牌响应式 | `css/design-token-reactivity` |

**练习**：把 `:has()` 和容器查询用在一个卡片列表上，写进 `demos/`。
**产出**：`notes/w02-css-layout.md`

---

## 第 3 周 · 表单与校验（和后端最相关）

**目标**：分清原生校验能做到什么、后端还必须做什么。

| 指南 | 链接 |
|---|---|
| 表单总览 | `forms/forms` |
| 交互后再校验 | `forms/validate-input-after-interaction` |
| 必填字段反馈 | `forms/required-field-feedback` |
| 字段自动适应内容 | `forms/form-fields-automatically-fit-contents` |
| 组合框（可搜索下拉） | `forms/combobox` |
| 品牌一致性表单 | `forms/brand-consistent-forms` |

**练习**：做一个带 `:user-invalid` 校验的注册表单，同时写一段对应的后端校验伪代码，对比职责边界。
**产出**：`notes/w03-forms.md`

---

## 第 4 周 · 对话框与浮层

**目标**：彻底替换"手写 div 弹窗 + JS 遮罩 + body overflow hidden"。

| 指南 | 链接 |
|---|---|
| 声明式 dialog/popover 控制 | `ui-behaviors/declarative-dialog-popover-control` |
| 点击外部关闭 | `ui-behaviors/light-dismiss-a-dialog` |
| 禁止背景滚动 | `ui-behaviors/prevent-page-scroll-under-modal-dialog` |
| top layer 进出场动画 | `ui-behaviors/animate-to-from-top-layer` |
| 悬停提示 | `ui-behaviors/interest-triggered-tooltips` |
| 锚点定位的下划线 | `ui-behaviors/anchor-positioning-tab-underline` |

**练习**：用原生 `<dialog>` + `popover` 重做一个弹窗，零 JS 关闭逻辑。
**产出**：`notes/w04-dialog-popover.md`

---

## 第 5 周 · 过渡与动效

**目标**：页面切换、元素进出用平台能力，不引动画库。

| 指南 | 链接 |
|---|---|
| 同文档过渡 | `ui-behaviors/same-document-transitions` |
| 跨文档过渡 | `ui-behaviors/cross-document-transitions` |
| 元素进出场动画 | `ui-behaviors/animate-element-entry-exit` |
| 动效总览 | `ui-behaviors/motion` |
| 物理缓动 | `ui-behaviors/physics-based-easing` |
| 滚动进出视口效果 | `ui-behaviors/scroll-entry-exit-effects` |

**练习**：给一个列表加 View Transitions，支持"添加/删除"的平滑过渡。
**产出**：`notes/w05-transitions.md`

---

## 第 6 周 · 性能

**目标**：知道加载和交互的关键指标，以及对应的原生手段。

| 指南 | 链接 |
|---|---|
| 性能总览 | `performance/performance` |
| 预加载优先级 | `performance/optimize-preload-priority` |
| 图片优先级 | `performance/optimize-image-priority` |
| 定位 INP 原因 | `performance/identify-inp-causes` |
| 拆分长任务 | `performance/break-up-long-tasks` |
| 按优先级调度任务 | `performance/schedule-tasks-by-priority` |
| 延迟渲染重内容 | `performance/defer-rendering-heavy-content` |

**练习**：用 Chrome DevTools 的 Performance 面板分别测一个"同步长任务"和 `scheduler.yield` 版本。
**产出**：`notes/w06-performance.md`

---

## 第 7 周 · 无障碍与安全

**目标**：不把它当合规负担，而当成"少写 bug 的默认路径"。

| 指南 | 链接 |
|---|---|
| 无障碍总览 | `accessibility/accessibility` |
| 错误信息可播报 | `accessibility/accessible-error-announcement` |
| 生成内容的可访问性 | `accessibility/accessible-generated-content` |
| 尊重系统字号 | `accessibility/respect-os-text-scale` |
| 安全总览 | `security/security` |
| 消毒不可信 HTML | `security/sanitize-untrusted-html` |
| Trusted Types | `security/trusted-types` |
| 校验来源 | `security/validate-origins` |

**练习**：给第 3 周的表单补上正确的错误播报，并用 `Trusted Types` 思路审一遍自己的 `innerHTML` 用法。
**产出**：`notes/w07-a11y-security.md`

---

## 第 8 周 · 实战与复盘

- [ ] 在自己的一个项目里跑 `npx modern-web-guidance@latest legacy-scan .`，记录发现
- [ ] 从 [Frontend Mentor](https://www.frontendmentor.io/challenges) 挑一个挑战，全程用学过的现代写法完成
- [ ] 复盘：哪些指南"实际用上了"，哪些"只是知道了"
- [ ] 更新索引和下一阶段计划

**产出**：`notes/w08-retro.md`

---

## 调整规则

- 某周没完成：不跳周，顺延，保持"一周一主题"
- 某个指南太难：先跳到下一篇，标记 `#待回看`，第 8 周统一处理
- 发现和实际工作相关的指南：加进下周清单，替换不相关的