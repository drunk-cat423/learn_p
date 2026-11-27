# 练习 Demo

自己写的、改造过的可运行示例放这里。每个 demo 一个文件夹：

```
demos/
├── native-dialog/
│   ├── index.html
│   └── README.md   ← 一句话说明练了什么
└── has-selector-cards/
    ├── index.html
    └── README.md
```

## 建议的练习清单

| 对应周 | 练习 | 检验什么 |
|---|---|---|
| W1 | 原生 `<user-card>` 自定义元素 | Web Components 心智模型 |
| W2 | 卡片列表用 `:has()` + 容器查询 | 告别 JS 算布局 |
| W3 | 带 `:user-invalid` 的注册表单 | 原生校验边界 |
| W4 | `<dialog>` + `popover` 重做弹窗 | 零 JS 关闭逻辑 |
| W5 | 列表增删的 View Transition | 平台级过渡 |
| W6 | `scheduler.yield` 拆分长任务 | INP 改善 |
| W7 | 错误播报 + Trusted Types 审计 | 无障碍与安全 |

## 跑起来

直接双击 `index.html` 即可。需要本地服务器时：

```bash
npx serve .
```