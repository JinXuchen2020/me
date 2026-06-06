---
title: 首页
layout: page
comments: false
permalink: /
---

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

.about-section {
  background: #f8f9fa;
  border-radius: 16px;
  padding: 40px;
  margin: 40px 0;
}

.about-content {
  display: flex;
  gap: 30px;
  align-items: flex-start;
  flex-wrap: wrap;
}

.about-avatar {
  flex-shrink: 0;
  width: 120px;
  height: 120px;
  border-radius: 50%;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 48px;
  color: white;
}

.about-text {
  flex: 1;
  min-width: 280px;
}

.about-text h3 {
  margin-top: 0;
  color: #333;
}

.about-text p {
  color: #666;
  line-height: 1.8;
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

.featured-projects {
  margin: 50px 0;
}

.project-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 24px;
}

.project-card {
  background: #fff;
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 2px 12px rgba(0,0,0,0.08);
  transition: transform 0.3s, box-shadow 0.3s;
}

.project-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 24px rgba(0,0,0,0.12);
}

.project-image {
  width: 100%;
  height: 160px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 40px;
  color: #fff;
}

.project-content {
  padding: 20px;
}

.project-title {
  font-size: 18px;
  font-weight: 600;
  margin-bottom: 8px;
}

.project-desc {
  font-size: 14px;
  color: #666;
  margin-bottom: 12px;
  line-height: 1.6;
}

.project-link {
  display: inline-block;
  color: #667eea;
  text-decoration: none;
  font-size: 14px;
  font-weight: 500;
}

.project-link:hover {
  text-decoration: underline;
}

.process-section {
  background: linear-gradient(135deg, #667eea15 0%, #764ba215 100%);
  border-radius: 16px;
  padding: 40px;
  margin: 40px 0;
}

.process-steps {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 30px;
  margin-top: 30px;
}

.process-step {
  text-align: center;
}

.step-number {
  width: 48px;
  height: 48px;
  border-radius: 50%;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 20px;
  font-weight: 700;
  margin: 0 auto 16px;
}

.step-title {
  font-weight: 600;
  margin-bottom: 8px;
}

.step-desc {
  font-size: 14px;
  color: #666;
}

.contact-cta {
  text-align: center;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  border-radius: 16px;
  padding: 50px 30px;
  margin: 50px 0;
}

.contact-cta h2 {
  color: white !important;
  margin-top: 0;
}

.contact-cta p {
  color: white !important;
  opacity: 0.9;
  margin-bottom: 24px;
}

.contact-cta-btn {
  display: inline-block;
  background: white;
  color: #667eea;
  padding: 14px 40px;
  border-radius: 8px;
  text-decoration: none;
  font-weight: 600;
  transition: all 0.3s;
}

.contact-cta-btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(0,0,0,0.2);
}
</style>

<div class="lang-switcher">
  <strong>中文</strong> · <a href="/en/">English</a>
</div>

<div class="hero-section">
  <h1>全栈开发工程师</h1>
  <p>专注于为企业提供高质量的软件外包服务</p>
  <div class="hero-cta">
    <a href="/me/portfolio/" class="hero-btn hero-btn-primary">查看作品</a>
    <a href="/me/contact/" class="hero-btn hero-btn-secondary">开始合作</a>
  </div>
</div>

## 关于我

<div class="about-section">
  <div class="about-content">
    <div class="about-avatar">👨‍💻</div>
    <div class="about-text">
      <h3>你好，我是 JinXuchen2020 👋</h3>
      <p>我是一名拥有 5 年以上开发经验的全栈工程师，专注于 Vue.js、React、Node.js 等现代技术栈。</p>
      <p>我热爱编程，追求高质量的代码和优秀的用户体验。已完成 20 多个开源项目，擅长从需求分析到产品交付的完整开发流程。</p>
      <p>无论是网站开发、移动应用还是后端系统，我都能为您提供专业的解决方案。</p>
    </div>
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

## 精选项目

展示我最优秀的几个开源项目，更多请查看作品集。

<div class="featured-projects">
  <div class="project-grid">
    <div class="project-card">
      <div class="project-image" style="background: linear-gradient(135deg, #42b983 0%, #35495e 100%);">🖥️</div>
      <div class="project-content">
        <div class="project-title">ERP Online</div>
        <div class="project-desc">Vue3 企业资源管理系统，包含采购、销售、库存、财务等完整业务流程</div>
        <a href="https://github.com/JinXuchen2020/erp_online" target="_blank" class="project-link">查看项目 →</a>
      </div>
    </div>
    <div class="project-card">
      <div class="project-image" style="background: linear-gradient(135deg, #2563eb 0%, #0f172a 100%);">🛒</div>
      <div class="project-content">
        <div class="project-title">Signples</div>
        <div class="project-desc">Vue.js 电商商城系统，包含商品展示、购物车、订单管理等功能</div>
        <a href="https://github.com/JinXuchen2020/signples" target="_blank" class="project-link">查看项目 →</a>
      </div>
    </div>
    <div class="project-card">
      <div class="project-image" style="background: linear-gradient(135deg, #13b9f6 0%, #0553b1 100%);">💎</div>
      <div class="project-content">
        <div class="project-title">DAPA Zodiac Wallet</div>
        <div class="project-desc">Flutter + Rust 跨平台数字钱包应用</div>
        <a href="https://github.com/JinXuchen2020/dapa-zodiac-wallet" target="_blank" class="project-link">查看项目 →</a>
      </div>
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

## 合作流程

清晰透明的合作流程，让您放心。

<div class="process-section">
  <div class="process-steps">
    <div class="process-step">
      <div class="step-number">1</div>
      <div class="step-title">需求沟通</div>
      <div class="step-desc">了解您的项目背景、具体需求和期望</div>
    </div>
    <div class="process-step">
      <div class="step-number">2</div>
      <div class="step-title">方案报价</div>
      <div class="step-desc">提供技术方案和详细的报价与时间规划</div>
    </div>
    <div class="process-step">
      <div class="step-number">3</div>
      <div class="step-title">签订合同</div>
      <div class="step-desc">确认方案后签订开发合同，支付预付款</div>
    </div>
    <div class="process-step">
      <div class="step-number">4</div>
      <div class="step-title">开发交付</div>
      <div class="step-desc">分阶段开发，及时沟通，按时交付</div>
    </div>
    <div class="process-step">
      <div class="step-number">5</div>
      <div class="step-title">验收支持</div>
      <div class="step-desc">测试验收，部署上线，后续技术支持</div>
    </div>
  </div>
</div>

## 准备开始了？

无论您有什么项目需求，都欢迎随时联系我。

<div class="contact-cta">
  <h2>让我们一起合作吧！</h2>
  <p>告诉我您的项目需求，我会在 24 小时内回复您</p>
  <a href="/me/contact/" class="contact-cta-btn">立即联系我</a>
</div>

---

> 💡 **欢迎合作！** 随时可以通过 GitHub 与我联系。
{% endraw %}
