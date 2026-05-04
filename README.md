# yiban1145.github.io
```markdown
# 🔮 纯净导航

> 一个极简、纯净、无追踪的浏览器导航页，搜索框支持命令行彩蛋。注意！只能用电脑UA访问

[![GitHub Pages](https://img.shields.io/badge/在线体验-GitHub%20Pages-blue)](https://yiban1145.github.io/nav)
[![License](https://img.shields.io/badge/License-MIT-green)](./LICENSE)
[![PR Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen)](https://github.com/yiban1145/nav/pulls)

## ✨ 特性

- 🔍 **多引擎搜索** — 一键切换 百度 / 谷歌 / 必应 / 360 / 搜狗
- 🌐 **智能识别** — 自动识别网址和搜索词，输入网址直接跳转
- 🌙 **暗色模式** — 支持亮色/暗色切换，自动跟随系统偏好
- ⌨️ **命令行彩蛋** — 搜索框输入命令触发隐藏功能
- 📱 **响应式设计** — 手机、平板、电脑完美适配
- 🔒 **隐私优先** — 纯静态页面，零追踪、零Cookie（仅存主题偏好）
- ⚡ **零依赖** — 单文件 HTML，无框架、无库、无后端

## 🎮 命令行彩蛋

在搜索框输入以下命令并回车：

| 命令 | 功能 |
|------|------|
| `/help` | 显示所有可用命令 |
| `/dark` | 切换到暗色模式 |
| `/light` | 切换到亮色模式 |
| `/theme` | 切换亮色/暗色 |
| `/time` | 显示当前时间 |
| `/date` | 显示当前日期 |
| `/hello` | 随机问候 |
| `/about` | 关于页面信息 |
| `/easter` | 🥚 发现一个彩蛋 |
| `/github` | 打开 GitHub |
| `/clear` | 清空搜索框 |

## ⌨️ 快捷键

| 快捷键 | 功能 |
|--------|------|
| `Ctrl + K` | 聚焦搜索框 |
| `/` | 聚焦搜索框 |
| `Esc` | 清除输入或取消聚焦 |
| `Ctrl + Shift + D` | 切换暗色模式 |
| `←` `→` | 切换搜索引擎 |

## 🚀 快速部署

### 方式一：GitHub Pages（推荐）

1. Fork 本仓库
2. 进入 Settings → Pages
3. Source 选择 `main` 分支，点击 Save
4. 等待一分钟，访问 `https://你的用户名.github.io/nav`

### 方式二：Vercel

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new)

点击上方按钮一键部署，或手动将 `index.html` 上传到 Vercel。

### 方式三：Cloudflare Pages

1. 将 `index.html` 上传到 GitHub 仓库
2. 登录 Cloudflare Dashboard → Pages
3. 连接仓库，直接部署

### 方式四：任意静态托管

直接将 `index.html` 上传到任何静态文件服务器即可，无需任何构建步骤。

### 方式五：设为浏览器主页

部署后，将链接设置为浏览器的启动主页或新标签页。

## 🎨 自定义

### 修改快捷入口

编辑 `index.html` 中 `<div class="quick-links">` 部分的链接：

```html
<a class="quick-link-card" href="你的网址" target="_blank" rel="noopener" title="名称">
    <div class="quick-link-icon">
        <img src="图标地址" alt="名称" loading="lazy"
             onerror="this.style.display='none';this.nextElementSibling.style.display='flex';">
        <div class="fallback-icon" style="display:none; background: #颜色;">文字</div>
    </div>
    <span class="quick-link-name">名称</span>
</a>
```

修改搜索引擎

编辑 <script> 标签中的 engineConfig 对象，可增删或修改搜索引擎。

添加新命令

编辑 <script> 标签中的 commands 对象：

```javascript
'/你的命令': () => {
    // 执行操作
    return '提示文字';
}
```

📂 项目结构

```
nav/
├── index.html    # 唯一文件，包含所有 HTML/CSS/JS
└── README.md     # 本文件
```

🤝 贡献

欢迎提交 Issue 和 Pull Request！

📜 许可证

MIT License — 自由使用、修改、分发。

---

<p align="center">
  <b>🔮 纯净、快速、零追踪的导航页</b><br>
  <sub>Made with ❤️ by 你的名字</sub>
</p>
```

📝 使用说明

1. 替换占位符：
   · 你的用户名 → 你的 GitHub 用户名
   · 你的名字 → 你的昵称
2. 添加预览图（可选但强烈推荐）：
   · 截一张带命令行的截图，保存为 preview.png
   · 在 README 的 ## ✨ 特性 上面添加：
   ```markdown
   ![预览](preview.png)
   ```
3. 创建 LICENSE 文件（可选）：
   · 在仓库根目录创建 LICENSE 文件，写入 MIT License 文本
4. 上传到 GitHub：
   · 把 index.html 和 README.md 推送到仓库
