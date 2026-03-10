---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<style>
:root {
  --main-color: #2563eb;
  --main-dark: #1d4ed8;
  --main-light: #3b82f6;
  --soft-bg: #f8fafc;
  --card-bg: #ffffff;
  --hero-bg-start: #eff6ff;
  --hero-bg-end: #dbeafe;
  --border-light: #e2e8f0;
  --border-mid: #cbd5e1;
  --text-main: #1e293b;
  --text-soft: #475569;
  --shadow-soft: 0 8px 24px rgba(37, 99, 235, 0.08);
  --shadow-hover: 0 14px 32px rgba(37, 99, 235, 0.12);
  --radius-lg: 22px;
  --radius-md: 18px;
  --radius-sm: 14px;
}

.page__content {
  font-size: 17px;
  line-height: 1.85;
  color: var(--text-main);
}

.page__content a {
  color: var(--main-color);
  text-decoration: none;
}

.page__content a:hover {
  text-decoration: underline;
}

/* ===== Language Toggle ===== */
.lang-toggle {
  position: fixed;
  top: 80px;
  right: 20px;
  z-index: 1000;
  display: flex;
  gap: 4px;
  background: #fff;
  border-radius: 999px;
  padding: 4px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
  border: 1px solid var(--border-light);
}

.lang-btn {
  padding: 8px 16px;
  border-radius: 999px;
  border: none;
  background: transparent;
  color: var(--text-soft);
  font-weight: 600;
  cursor: pointer;
  transition: all 0.2s ease;
  font-size: 0.9rem;
}

.lang-btn:hover {
  color: var(--main-color);
}

.lang-btn.active {
  background: var(--main-color);
  color: #fff;
}

/* ===== Hero ===== */
.hero-card {
  position: relative;
  overflow: hidden;
  background: linear-gradient(135deg, var(--hero-bg-start) 0%, var(--hero-bg-end) 100%);
  border: 1px solid var(--border-light);
  border-radius: 26px;
  padding: 34px 38px 30px 38px;
  margin-bottom: 18px;
  box-shadow: var(--shadow-soft);
}

.hero-card::after {
  content: "";
  position: absolute;
  right: -80px;
  top: -80px;
  width: 220px;
  height: 220px;
  border-radius: 50%;
  background: radial-gradient(circle, rgba(37, 99, 235, 0.12) 0%, rgba(37, 99, 235, 0.03) 55%, rgba(37, 99, 235, 0) 72%);
  pointer-events: none;
}

.hero-title {
  margin: 0 0 10px 0;
  font-size: 2.2rem;
  font-weight: 800;
  line-height: 1.25;
  color: var(--text-main);
}

.hero-subtitle {
  display: inline-block;
  margin-bottom: 18px;
  padding: 6px 14px;
  border-radius: 999px;
  background: #dbeafe;
  border: 1px solid #93c5fd;
  color: var(--main-dark);
  font-size: 0.96rem;
  font-weight: 700;
}

.hero-card p {
  margin: 0 0 14px 0;
  font-size: 1.05rem;
  color: var(--text-main);
}

.hero-email {
  font-weight: 700;
  color: var(--main-dark);
}

/* ===== Quick Links ===== */
.home-links {
  display: flex;
  flex-wrap: wrap;
  gap: 14px;
  margin: 4px 0 34px 0;
}

.home-btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  padding: 10px 18px;
  border-radius: 999px;
  border: 1px solid var(--border-mid);
  background: #fff;
  color: var(--main-color) !important;
  font-weight: 700;
  text-decoration: none !important;
  box-shadow: 0 3px 10px rgba(0, 0, 0, 0.03);
  transition: all 0.22s ease;
}

.home-btn:hover {
  background: #eff6ff;
  border-color: var(--main-light);
  transform: translateY(-2px);
  box-shadow: 0 10px 20px rgba(37, 99, 235, 0.12);
  text-decoration: none !important;
}

.home-btn.primary {
  background: var(--main-color);
  color: #fff !important;
  border-color: var(--main-color);
}

.home-btn.primary:hover {
  background: var(--main-dark);
  border-color: var(--main-dark);
}

/* ===== Section Title ===== */
.section-title {
  display: flex;
  align-items: center;
  gap: 10px;
  font-size: 1.55rem;
  font-weight: 800;
  color: var(--text-main);
  margin: 36px 0 18px 0;
  padding-left: 14px;
  border-left: 5px solid var(--main-color);
}

/* ===== Skills Section ===== */
.skills-container {
  background: var(--card-bg);
  border: 1px solid var(--border-light);
  border-radius: var(--radius-md);
  padding: 24px;
  box-shadow: var(--shadow-soft);
}

.skill-category {
  margin-bottom: 20px;
}

.skill-category:last-child {
  margin-bottom: 0;
}

.skill-category-title {
  font-size: 1rem;
  font-weight: 700;
  color: var(--main-color);
  margin-bottom: 12px;
}

.skill-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}

.skill-tag {
  display: inline-flex;
  align-items: center;
  padding: 7px 14px;
  border-radius: 999px;
  background: #eff6ff;
  border: 1px solid #bfdbfe;
  color: var(--main-dark);
  font-size: 0.9rem;
  font-weight: 600;
  transition: all 0.2s ease;
}

.skill-tag:hover {
  background: #dbeafe;
  border-color: #93c5fd;
}

/* ===== Projects Grid ===== */
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 22px;
}

.project-card {
  background: var(--card-bg);
  border: 1px solid var(--border-light);
  border-radius: var(--radius-md);
  padding: 22px;
  box-shadow: var(--shadow-soft);
  transition: transform 0.22s ease, box-shadow 0.22s ease, border-color 0.22s ease;
}

.project-card:hover {
  transform: translateY(-4px);
  box-shadow: var(--shadow-hover);
  border-color: #93c5fd;
}

.project-card h3 {
  margin: 0 0 10px 0;
  color: var(--main-color);
  font-size: 1.15rem;
  line-height: 1.4;
}

.project-card p {
  margin: 0 0 14px 0;
  color: var(--text-soft);
  font-size: 0.95rem;
}

.project-tech {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin-bottom: 14px;
}

.project-tech-tag {
  padding: 4px 10px;
  border-radius: 999px;
  background: #f1f5f9;
  border: 1px solid #e2e8f0;
  color: var(--text-soft);
  font-size: 0.82rem;
  font-weight: 600;
}

.project-links {
  display: flex;
  gap: 10px;
}

.project-link {
  display: inline-flex;
  align-items: center;
  padding: 6px 12px;
  border-radius: 999px;
  background: var(--main-color);
  color: #fff !important;
  font-size: 0.85rem;
  font-weight: 600;
  text-decoration: none !important;
  transition: all 0.2s ease;
}

.project-link:hover {
  background: var(--main-dark);
}

.project-link.secondary {
  background: #fff;
  color: var(--main-color) !important;
  border: 1px solid var(--main-color);
}

.project-link.secondary:hover {
  background: #eff6ff;
}

/* ===== Experience Timeline ===== */
.experience-timeline {
  position: relative;
  margin-top: 4px;
  padding-left: 26px;
  border-left: 3px solid #bfdbfe;
}

.experience-item {
  position: relative;
  margin-bottom: 28px;
  padding: 0 0 0 10px;
}

.experience-item:last-child {
  margin-bottom: 0;
}

.experience-item::before {
  content: "";
  position: absolute;
  left: -35px;
  top: 8px;
  width: 14px;
  height: 14px;
  border-radius: 50%;
  background: var(--main-color);
  box-shadow: 0 0 0 4px #eff6ff;
}

.experience-title {
  font-size: 1.1rem;
  font-weight: 700;
  color: var(--text-main);
  margin-bottom: 4px;
}

.experience-subtitle {
  font-size: 0.95rem;
  color: var(--main-color);
  font-weight: 600;
  margin-bottom: 4px;
}

.experience-period {
  font-size: 0.9rem;
  color: var(--text-soft);
  margin-bottom: 8px;
}

.experience-desc {
  color: var(--text-main);
  font-size: 0.95rem;
  margin: 0;
}

/* ===== Blog List ===== */
.blog-list {
  display: flex;
  flex-direction: column;
  gap: 14px;
}

.blog-card {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 16px 20px;
  background: var(--card-bg);
  border: 1px solid var(--border-light);
  border-radius: var(--radius-sm);
  transition: all 0.22s ease;
}

.blog-card:hover {
  border-color: #93c5fd;
  box-shadow: var(--shadow-soft);
}

.blog-info {
  flex: 1;
}

.blog-title {
  font-size: 1rem;
  font-weight: 600;
  color: var(--text-main);
  margin-bottom: 4px;
}

.blog-meta {
  font-size: 0.85rem;
  color: var(--text-soft);
}

.blog-platform {
  display: inline-flex;
  align-items: center;
  padding: 4px 10px;
  border-radius: 999px;
  background: #f1f5f9;
  border: 1px solid #e2e8f0;
  color: var(--text-soft);
  font-size: 0.8rem;
  font-weight: 600;
}

/* ===== GitHub Stats ===== */
.github-stats {
  background: var(--card-bg);
  border: 1px solid var(--border-light);
  border-radius: var(--radius-md);
  padding: 24px;
  box-shadow: var(--shadow-soft);
  text-align: center;
}

.github-stats-img {
  max-width: 100%;
  height: auto;
  border-radius: var(--radius-sm);
  margin-bottom: 16px;
}

.github-stats-img:last-child {
  margin-bottom: 0;
}

/* ===== Contact Section ===== */
.contact-section {
  background: var(--card-bg);
  border: 1px solid var(--border-light);
  border-radius: var(--radius-md);
  padding: 24px;
  box-shadow: var(--shadow-soft);
}

.contact-links {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  margin-top: 16px;
}

.contact-btn {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  padding: 10px 18px;
  border-radius: 999px;
  background: #fff;
  border: 1px solid var(--border-mid);
  color: var(--text-main) !important;
  font-weight: 600;
  text-decoration: none !important;
  transition: all 0.22s ease;
}

.contact-btn:hover {
  background: #eff6ff;
  border-color: var(--main-light);
  text-decoration: none !important;
}

.contact-btn.primary {
  background: var(--main-color);
  color: #fff !important;
  border-color: var(--main-color);
}

.contact-btn.primary:hover {
  background: var(--main-dark);
}

/* ===== Responsive ===== */
@media (max-width: 768px) {
  .lang-toggle {
    top: 10px;
    right: 10px;
  }

  .lang-btn {
    padding: 6px 12px;
    font-size: 0.85rem;
  }

  .hero-card {
    padding: 26px 22px;
  }

  .hero-title {
    font-size: 1.8rem;
  }

  .page__content {
    font-size: 16px;
  }

  .section-title {
    font-size: 1.35rem;
  }

  .projects-grid {
    grid-template-columns: 1fr;
  }

  .blog-card {
    flex-direction: column;
    align-items: flex-start;
    gap: 10px;
  }
}
</style>

<!-- Language Toggle Button -->
<div class="lang-toggle">
  <button class="lang-btn active" data-lang="en" onclick="switchLanguage('en')">EN</button>
  <button class="lang-btn" data-lang="zh" onclick="switchLanguage('zh')">中文</button>
</div>

<!-- Hero Section -->
<div class="hero-card">
  <div class="hero-subtitle" data-i18n="bio">Research Interests: VLM, LLM, Motion Planning</div>

  <h1 class="hero-title">
    <span data-i18n="greeting">Hello, I am</span> <strong>Huang Zhenwei (黄圳炜)</strong>
  </h1>

  <p data-i18n="intro">
    I am currently a Master's student passionate about AI research, focusing on Vision-Language Models, Large Language Models, and Motion Planning.
  </p>

  <p>
    <span data-i18n="contact_prompt">If you are interested in collaboration, please contact me via email:</span>
    <span class="hero-email">12532510@mail.sustech.edu.cn</span>
  </p>
</div>

<div class="home-links">
  <a class="home-btn primary" href="mailto:12532510@mail.sustech.edu.cn" data-i18n="email_me">Email Me</a>
  <a class="home-btn" href="https://github.com/Enei7" target="_blank">GitHub</a>
  <a class="home-btn" href="#projects" data-i18n="projects">Projects</a>
  <a class="home-btn" href="#contact" data-i18n="contact">Contact</a>
  <a class="home-btn" href="/Photos.html" data-i18n="photos">Photos</a>
</div>

<!-- Education Section -->
<div class="section-title" data-i18n="education">Education</div>

<div class="experience-timeline">
  <div class="experience-item">
    <div class="experience-title"><span data-i18n="sustech">Southern University of Science and Technology (SUSTech)</span></div>
    <div class="experience-subtitle"><span data-i18n="sustech_degree">M.Eng. in Electronic Science and Technology</span></div>
    <div class="experience-period"><span data-i18n="sustech_period">Shenzhen, China | Sep. 2025 - Present (expected Jun. 2028)</span></div>
    <p class="experience-desc"><span data-i18n="sustech_desc">Admitted through Postgraduate Recommendation. Research focus on AI and Robotics.</span></p>
  </div>
  <div class="experience-item">
    <div class="experience-title"><span data-i18n="gdut">Guangdong University of Technology (GDUT)</span></div>
    <div class="experience-subtitle"><span data-i18n="gdut_degree">B.Eng. in Information Engineering (Excellence Class)</span></div>
    <div class="experience-period"><span data-i18n="gdut_period">Guangzhou, China | Sep. 2021 - Jun. 2025</span></div>
    <p class="experience-desc"><span data-i18n="gdut_desc">Undergraduate studies. CET & CET-6 Certified.</span></p>
  </div>
</div>

<!-- Projects Section -->
<span id="projects"></span>
<div class="section-title" data-i18n="projects">Projects</div>

<div class="projects-grid">
  <div class="project-card">
    <h3 data-i18n="project1_name">Project One</h3>
    <p data-i18n="project1_desc">A brief description of the project. What it does and the problem it solves.</p>
    <div class="project-tech">
      <span class="project-tech-tag">PyTorch</span>
      <span class="project-tech-tag">Python</span>
    </div>
    <div class="project-links">
      <a href="#" class="project-link" target="_blank">GitHub</a>
    </div>
  </div>

  <div class="project-card">
    <h3 data-i18n="project2_name">Project Two</h3>
    <p data-i18n="project2_desc">Another project description. Highlight key features and technologies used.</p>
    <div class="project-tech">
      <span class="project-tech-tag">ROS</span>
      <span class="project-tech-tag">C++</span>
    </div>
    <div class="project-links">
      <a href="#" class="project-link" target="_blank">GitHub</a>
    </div>
  </div>
</div>

<!-- Research Interests -->
<div class="section-title" data-i18n="research_interests">Research Interests</div>

<div class="skills-container">
  <div class="skill-tags">
    <span class="skill-tag">Vision-Language Models (VLM)</span>
    <span class="skill-tag">Large Language Models (LLM)</span>
    <span class="skill-tag">Motion Planning</span>
    <span class="skill-tag">Embodied AI</span>
    <span class="skill-tag">Robotics</span>
  </div>
</div>

<!-- Skills Section -->
<div class="section-title" data-i18n="skills">Technical Skills</div>

<div class="skills-container">
  <div class="skill-category">
    <div class="skill-category-title" data-i18n="programming_languages">Programming Languages</div>
    <div class="skill-tags">
      <span class="skill-tag">Python</span>
      <span class="skill-tag">C++</span>
      <span class="skill-tag">JavaScript</span>
      <span class="skill-tag">TypeScript</span>
    </div>
  </div>

  <div class="skill-category">
    <div class="skill-category-title" data-i18n="frameworks">Frameworks & Libraries</div>
    <div class="skill-tags">
      <span class="skill-tag">PyTorch</span>
      <span class="skill-tag">TensorFlow</span>
      <span class="skill-tag">Transformers</span>
      <span class="skill-tag">ROS</span>
      <span class="skill-tag">OpenCV</span>
    </div>
  </div>

  <div class="skill-category">
    <div class="skill-category-title" data-i18n="tools">Tools & Platforms</div>
    <div class="skill-tags">
      <span class="skill-tag">Git</span>
      <span class="skill-tag">Docker</span>
      <span class="skill-tag">Linux</span>
      <span class="skill-tag">CUDA</span>
      <span class="skill-tag">AWS</span>
    </div>
  </div>
</div>

<!-- GitHub Stats Section -->
<div class="section-title" data-i18n="github_stats">GitHub Statistics</div>

<div class="github-stats">
  <img class="github-stats-img" src="https://github-readme-stats.vercel.app/api?username=Enei7&show_icons=true&theme=default&hide_border=true&bg_color=ffffff&title_color=2563eb&icon_color=2563eb&text_color=1e293b" alt="GitHub Stats" loading="lazy" />
  <img class="github-stats-img" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Enei7&layout=compact&hide_border=true&bg_color=ffffff&title_color=2563eb&text_color=1e293b" alt="Top Languages" loading="lazy" />
</div>

<!-- Contact Section -->
<span id="contact"></span>
<div class="section-title" data-i18n="contact">Contact Me</div>

<div class="contact-section">
  <p data-i18n="contact_intro">I'm always open to discussing new opportunities, interesting projects, or potential collaborations.</p>

  <div class="contact-links">
    <a class="contact-btn primary" href="mailto:12532510@mail.sustech.edu.cn">
      <i class="fas fa-envelope"></i> <span data-i18n="email_me">Email Me</span>
    </a>
    <a class="contact-btn" href="https://github.com/Enei7" target="_blank">
      <i class="fab fa-github"></i> GitHub
    </a>
  </div>
</div>

<!-- Language Switch Script -->
<script>
const translations = {
  en: {
    bio: "Research Interests: VLM, LLM, Motion Planning",
    greeting: "Hello, I am",
    intro: "I am currently a Master's student passionate about AI research, focusing on Vision-Language Models, Large Language Models, and Motion Planning. I welcome academic collaboration and discussion. If you have internship or job opportunities, please feel free to contact me.",
    contact_prompt: "If you are interested in collaboration, please contact me via email:",
    email_me: "Email Me",
    projects: "Projects",
    contact: "Contact",
    photos: "Photos",
    research_interests: "Research Interests",
    skills: "Technical Skills",
    programming_languages: "Programming Languages",
    frameworks: "Frameworks & Libraries",
    tools: "Tools & Platforms",
    education: "Education",
    degree: "Bachelor's Degree",
    edu_desc: "Research focus on AI and Robotics.",
    sustech: "Southern University of Science and Technology (SUSTech)",
    sustech_degree: "M.Eng. in Electronic Science and Technology",
    sustech_period: "Shenzhen, China | Sep. 2025 - Present (expected Jun. 2028)",
    sustech_desc: "Admitted through Postgraduate Recommendation. Research focus on AI and Robotics.",
    gdut: "Guangdong University of Technology (GDUT)",
    gdut_degree: "B.Eng. in Information Engineering (Excellence Class)",
    gdut_period: "Guangzhou, China | Sep. 2021 - Jun. 2025",
    gdut_desc: "Undergraduate studies. CET & CET-6 Certified.",
    github_stats: "GitHub Statistics",
    contact_intro: "I'm always open to discussing new opportunities, interesting projects, or potential collaborations.",
    project1_name: "Project One",
    project1_desc: "A brief description of the project. What it does and the problem it solves.",
    project2_name: "Project Two",
    project2_desc: "Another project description. Highlight key features and technologies used."
  },
  zh: {
    bio: "研究兴趣：VLM, LLM, 运动规划",
    greeting: "你好，我是",
    intro: "我是一名在读硕士研究生，专注于人工智能研究，研究方向包括视觉语言模型、大语言模型和运动规划。欢迎学术合作与交流，如有实习或工作机会，欢迎与我联系。",
    contact_prompt: "如果您对合作感兴趣，请通过邮件联系我：",
    email_me: "发送邮件",
    projects: "项目",
    contact: "联系",
    photos: "照片",
    research_interests: "研究兴趣",
    skills: "技术技能",
    programming_languages: "编程语言",
    frameworks: "框架与库",
    tools: "工具与平台",
    education: "教育背景",
    degree: "学士学位",
    edu_desc: "研究方向为人工智能与机器人。",
    sustech: "南方科技大学 (SUSTech)",
    sustech_degree: "电子科学与技术 工学硕士",
    sustech_period: "中国深圳 | 2025.09 - 至今 (预计2028.06毕业)",
    sustech_desc: "保研入学。研究方向：人工智能与机器人。",
    gdut: "广东工业大学 (GDUT)",
    gdut_degree: "信息工程 工学学士 (卓越班)",
    gdut_period: "中国广州 | 2021.09 - 2025.06",
    gdut_desc: "本科学习。通过大学英语四级和六级。",
    github_stats: "GitHub 统计",
    contact_intro: "欢迎与我讨论新的机会、有趣的项目或潜在的合作。",
    project1_name: "项目一",
    project1_desc: "项目简介。描述项目功能和解决的问题。",
    project2_name: "项目二",
    project2_desc: "另一个项目描述。突出关键特性和使用的技术。"
  }
};

function switchLanguage(lang) {
  // Update active button
  document.querySelectorAll('.lang-btn').forEach(btn => {
    btn.classList.remove('active');
    if (btn.dataset.lang === lang) {
      btn.classList.add('active');
    }
  });

  // Update all translatable elements
  document.querySelectorAll('[data-i18n]').forEach(el => {
    const key = el.dataset.i18n;
    if (translations[lang] && translations[lang][key]) {
      el.textContent = translations[lang][key];
    }
  });

  // Save preference
  localStorage.setItem('preferred-language', lang);
}

// Load saved language preference
document.addEventListener('DOMContentLoaded', function() {
  const savedLang = localStorage.getItem('preferred-language') || 'en';
  switchLanguage(savedLang);
});
</script>