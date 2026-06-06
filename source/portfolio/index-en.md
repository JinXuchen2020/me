---
title: Portfolio
date: 2024-01-01 00:00:00
type: portfolio
layout: page
comments: false
permalink: /en/portfolio/
---

## Open Source Projects

{% raw %}
<style>
.lang-switcher {
  text-align: center;
  margin: 20px 0;
  padding: 10px;
  background: #f8f9fa;
  border-radius: 8px;
}

.lang-switcher a {
  color: #667eea;
  text-decoration: none;
  font-weight: 600;
  padding: 8px 16px;
  border-radius: 4px;
  transition: background 0.2s;
}

.lang-switcher a:hover {
  background: #667eea;
  color: white;
}

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

<div class="lang-switcher">
  <a href="/portfolio/">中文</a> · <strong>English</strong>
</div>

<div class="github-stats">
  <h3>📊 GitHub Statistics</h3>
  <div class="stats-grid">
    <div class="stat-item">
      <div class="stat-number">20</div>
      <div class="stat-label">Repositories</div>
    </div>
    <div class="stat-item">
      <div class="stat-number">Vue.js / TS / Flutter</div>
      <div class="stat-label">Main Tech Stack</div>
    </div>
  </div>
</div>

<div class="portfolio-grid">
  <div class="portfolio-card">
    <div class="portfolio-image" style="background: linear-gradient(135deg, #42b983 0%, #35495e 100%);">🖥️</div>
    <div class="portfolio-content">
      <div class="portfolio-title">ERP Online</div>
      <div class="portfolio-desc">Vue3 Enterprise Resource Planning system with complete business process management including procurement, sales, inventory, and finance</div>
      <div class="portfolio-tags">
        <span class="portfolio-tag">Vue.js</span>
        <span class="portfolio-tag">Node.js</span>
        <span class="portfolio-tag">MySQL</span>
        <span class="portfolio-tag">ERP</span>
      </div>
      <a href="https://github.com/JinXuchen2020/erp_online" target="_blank" class="portfolio-link">View on GitHub</a>
    </div>
  </div>

  <div class="portfolio-card">
    <div class="portfolio-image" style="background: linear-gradient(135deg, #2563eb 0%, #0f172a 100%);">🛒</div>
    <div class="portfolio-content">
      <div class="portfolio-title">Signples</div>
      <div class="portfolio-desc">Vue.js shopping mall system with product display, shopping cart, and order management features</div>
      <div class="portfolio-tags">
        <span class="portfolio-tag">Vue.js</span>
        <span class="portfolio-tag">JavaScript</span>
        <span class="portfolio-tag">SCSS</span>
        <span class="portfolio-tag">TypeScript</span>
      </div>
      <a href="https://github.com/JinXuchen2020/signples" target="_blank" class="portfolio-link">View on GitHub</a>
    </div>
  </div>

  <div class="portfolio-card">
    <div class="portfolio-image" style="background: linear-gradient(135deg, #13b9f6 0%, #0553b1 100%);">💰</div>
    <div class="portfolio-content">
      <div class="portfolio-title">DAPA Zodiac Wallet</div>
      <div class="portfolio-desc">Cross-platform digital wallet app built with Flutter and Rust, supporting multiple platforms</div>
      <div class="portfolio-tags">
        <span class="portfolio-tag">Flutter</span>
        <span class="portfolio-tag">Dart</span>
        <span class="portfolio-tag">Rust</span>
        <span class="portfolio-tag">C++</span>
      </div>
      <a href="https://github.com/JinXuchen2020/dapa-zodiac-wallet" target="_blank" class="portfolio-link">View on GitHub</a>
    </div>
  </div>

  <div class="portfolio-card">
    <div class="portfolio-image" style="background: linear-gradient(135deg, #000000 0%, #333333 100%);">🎬</div>
    <div class="portfolio-content">
      <div class="portfolio-title">Anchor Movie Review</div>
      <div class="portfolio-desc">Modern movie review app built with T3 Stack, featuring user reviews and rating systems</div>
      <div class="portfolio-tags">
        <span class="portfolio-tag">TypeScript</span>
        <span class="portfolio-tag">Next.js</span>
        <span class="portfolio-tag">Rust</span>
        <span class="portfolio-tag">tRPC</span>
      </div>
      <a href="https://github.com/JinXuchen2020/anchor-movie-review" target="_blank" class="portfolio-link">View on GitHub</a>
    </div>
  </div>

  <div class="portfolio-card">
    <div class="portfolio-image" style="background: linear-gradient(135deg, #e44d26 0%, #f26522 100%);">📦</div>
    <div class="portfolio-content">
      <div class="portfolio-title">ZXBDM Inventory Server</div>
      <div class="portfolio-desc">ZXBDM Inventory Management System backend service providing inventory management API</div>
      <div class="portfolio-tags">
        <span class="portfolio-tag">TypeScript</span>
        <span class="portfolio-tag">Node.js</span>
        <span class="portfolio-tag">EJS</span>
      </div>
      <a href="https://github.com/JinXuchen2020/zxbdm-inventory-server" target="_blank" class="portfolio-link">View on GitHub</a>
    </div>
  </div>
</div>
{% endraw %}

---

## More Projects

> 💡 View all 20 GitHub repositories: <https://github.com/JinXuchen2020?tab=repositories>

---

## Project Process

| Stage | Description |
|-------|-------------|
| Requirements | Understand project background, requirements, budget, and timeline |
| Proposal | Provide technical solution and detailed quotation |
| Contract | Sign development contract with deposit payment |
| Development | Deliver in phases with timely progress updates |
| Acceptance | Testing and deployment |
| Support | Bug fixes and technical support |

---

> 💡 **Tip**: For more case studies or to discuss your project requirements, please [contact me](/en/contact/)
