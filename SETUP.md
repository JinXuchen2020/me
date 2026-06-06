# 项目配置指南

## 快速开始

### 1. 替换联系信息

在 [`source/contact/index.md`](file:///workspace/hexo-portfolio/source/contact/index.md) 中找到以下内容并替换：

| 占位符 | 说明 |
|--------|------|
| `jinxuchen2020@email.com` | 你的真实邮箱 |
| `jinxuchen2020` | 你的微信号 |
| `138-xxxx-xxxx` | 你的手机号 |
| `https://github.com/JinXuchen2020` | 你的GitHub链接 |
| `your-form-id` | Formspree 表单ID（见下方注册） |

---

### 2. 注册 Formspree（可选，用于接收表单咨询）

1. 访问 [formspree.io](https://formspree.io/) 免费注册
2. 验证邮箱后创建一个新表单
3. 获得表单ID（URL中的部分，例如 `f/xyz123abc`）
4. 替换 [`source/contact/index.md`](file:///workspace/hexo-portfolio/source/contact/index.md) 中的 `your-form-id`

---

### 3. 更新作品集内容

编辑 [`source/portfolio/index.md`](file:///workspace/hexo-portfolio/source/portfolio/index.md)：

- 修改项目标题、描述和标签
- 将图片（如果有）替换为真实项目截图
- 链接改为项目的真实地址或 GitHub 仓库

---

### 4. 更新服务项目

编辑 [`source/services/index.md`](file:///workspace/hexo-portfolio/source/services/index.md)：

- 根据你实际的技术能力调整技术栈和熟练度
- 修改服务项目描述

---

## 开发与部署

### 本地开发

```bash
cd /workspace/hexo-portfolio
pnpm install
pnpm run server
```

访问 http://localhost:4000

### 部署到 GitHub Pages

```bash
pnpm run clean
pnpm run build
pnpm run deploy
```

---

## 修改菜单图标（可选）

编辑 [`_config.next.yml`](file:///workspace/hexo-portfolio/_config.next.yml) 的 `menu` 部分，图标使用 [Font Awesome 4.7](https://fontawesome.com/v4/icons/)

---

## 修改主题配色（可选）

NexT 主题支持定制配色，详见 [NexT 文档](https://theme-next.js.org/docs/theme-settings/)
