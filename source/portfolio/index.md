---
title: 作品集
date: 2024-01-01 00:00:00
type: portfolio
layout: page
comments: false
---

## 开源项目

{% raw %}
<style>
.portfolio-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 24px;
  margin: 30px 0;
}
.portfolio-card {
  background: var(--card-bg, #fff);
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 2px 12px rgba(0,0,0,0.08);
  transition: transform 0.3s, box-shadow 0.3s;
}
.portfolio-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 24px rgba(0,0,0,0.12);
}
.portfolio-image {
  width: 100%;
  height: 180px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 48px;
  color: #fff;
}
.portfolio-content {
  padding: 20px;
}
.portfolio-title {
  font-size: 18px;
  font-weight: 600;
  margin-bottom: 8px;
  color: var(--text-color, #333);
}
.portfolio-desc {
  font-size: 14px;
  color: #666;
  margin-bottom: 12px;
  line-height: 1.6;
}
.portfolio-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 6px;
  margin-bottom: 12px;
}
.portfolio-tag {
  background: #e8e8e8;
  padding: 4px 10px;
  border-radius: 20px;
  font-size: 12px;
  color: #555;
}
.portfolio-link {
  display: inline-block;
  color: #fff;
  background: #667eea;
  padding: 8px 16px;
  border-radius: 6px;
  text-decoration: none;
  font-size: 13px;
  transition: background 0.2s;
}
.portfolio-link:hover {
  background: #5a6fd6;
}
.github-stats {
  background: linear-gradient(135deg, #11998e 0%, #38ef7d 100%);
  border-radius: 12px;
  padding: 24px;
  margin: 30px 0;
  color: #fff;
  text-align: center;
}
.github-stats h3 {
  margin: 0 0 16px 0;
  font-size: 20px;
}
.stats-grid {
  display: flex;
  justify-content: center;
  gap: 40px;
}
.stat-item {
  text-align: center;
}
.stat-number {
  font-size: 32px;
  font-weight: 700;
}
.stat-label {
  font-size: 14px;
  opacity: 0.9;
}
</style>

<div class="github-stats">
  <h3>📊 GitHub 统计</h3>
  <div class="stats-grid">
    <div class="stat-item">
      <div class="stat-number">20</div>
      <div class="stat-label">仓库</div>
    </div>
    <div class="stat-item">
      <div class="stat-number">Vue.js / TS / Flutter</div>
      <div class="stat-label">主要技术栈</div>
    </div>
  </div>
</div>

<div class="portfolio-grid">
  <div class="portfolio-card">
    <div class="portfolio-image" style="background: linear-gradient(135deg, #42b983 0%, #35495e 100%);">🖥️</div>
    <div class="portfolio-content">
      <div class="portfolio-title">ERP Online</div>
      <div class="portfolio-desc">Vue3 企业资源规划系统，包含采购、销售、库存、财务等完整业务流程管理</div>
      <div class="portfolio-tags">
        <span class="portfolio-tag">Vue.js</span>
        <span class="portfolio-tag">Node.js</span>
        <span class="portfolio-tag">MySQL</span>
        <span class="portfolio-tag">ERP</span>
      </div>
      <a href="https://github.com/JinXuchen2020/erp_online" target="_blank" class="portfolio-link">查看 GitHub</a>
    </div>
  </div>

  <div class="portfolio-card">
    <div class="portfolio-image" style="background: linear-gradient(135deg, #2563eb 0%, #0f172a 100%);">🛒</div>
    <div class="portfolio-content">
      <div class="portfolio-title">Signples</div>
      <div class="portfolio-desc">Vue.js 购物商城系统，包含商品展示、购物车、订单管理等功能</div>
      <div class="portfolio-tags">
        <span class="portfolio-tag">Vue.js</span>
        <span class="portfolio-tag">JavaScript</span>
        <span class="portfolio-tag">SCSS</span>
        <span class="portfolio-tag">TypeScript</span>
      </div>
      <a href="https://github.com/JinXuchen2020/signples" target="_blank" class="portfolio-link">查看 GitHub</a>
    </div>
  </div>

  <div class="portfolio-card">
    <div class="portfolio-image" style="background: linear-gradient(135deg, #13b9f6 0%, #0553b1 100%);">💰</div>
    <div class="portfolio-content">
      <div class="portfolio-title">DAPA Zodiac Wallet</div>
      <div class="portfolio-desc">基于 Flutter 和 Rust 的跨平台数字钱包应用，支持多平台运行</div>
      <div class="portfolio-tags">
        <span class="portfolio-tag">Flutter</span>
        <span class="portfolio-tag">Dart</span>
        <span class="portfolio-tag">Rust</span>
        <span class="portfolio-tag">C++</span>
      </div>
      <a href="https://github.com/JinXuchen2020/dapa-zodiac-wallet" target="_blank" class="portfolio-link">查看 GitHub</a>
    </div>
  </div>

  <div class="portfolio-card">
    <div class="portfolio-image" style="background: linear-gradient(135deg, #000000 0%, #333333 100%);">🎬</div>
    <div class="portfolio-content">
      <div class="portfolio-title">Anchor Movie Review</div>
      <div class="portfolio-desc">现代影评应用，基于 T3 Stack 构建，包含用户评论、评分系统等功能</div>
      <div class="portfolio-tags">
        <span class="portfolio-tag">TypeScript</span>
        <span class="portfolio-tag">Next.js</span>
        <span class="portfolio-tag">Rust</span>
        <span class="portfolio-tag">tRPC</span>
      </div>
      <a href="https://github.com/JinXuchen2020/anchor-movie-review" target="_blank" class="portfolio-link">查看 GitHub</a>
    </div>
  </div>

  <div class="portfolio-card">
    <div class="portfolio-image" style="background: linear-gradient(135deg, #e44d26 0%, #f26522 100%);">📦</div>
    <div class="portfolio-content">
      <div class="portfolio-title">ZXBDM Inventory Server</div>
      <div class="portfolio-desc">ZXBDM 库存管理系统后端服务，提供库存管理相关 API 接口</div>
      <div class="portfolio-tags">
        <span class="portfolio-tag">TypeScript</span>
        <span class="portfolio-tag">Node.js</span>
        <span class="portfolio-tag">EJS</span>
      </div>
      <a href="https://github.com/JinXuchen2020/zxbdm-inventory-server" target="_blank" class="portfolio-link">查看 GitHub</a>
    </div>
  </div>
</div>
{% endraw %}

---

## 更多项目

> 💡 查看全部 20 个 GitHub 仓库：<https://github.com/JinXuchen2020?tab=repositories>

---

## 项目流程

| 阶段 | 说明 |
|------|------|
| 需求沟通 | 了解项目背景、功能需求、预算周期 |
| 方案报价 | 提供技术方案与详细报价单 |
| 合同签订 | 签署开发合同，预付定金 |
| 开发执行 | 阶段性交付，及时反馈进度 |
| 验收交付 | 功能测试，上线部署 |
| 售后服务 | Bug修复，技术支持 |

---

> 💡 **提示**：如需查看更多案例或讨论项目需求，请通过 [联系方式](/me/contact/) 与我取得联系
