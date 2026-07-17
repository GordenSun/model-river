# 模型的长河 · River of Models

> 一幅徐徐展开的长卷：从 ChatGPT (2022-11-30) 到昨日，84 个知名 AI 大模型、13 家实验室、45 个月的发布编年史。

**在线预览：<https://gordensun.github.io/model-river/>**

## 这是什么

一个单文件（`index.html`）的滚动驱动动画页面：

- 日历如画卷般横向展开（竖向滚动驱动镜头平移，带惯性跟拍）
- 每个模型在其发布日期被逐一点亮（共 84 盏）
- 每个节点附带模型名、厂商名、厂商图标与一句话备注
- 卷首题字、月份刻度、年份章节、卷轴轴杆、星空与年份水印

零依赖：无构建步骤、无框架、无外部 JS 库，字体来自 Google Fonts CDN。
厂商图标来自 [LobeHub Icons](https://lobehub.com/zh/icons)（[@lobehub/icons-static-svg](https://www.npmjs.com/package/@lobehub/icons-static-svg)，MIT），已内联为单色 SVG。

## 数据

完整数据与月/年/厂商分布见 [MODELS.md](./MODELS.md)。页面内数据与之一致（`index.html` 中 `MODELS` 数组）。

- 范围：2022-11-30 → 2026-07-16，知名基础模型与旗舰模型
- 标「约」的条目为月份级约数

## 本地预览

```bash
cd model-river
python3 -m http.server 8000
# 打开 http://localhost:8000
```

或直接双击 `index.html`。

## 部署

静态托管即可（本仓库使用 GitHub Pages，分支 `main` 根目录）。
