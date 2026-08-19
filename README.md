# 品控稽核独立看板

此目录为独立版本，不依赖 WorkBuddy。

## 文件

- `index.html`：看板页面与筛选、统计逻辑。
- `data/qc-data.json`：可审计的业务数据源。
- `data/qc-data.js`：浏览器直接加载的数据文件，由 JSON 生成。
- `update-data.mjs`：修改 JSON 后重新生成 JS 数据文件。

## 更新数据

1. 更新 `data/qc-data.json`。
2. 在本目录执行：`node update-data.mjs`。
3. 打开 `index.html` 检查日期、报告数、问题点和红线数。

当前数据范围：2026-08-01 至 2026-08-19。

