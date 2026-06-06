---
title: 首页
layout: page
comments: false
permalink: /
---

{% raw %}
<style>
.hero-section {
  text-align: center;
  padding: 60px 20px;
  margin-bottom: 40px;
  border-radius: 16px;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
}

.hero-section h1 {
  font-size: 2.5rem;
  margin-bottom: 10px;
  color: white !important;
}

.hero-section p {
  font-size: 1.2rem;
  opacity: 0.9;
  margin-bottom: 30px;
  color: white !important;
}

.hero-cta {
  display: flex;
  gap: 16px;
  justify-content: center;
  flex-wrap: wrap;
}

.hero-btn {
  padding: 12px 30px;
  border-radius: 8px;
  text-decoration: none;
  font-weight: 600;
  transition: all 0.3s;
}

.hero-btn-primary {
  background: white;
  color: #667eea;
}

.hero-btn-primary:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(0,0,0,0.2);
}

.hero-btn-secondary {
  border: 2px solid white;
  color: white;
}

.hero-btn-secondary:hover {
  background: rgba(255,255,255,0.1);
}

.highlights {
  margin: 50px 0;
}

.highlight-card {
  background: #f8f9fa;
  border-radius: 12px;
  padding: 30px;
  text-align: center;
  transition: transform 0.3s;
}

.highlight-card:hover {
  transform: translateY(-5px);
}

.highlight-icon {
  font-size: 48px;
  margin-bottom: 16px;
}

.highlight-title {
  font-size: 20px;
  font-weight: 600;
  margin-bottom: 12px;
}

.tech-stack {
  margin: 50px 0;
}

.tech-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(100px, 1fr));
  gap: 16px;
}

.tech-item {
  background: #f8f9fa;
  border-radius: 8px;
  padding: 20px 10px;
  text-align: center;
  font-weight: 500;
}

.stats {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  gap: 24px;
  margin: 50px 0;
}

.stat-card {
  background: #f8f9fa;
  border-radius: 12px;
  padding: 30px 20px;
  text-align: center;
}

.stat-number {
  font-size: 36px;
  font-weight: 700;
  color: #667eea;
}

.stat-label {
  font-size: 14px;
  color: #666;
  margin-top: 8px;
}
</style>

<div class="hero-section">
  <h1>全栈开发工程师</h1>
  <p>专注于为企业提供高质量的软件外包服务</p>
  <div class="hero-cta">
    <a href="/me/portfolio/" class="hero-btn hero-btn-primary">查看作品</a>
    <a href="/me/contact/" class="hero-btn hero-btn-secondary">开始合作</a>
  </div>
</div>

## 服务介绍

我提供以下专业技术服务，为您的项目需求提供最佳解决方案。

<div class="highlights">
  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 24px;">
    <div class="highlight-card">
      <div class="highlight-icon">🖥️</div>
      <div class="highlight-title">Web 开发</div>
      <p>Vue.js、React 等现代框架，打造高性能网站</p>
    </div>
    <div class="highlight-card">
      <div class="highlight-icon">📱</div>
      <div class="highlight-title">移动应用</div>
      <p>Flutter 跨平台应用，同时支持 iOS 和 Android</p>
    </div>
    <div class="highlight-card">
      <div class="highlight-icon">⚙️</div>
      <div class="highlight-title">后端服务</div>
      <p>Node.js、RESTful API，稳定高效的后台系统</p>
    </div>
  </div>
</div>

## 技术栈

我熟练掌握以下技术，可以为您的项目提供全方位的技术支持。

<div class="tech-stack">
  <div class="tech-grid">
    <div class="tech-item">Vue.js</div>
    <div class="tech-item">React</div>
    <div class="tech-item">TypeScript</div>
    <div class="tech-item">Node.js</div>
    <div class="tech-item">Flutter</div>
    <div class="tech-item">MySQL</div>
    <div class="tech-item">MongoDB</div>
    <div class="tech-item">Python</div>
  </div>
</div>

## 项目统计

通过 GitHub 上的开源项目展示我的技术能力。

<div class="stats">
  <div class="stat-card">
    <div class="stat-number">20+</div>
    <div class="stat-label">开源项目</div>
  </div>
  <div class="stat-card">
    <div class="stat-number">5+</div>
    <div class="stat-label">开发年数</div>
  </div>
  <div class="stat-card">
    <div class="stat-number">100%</div>
    <div class="stat-label">客户满意度</div>
  </div>
</div>

## 快速导航

- 👉 [查看作品](/me/portfolio/)
- 📋 [服务介绍](/me/services/)
- 📧 [联系我](/me/contact/)

---

> 💡 **欢迎合作！** 无论您有什么项目需求，都欢迎随时联系我。
{% endraw %}
