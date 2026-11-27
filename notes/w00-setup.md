# W0 · 准备

日期：2026-11-27

## 为什么要学这个

AI 生成的代码默认偏旧：训练数据里堆着大量 2015–2020 年的写法。真正用过原生能力的人，才能判断 AI 给的是"能用"还是"过时"。

## 本周要做的事

- [ ] 安装 Obsidian，打开本仓库作为 vault
- [ ] 安装 Spaced Repetition 插件
- [ ] 双击打开第一篇 demo：
      `guides/ui-behaviors/animate-to-from-top-layer/demo.html`
      （本地没有原仓库的话，先 `git clone https://github.com/GoogleChrome/modern-web-guidance-src`）
- [ ] 读 `guides/README.md` 了解结构
- [ ] 写下自己的目标

## 我的目标

（用自己的话写，写完删除本行）

例如：
- 能独立判断一个 UI 需求该用原生 API 还是库
- 把项目里手写的 dialog / tooltip / 表单校验换成平台能力
- 8 周后能看懂 modern-web-guidance 里的任意一篇指南

## 第一篇笔记：animate-to-from-top-layer

**问题**：`<dialog>` 打开时从 `display: none` 变成可见，是离散变化，普通 `transition` 不起作用。

**方案**：

```css
dialog[open] {
  opacity: 1;
  transition: opacity 0.2s, display 0.2s, overlay 0.2s;
  transition-behavior: allow-discrete; /* 让 display 也能过渡 */
  @starting-style { opacity: 0; }      /* 定义"从哪来" */
}
```

**记忆点**：`allow-discrete` 管"离散属性怎么变"，`@starting-style` 管"第一次出现从什么状态开始"。

## 复习卡片

`@starting-style` 解决什么问题？::让元素首次渲染（或 `display:none` 变可见）时有一个起始状态可以过渡，避免进场动画失效。

`transition-behavior: allow-discrete` 是做什么的？::允许 `display`、`overlay` 这类离散属性参与过渡，同时让元素在退场动画期间保持可见。