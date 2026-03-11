<template>
  <div class="page-container">
    <!-- 头部导航区 -->
    <header class="header">
      <div class="logo">游戏策划作品集</div>
      <nav class="nav">
        <a href="#home">首页</a>
        <a href="#projects">项目经历</a>
        <a href="#games">游戏经历</a>
        <a href="#skills">技能工具</a>
        <a href="#contact">联系我</a>
      </nav>
    </header>

    <!-- 主体内容区 -->
    <main class="main-content">
      <!-- 首页/简介区块 -->
      <section id="home" class="section home-section">
        <h1 class="title">Hi, 我是[你的名字]</h1>
        <p class="subtitle">游戏系统策划 | 深度玩家 | AI工具践行者</p>
        <div class="intro-text">
          擅长系统设计、用户体验优化与跨部门协作，拥有从0到1推动产品落地的完整经验。
        </div>
      </section>

      <!-- 项目经历区块（示例卡片布局） -->
      <section id="projects" class="section projects-section">
        <h2 class="section-title">项目经历</h2>
        <div class="cards-grid">
          <div class="project-card">
            <h3>口腔诊断可视化系统</h3>
            <p class="card-role">项目负责人</p>
            <p class="card-desc">主导从0到1全流程设计，负责核心系统架构与交互规划，系统已进入临床试运行。</p>
          </div>
          <div class="project-card">
            <h3>文博元宇宙</h3>
            <p class="card-role">交互策划 (UNITY)</p>
            <p class="card-desc">负责数字人导游交互场景设计，设计对话触发机制与互动反馈表现。</p>
          </div>
          <div class="project-card">
            <h3>3D打印虚拟工坊</h3>
            <p class="card-role">系统策划 (UNITY)</p>
            <p class="card-desc">负责核心玩法机制与操作逻辑设计，设计交互引导与错误反馈机制。</p>
          </div>
        </div>
      </section>

      <!-- 技能标签区块 -->
      <section id="skills" class="section skills-section">
        <h2 class="section-title">技能工具</h2>
        <div class="skills-tags">
          <span class="tag">系统策划</span>
          <span class="tag">交互设计</span>
          <span class="tag">UNITY基础</span>
          <span class="tag">Python</span>
          <span class="tag">ChatGPT/GPT-4</span>
          <span class="tag">Midjourney</span>
          <span class="tag">Runway/Pika</span>
          <span class="tag">Cursor/GitHub Copilot</span>
          <span class="tag">Excel/数据处理</span>
        </div>
      </section>
    </main>

    <!-- 底部版权区 -->
    <footer class="footer">
      <p>© 2025 [你的名字] · 游戏系统策划求职作品集</p>
      <p class="footer-links">
        <a href="#">关于我</a> · 
        <a href="#">联系方式</a> · 
        <a href="#">作品集PDF下载</a>
      </p>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'PortfolioPage',
  data() {
    return {
      // 可以放一些页面数据，比如项目列表、技能列表等
    }
  },
  mounted() {
    // 页面加载完成后的逻辑（如滚动监听等）
  },
  methods: {
    // 页面交互方法
  }
}
</script>

<style scoped>
/* 全局重置与字体 */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.page-container {
  font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
  line-height: 1.6;
  color: #333;
  background-color: #fafafa;
}

/* 头部样式 */
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1.2rem 2rem;
  background-color: #fff;
  box-shadow: 0 2px 10px rgba(0,0,0,0.05);
  position: sticky;
  top: 0;
  z-index: 100;
}

.logo {
  font-size: 1.5rem;
  font-weight: 600;
  color: #2c3e50;
  letter-spacing: 0.5px;
}

.nav a {
  margin-left: 2rem;
  text-decoration: none;
  color: #4a5568;
  font-weight: 500;
  transition: color 0.2s;
}

.nav a:hover {
  color: #007acc;
}

/* 主要内容区 */
.main-content {
  max-width: 1200px;
  margin: 0 auto;
  padding: 2rem;
}

/* 通用区块样式 */
.section {
  margin-bottom: 4rem;
}

.section-title {
  font-size: 2rem;
  font-weight: 600;
  margin-bottom: 2rem;
  color: #2c3e50;
  border-bottom: 3px solid #e2e8f0;
  padding-bottom: 0.5rem;
  display: inline-block;
}

/* 首页区块 */
.home-section {
  text-align: center;
  padding: 3rem 1rem;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  border-radius: 12px;
  color: white;
  margin-top: 1rem;
}

.title {
  font-size: 2.8rem;
  font-weight: 700;
  margin-bottom: 0.5rem;
}

.subtitle {
  font-size: 1.3rem;
  opacity: 0.95;
  margin-bottom: 1.5rem;
  font-weight: 300;
}

.intro-text {
  font-size: 1.1rem;
  max-width: 600px;
  margin: 0 auto;
  opacity: 0.9;
}

/* 项目卡片网格 */
.cards-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 2rem;
  margin-top: 1rem;
}

.project-card {
  background: white;
  border-radius: 10px;
  padding: 1.8rem;
  box-shadow: 0 4px 15px rgba(0,0,0,0.05);
  transition: transform 0.2s, box-shadow 0.2s;
  border: 1px solid #edf2f7;
}

.project-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 25px rgba(0,0,0,0.1);
}

.project-card h3 {
  font-size: 1.4rem;
  margin-bottom: 0.5rem;
  color: #2d3748;
}

.card-role {
  color: #007acc;
  font-weight: 600;
  font-size: 0.9rem;
  margin-bottom: 0.8rem;
  text-transform: uppercase;
  letter-spacing: 0.5px;
}

.card-desc {
  color: #4a5568;
  line-height: 1.6;
}

/* 技能标签 */
.skills-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.8rem;
}

.tag {
  background: #edf2f7;
  color: #2d3748;
  padding: 0.5rem 1.2rem;
  border-radius: 30px;
  font-size: 0.95rem;
  font-weight: 500;
  transition: all 0.2s;
  border: 1px solid transparent;
}

.tag:hover {
  background: #007acc;
  color: white;
  transform: scale(1.02);
}

/* 底部样式 */
.footer {
  background-color: #2d3748;
  color: #cbd5e0;
  text-align: center;
  padding: 2rem;
  margin-top: 2rem;
  font-size: 0.95rem;
}

.footer-links {
  margin-top: 0.8rem;
}

.footer-links a {
  color: #a0aec0;
  text-decoration: none;
  margin: 0 0.5rem;
  transition: color 0.2s;
}

.footer-links a:hover {
  color: white;
}

/* 响应式调整 */
@media (max-width: 768px) {
  .header {
    flex-direction: column;
    padding: 1rem;
  }
  
  .nav {
    margin-top: 1rem;
  }
  
  .nav a {
    margin: 0 0.8rem;
  }
  
  .title {
    font-size: 2rem;
  }
  
  .cards-grid {
    grid-template-columns: 1fr;
  }
}
</style>