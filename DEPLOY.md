# 快速部署指南

## 前置条件

- GitHub 账号
- Node.js 和 npm 安装（用于本地开发）
- 可选：Formspree 账号（用于接收联系表单）

---

## 1. 配置个人信息

### 编辑联系方式

编辑文件：[source/contact/index.md](file:///workspace/hexo-portfolio/source/contact/index.md)

替换以下内容：
- `your-email@example.com` → 你的真实邮箱
- `your-wechat-id` → 你的微信号
- `your-phone-number` → 你的手机号

### 编辑联系表单（可选）

如果需要使用 Formspree 接收表单提交：
1. 注册 [formspree.io](https://formspree.io/)
2. 创建新表单
3. 替换 `your-form-id` 为你的表单 ID

---

## 2. 更新站点配置

### 编辑主配置

编辑文件：[_config.yml](file:///workspace/hexo-portfolio/_config.yml)

更新内容：
- `title`: 你的名字或品牌名
- `subtitle`: 简短介绍
- `description`: SEO 描述
- `author`: 你的名字
- `url`: 你的 GitHub Pages URL（例如：`https://jinxuchen2020.github.io/me/`）

---

## 3. 部署到 GitHub Pages

### 方法一：使用 GitHub Actions 自动部署

项目已包含 GitHub Actions 配置，可自动部署：

1. 将代码推送到 GitHub
2. 在仓库设置中启用 GitHub Pages
3. 将部署分支设置为 `gh-pages`

### 方法二：手动部署

```bash
cd /workspace/hexo-portfolio
npm install
npm run build
npm run deploy
```

---

## 4. 项目文件结构

```
/workspace/hexo-portfolio/
├── source/
│   ├── portfolio/        # 作品集页面
│   ├── services/         # 服务介绍
│   └── contact/          # 联系方式
├── _config.yml           # 主配置
├── _config.next.yml      # NexT 主题配置
└── README.md             # 项目说明
```

---

## 5. 自定义内容

### 添加更多作品集项目

在 [source/portfolio/index.md](file:///workspace/hexo-portfolio/source/portfolio/index.md) 中添加更多项目卡片，使用以下模板：

```html
<div class="portfolio-card">
  <div class="portfolio-image" style="background: linear-gradient(135deg, #颜色1 0%, #颜色2 100%);">图标</div>
  <div class="portfolio-content">
    <div class="portfolio-title">项目名</div>
    <div class="portfolio-desc">项目描述</div>
    <div class="portfolio-tags">
      <span class="portfolio-tag">标签1</span>
      <span class="portfolio-tag">标签2</span>
    </div>
    <a href="GitHub链接" target="_blank" class="portfolio-link">查看 GitHub</a>
  </div>
</div>
```

### 修改菜单

编辑 [_config.next.yml](file:///workspace/hexo-portfolio/_config.next.yml) 的 `menu` 部分

---

## 6. 本地开发

```bash
cd /workspace/hexo-portfolio
npm install
npm run server
# 访问 http://localhost:4000
```

---

## 7. 下一步建议

1. 为 GitHub 仓库添加描述和主题（Topics）
2. 在 README 中添加项目截图
3. 补充个人联系方式
4. 部署到 GitHub Pages
