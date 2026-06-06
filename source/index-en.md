---
title: Home
layout: page
comments: false
permalink: /en/
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
  <a href="/me/">中文</a> · <strong>English</strong>
</div>

<div class="hero-section">
  <h1>Full-Stack Developer</h1>
  <p>Specialized in providing high-quality software outsourcing services</p>
  <div class="hero-cta">
    <a href="/me/en/portfolio/" class="hero-btn hero-btn-primary">View Portfolio</a>
    <a href="/me/en/contact/" class="hero-btn hero-btn-secondary">Start Project</a>
  </div>
</div>

## About Me

<div class="about-section">
  <div class="about-content">
    <div class="about-avatar">👨‍💻</div>
    <div class="about-text">
      <h3>Hello, I'm JinXuchen2020 👋</h3>
      <p>I'm a full-stack engineer with over 5 years of development experience, specializing in modern tech stacks like Vue.js, React, and Node.js.</p>
      <p>I love coding and pursue high-quality code and excellent user experience. I've completed over 20 open source projects and excel in the complete development process from requirements analysis to product delivery.</p>
      <p>Whether it's web development, mobile apps, or backend systems, I can provide professional solutions for you.</p>
    </div>
  </div>
</div>

## Services

I provide the following professional technical services to deliver the best solutions for your project needs.

<div class="highlights">
  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 24px;">
    <div class="highlight-card">
      <div class="highlight-icon">🖥️</div>
      <div class="highlight-title">Web Development</div>
      <p>Vue.js, React and other modern frameworks for high-performance websites</p>
    </div>
    <div class="highlight-card">
      <div class="highlight-icon">📱</div>
      <div class="highlight-title">Mobile Apps</div>
      <p>Flutter cross-platform apps supporting both iOS and Android</p>
    </div>
    <div class="highlight-card">
      <div class="highlight-icon">⚙️</div>
      <div class="highlight-title">Backend Services</div>
      <p>Node.js, RESTful APIs for stable and efficient backend systems</p>
    </div>
  </div>
</div>

## Featured Projects

Showcasing my best open source projects. View more in portfolio.

<div class="featured-projects">
  <div class="project-grid">
    <div class="project-card">
      <div class="project-image" style="background: linear-gradient(135deg, #42b983 0%, #35495e 100%);">🖥️</div>
      <div class="project-content">
        <div class="project-title">ERP Online</div>
        <div class="project-desc">Vue3 Enterprise Resource Management system with procurement, sales, inventory, and finance modules</div>
        <a href="https://github.com/JinXuchen2020/erp_online" target="_blank" class="project-link">View Project →</a>
      </div>
    </div>
    <div class="project-card">
      <div class="project-image" style="background: linear-gradient(135deg, #2563eb 0%, #0f172a 100%);">🛒</div>
      <div class="project-content">
        <div class="project-title">Signples</div>
        <div class="project-desc">Vue.js e-commerce mall system with product display, shopping cart, and order management</div>
        <a href="https://github.com/JinXuchen2020/signples" target="_blank" class="project-link">View Project →</a>
      </div>
    </div>
    <div class="project-card">
      <div class="project-image" style="background: linear-gradient(135deg, #13b9f6 0%, #0553b1 100%);">💎</div>
      <div class="project-content">
        <div class="project-title">DAPA Zodiac Wallet</div>
        <div class="project-desc">Flutter + Rust cross-platform digital wallet application</div>
        <a href="https://github.com/JinXuchen2020/dapa-zodiac-wallet" target="_blank" class="project-link">View Project →</a>
      </div>
    </div>
  </div>
</div>

## Tech Stack

I'm proficient in the following technologies to provide comprehensive technical support for your projects.

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

## Project Statistics

Showcasing my technical capabilities through open source projects on GitHub.

<div class="stats">
  <div class="stat-card">
    <div class="stat-number">20+</div>
    <div class="stat-label">Open Source Projects</div>
  </div>
  <div class="stat-card">
    <div class="stat-number">5+</div>
    <div class="stat-label">Years of Experience</div>
  </div>
  <div class="stat-card">
    <div class="stat-number">100%</div>
    <div class="stat-label">Client Satisfaction</div>
  </div>
</div>

## Collaboration Process

Clear and transparent collaboration process you can trust.

<div class="process-section">
  <div class="process-steps">
    <div class="process-step">
      <div class="step-number">1</div>
      <div class="step-title">Requirements</div>
      <div class="step-desc">Understand your project background, specific needs, and expectations</div>
    </div>
    <div class="process-step">
      <div class="step-number">2</div>
      <div class="step-title">Proposal</div>
      <div class="step-desc">Provide technical solution with detailed quote and timeline</div>
    </div>
    <div class="process-step">
      <div class="step-number">3</div>
      <div class="step-title">Contract</div>
      <div class="step-desc">Sign development contract after confirming the proposal</div>
    </div>
    <div class="process-step">
      <div class="step-number">4</div>
      <div class="step-title">Development</div>
      <div class="step-desc">Phased development, timely communication, on-time delivery</div>
    </div>
    <div class="process-step">
      <div class="step-number">5</div>
      <div class="step-title">Support</div>
      <div class="step-desc">Testing, deployment, and ongoing technical support</div>
    </div>
  </div>
</div>

## Ready to Start?

Feel free to contact me for any project needs.

<div class="contact-cta">
  <h2>Let's Work Together!</h2>
  <p>Tell me your project needs and I'll respond within 24 hours</p>
  <a href="/me/en/contact/" class="contact-cta-btn">Contact Me Now</a>
</div>

---

> 💡 **Welcome to collaborate!** Feel free to reach out via GitHub anytime.
{% endraw %}
