# 78gpt — ChatGPT Plus 卡密充值前台

纯静态单页，调用 `https://gpt.86gamestore.com/api/check` 与 `/api/activate` 完成卡密查询和激活。

## 部署

直接在 Vercel 导入此 GitHub 仓库，无需任何构建配置，Vercel 会自动把 `index.html` 作为首页发布。

## 文件

- `index.html` — 充值页面
- `vercel.json` — Vercel 路由配置（`cleanUrls` 去掉 .html 后缀）

## 后端接口

页面内 `API_BASE` 已硬编码为：
```
https://gpt.86gamestore.com/api
```

如果后端域名变更，编辑 `index.html` 顶部 `<script>` 里的 `API_BASE` 常量即可。
