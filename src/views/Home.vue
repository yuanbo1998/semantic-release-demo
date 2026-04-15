<template>
  <div class="home">
    <h1>首页</h1>
    <p>欢迎使用 Semantic Release Demo 项目</p>
    <p>本项目演示如何使用 semantic-release 进行自动化版本发布控制。</p>
    <div class="features">
      <div class="feature-card">
        <h3>🚀 Vite</h3>
        <p>下一代前端构建工具</p>
      </div>
      <div class="feature-card">
        <h3>💚 Vue 3</h3>
        <p>渐进式 JavaScript 框架</p>
      </div>
      <div class="feature-card">
        <h3>🛤️ Vue Router</h3>
        <p>Vue.js 官方路由管理器</p>
      </div>
      <div class="feature-card">
        <h3>📦 Semantic Release</h3>
        <p>自动化版本发布工具</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.home {
  text-align: center;
  padding: 2rem;
}
.home h1 {
  font-size: 2rem;
  margin-bottom: 1rem;
  color: #42b883;
}
.home > p {
  color: #666;
  margin-bottom: 0.5rem;
}
.features {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 1.5rem;
  margin-top: 2rem;
  max-width: 800px;
  margin-left: auto;
  margin-right: auto;
}
.feature-card {
  padding: 1.5rem;
  border: 1px solid #e2e8f0;
  border-radius: 8px;
  background: #f8fafc;
  transition: transform 0.2s, box-shadow 0.2s;
}
.feature-card:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}
.feature-card h3 {
  margin-bottom: 0.5rem;
  font-size: 1.2rem;
}
.feature-card p {
  color: #64748b;
  font-size: 0.9rem;
}
</style>
