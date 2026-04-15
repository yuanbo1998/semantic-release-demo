<template>
  <div id="app-wrapper">
    <nav class="navbar">
      <div class="nav-brand">Semantic Release Demo</div>
      <div class="nav-links">
        <router-link to="/">首页</router-link>
        <router-link to="/about">关于</router-link>
      </div>
    </nav>
    <main class="main-content">
      <router-view />
    </main>
  </div>
</template>

<style scoped>
.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 2rem;
  height: 60px;
  background: #42b883;
  color: white;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
}
.nav-brand {
  font-size: 1.3rem;
  font-weight: 700;
}
.nav-links {
  display: flex;
  gap: 1.5rem;
}
.nav-links a {
  color: white;
  text-decoration: none;
  font-size: 1rem;
  padding: 0.5rem 1rem;
  border-radius: 6px;
  transition: background 0.2s;
}
.nav-links a:hover {
  background: rgba(255, 255, 255, 0.2);
}
.nav-links a.router-link-active {
  background: rgba(255, 255, 255, 0.3);
  font-weight: 600;
}
.main-content {
  min-height: calc(100vh - 60px);
}
</style>
