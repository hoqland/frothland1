# Help Center · FAQ + LandX Memory

一个轻量、现代的帮助中心/FAQ 模版：分类侧栏 + 大搜索框 + 折叠卡片 + 本地收藏模块 **LandX**（localStorage 持久化）。

## 文件
- `index.html` 页面结构（侧栏、LandX 面板、内容区）
- `styles.css` 轻量浅色设计
- `app.js` 渲染、搜索、分类、折叠、LandX 收藏
- `faq.json` 数据源（可自由增删）

## 部署到 GitHub Pages
1. 新建 public 仓库，上传全部文件到根目录。
2. 仓库 `Settings → Pages`：Source 选 **Deploy from a branch**，Branch 选 **main / root**。
3. 等 1–2 分钟即可访问。

## 编辑数据
在 `faq.json` 增加一条：
```json
{
  "id": "q-unique-id",
  "question": "问题标题？",
  "answer": "答案内容，可以包含简单 HTML（例如 <code>code</code>）。",
  "category": "General FAQ",
  "tags": ["tag1","tag2"]
}
```

## LandX 记忆模块
- 每条问答右下角「☆ 收藏到 LandX」可加入收藏。
- 侧栏会显示你收藏的问答，点击可直达，支持移除/清空。
- 数据仅保存在本地浏览器的 `localStorage` 中。

## 自定义
- 主题色：改 `styles.css` 里的 `--brand / --brand2`。
- 类目图标：在 `app.js` 的 `emojis` 映射里自定义。
