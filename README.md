# 老板的博客 📊

个人博客站点 - 业务思考 · 市场分析 · 产品规划

## 快速部署

### 方案一：GitHub Pages（推荐）

```bash
# 1. 初始化 Git
cd blog
git init
git add .
git commit -m "Initial blog"

# 2. 创建 GitHub 仓库并推送
git remote add origin https://github.com/你的用户名/你的仓库名.git
git branch -M main
git push -u origin main

# 3. 在 GitHub 设置中启用 Pages
# Settings → Pages → Source: main branch → Save
```

访问：`https://你的用户名.github.io/你的仓库名/`

### 方案二：Vercel

```bash
# 1. 安装 Vercel CLI
npm install -g vercel

# 2. 部署
cd blog
vercel

# 3. 按提示完成配置
```

### 方案三：本地预览

```bash
# 用任意 HTTP 服务器
python3 -m http.server 8000
# 或
npx serve
```

访问：`http://localhost:8000`

## 添加新文章

1. 复制 `articles/hello-world.html` 为新文件
2. 修改文件名、标题、日期、内容
3. 在 `index.html` 中添加文章链接

## 自定义

- 修改 `index.html` 中的博客名称和描述
- 调整 CSS 变量更改主题色
- 编辑 `about.html` 更新个人信息

## 文件结构

```
blog/
├── index.html          # 首页
├── about.html          # 关于页
├── articles/           # 文章目录
│   └── hello-world.html
└── README.md
```

---

Powered by 🦞
