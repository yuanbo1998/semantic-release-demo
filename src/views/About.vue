<template>
  <div class="about">
    <h1>关于 Semantic Release</h1>
    <div class="content">
      <section>
        <h2>什么是 Semantic Release？</h2>
        <p>Semantic Release 是一个自动化版本发布工具，它根据 Commit Message 自动确定下一个版本号、生成 CHANGELOG 并发布。</p>
      </section>
      <section>
        <h2>Commit 规范</h2>
        <table>
          <thead>
            <tr><th>类型</th><th>说明</th><th>版本影响</th></tr>
          </thead>
          <tbody>
            <tr><td><code>feat:</code></td><td>新功能</td><td>Minor 版本</td></tr>
            <tr><td><code>fix:</code></td><td>修复 Bug</td><td>Patch 版本</td></tr>
            <tr><td><code>feat!:</code></td><td>破坏性变更</td><td>Major 版本</td></tr>
            <tr><td><code>docs:</code></td><td>文档变更</td><td>无版本影响</td></tr>
            <tr><td><code>style:</code></td><td>代码格式</td><td>无版本影响</td></tr>
            <tr><td><code>refactor:</code></td><td>代码重构</td><td>无版本影响</td></tr>
            <tr><td><code>chore:</code></td><td>构建/工具</td><td>无版本影响</td></tr>
          </tbody>
        </table>
      </section>
      <section>
        <h2>工作流程</h2>
        <ol>
          <li>开发者按照 Conventional Commits 规范提交代码</li>
          <li>CI/CD 流水线触发 semantic-release</li>
          <li>semantic-release 分析 commits，决定版本号</li>
          <li>自动生成 CHANGELOG.md</li>
          <li>自动创建 Git Tag 并发布</li>
        </ol>
      </section>
    </div>
  </div>
</template>

<style scoped>
.about {
  padding: 2rem;
  max-width: 800px;
  margin: 0 auto;
}
.about h1 {
  color: #42b883;
  text-align: center;
  margin-bottom: 2rem;
}
.content section {
  margin-bottom: 2rem;
}
.content h2 {
  color: #334155;
  border-bottom: 2px solid #42b883;
  padding-bottom: 0.5rem;
  margin-bottom: 1rem;
}
.content p {
  color: #475569;
  line-height: 1.8;
}
table {
  width: 100%;
  border-collapse: collapse;
}
th, td {
  padding: 0.75rem;
  text-align: left;
  border-bottom: 1px solid #e2e8f0;
}
th {
  background: #f1f5f9;
  color: #334155;
}
code {
  background: #f1f5f9;
  padding: 0.2rem 0.5rem;
  border-radius: 4px;
  color: #e11d48;
  font-size: 0.9rem;
}
ol {
  padding-left: 1.5rem;
}
ol li {
  color: #475569;
  line-height: 2;
}
</style>
