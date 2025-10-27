# 🚀 快速入门指南 / Quick Start Guide

> 5 分钟让您的个人主页上线！

---

## ⚡ 快速部署（3 步）

### 第 1 步：推送到 GitHub

```bash
# 在项目目录下
cd /home/jqh/Lucas-Jin-Qh.github.io

# 查看修改
git status

# 添加所有文件
git add .

# 提交更改
git commit -m "🚀 Optimize homepage: SEO, performance, and documentation"

# 推送到 GitHub
git push origin main
```

### 第 2 步：启用 GitHub Pages

1. 访问仓库：https://github.com/Lucas-Jin-Qh/Lucas-Jin-Qh.github.io
2. 点击 **Settings** (设置)
3. 左侧菜单点击 **Pages**
4. 在 **Source** 下选择：
   - Branch: `main`
   - Folder: `/ (root)`
5. 点击 **Save** (保存)
6. 等待 1-2 分钟

### 第 3 步：访问您的网站

🌐 **您的网站地址**：https://Lucas-Jin-Qh.github.io/

---

## 📝 立即更新内容

### ✅ 必做清单

#### 1. 检查个人信息
编辑 `data/site-data.json`：
```json
{
  "email": "qihangjin@mail.ustc.edu.cn",  // ✅ 确认邮箱正确
  "links": {
    "github": "...",    // ✅ 检查链接
    "scholar": "...",   // ✅ 检查链接
    "orcid": "..."      // ⚠️ 更新您的 ORCID 链接
  }
}
```

#### 2. 更新论文列表
编辑 `data/publications.json`，确保：
- ✅ 所有论文信息准确
- ✅ PDF 链接可访问
- ✅ 代码仓库链接正确
- ✅ BibTeX 格式正确

#### 3. 更新新闻动态
编辑 `data/news.json`：
- ✅ 删除示例新闻
- ✅ 添加真实的最新动态
- ✅ 按日期降序排列

#### 4. 检查报告/教学/服务
检查这些文件是否需要更新：
- `data/talks.json`
- `data/teaching.json`
- `data/service.json`

---

## 🎨 个性化定制

### 更换头像

**方法 1：使用自定义图片**
```html
<!-- 在 index.html 第 132 行附近 -->
<img src="./images/avatar.jpg"  <!-- 使用本地图片 -->
     alt="Lucas Jin (金启航) - AI Researcher">
```

**方法 2：使用其他头像服务**
```html
<img src="https://www.gravatar.com/avatar/YOUR_HASH"
     alt="...">
```

### 修改主题色

当前主题色：**Sky Blue** (`#0ea5e9`)

如需更换：
1. 搜索 `sky-` 并替换为其他颜色（如 `blue-`, `indigo-`, `purple-`）
2. 更新 `meta theme-color`：
```html
<meta name="theme-color" content="#你的颜色代码" />
```

### 调整布局

**隐藏某个板块**：
```html
<!-- 在对应的 section 标签上添加 hidden 类 -->
<section id="talks" class="hidden ...">
```

**调整顺序**：
直接在 `index.html` 中移动整个 `<section>` 代码块

---

## 🔍 SEO 提交清单

### Google Search Console

1. 访问：https://search.google.com/search-console
2. 添加资源：`https://Lucas-Jin-Qh.github.io/`
3. 验证所有权（通过 HTML 文件或 meta 标签）
4. 提交 Sitemap：`https://Lucas-Jin-Qh.github.io/sitemap.xml`

### Google Scholar

确保您的论文已被收录：
1. 访问：https://scholar.google.com/citations
2. 添加论文时引用您的个人主页

### 学术社交网络

更新以下平台的个人资料，添加主页链接：
- ✅ Google Scholar
- ✅ ORCID
- ✅ ResearchGate
- ✅ LinkedIn
- ✅ Twitter/X

---

## 📊 添加访问统计

### 方法 1：Google Analytics 4 (免费)

1. 访问：https://analytics.google.com/
2. 创建账号和资源
3. 获取测量 ID（格式：`G-XXXXXXXXXX`）
4. 在 `index.html` 的 `</head>` 前添加：

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

### 方法 2：Plausible Analytics (隐私友好)

更简单，不需要 Cookie 横幅：

```html
<script defer data-domain="Lucas-Jin-Qh.github.io" 
        src="https://plausible.io/js/script.js"></script>
```

---

## 🐛 常见问题

### ❓ 网站不显示？

**检查清单**：
1. GitHub Pages 是否已启用？
2. 分支是否选择正确（`main`）？
3. 等待 1-5 分钟让 GitHub 构建
4. 清除浏览器缓存（Ctrl+Shift+R / Cmd+Shift+R）

### ❓ 数据没有更新？

**解决方法**：
1. 检查 JSON 文件格式（使用 https://jsonlint.com/）
2. 清除浏览器缓存
3. 检查浏览器控制台是否有错误（F12）
4. 确认文件路径正确（`/data/xxx.json`）

### ❓ 深色模式不工作？

**检查**：
```javascript
// 浏览器控制台测试
localStorage.getItem('theme')  // 应返回 'dark' 或 'light'
```

**重置**：
```javascript
localStorage.removeItem('theme');
location.reload();
```

### ❓ GitHub 仓库不显示？

**原因**：API 限流（未登录 60 次/小时）

**解决**：
1. 等待 1 小时后自动恢复
2. 或使用 GitHub Token（参考 README.md）

---

## 📱 测试清单

在发布前，请测试：

### 桌面端
- [ ] Chrome/Edge
- [ ] Firefox  
- [ ] Safari (Mac)

### 移动端
- [ ] iOS Safari
- [ ] Android Chrome
- [ ] 微信内置浏览器

### 功能测试
- [ ] 中英文切换
- [ ] 深色模式切换
- [ ] 所有链接可点击
- [ ] 论文搜索功能
- [ ] 联系表单（生成邮件）
- [ ] 响应式布局（缩放窗口）

---

## 🎯 下一步建议

### 本周完成
1. ✅ 更新所有个人信息
2. ✅ 检查所有外部链接
3. ✅ 添加真实头像
4. ✅ 提交到 Google Search Console
5. ✅ 分享到社交媒体

### 本月完成
1. 📊 添加访问统计
2. 📝 撰写 1-2 篇博客（可选）
3. 🎨 优化移动端体验
4. 📧 在邮件签名中添加主页链接
5. 🔗 申请自定义域名（可选）

### 长期维护
1. 每月更新新闻动态
2. 及时添加新论文
3. 定期检查链接有效性
4. 关注 Google Analytics 数据
5. 根据反馈持续优化

---

## 💡 专业建议

### 学术用途
- 在 CV 中突出显示您的主页链接
- 在论文作者信息中包含主页
- 会议海报/PPT 中展示 QR 码
- 邮件签名中添加主页

### 求职/申请
- PhD 申请材料中引用主页
- RA 申请邮件中包含链接
- LinkedIn 个人资料添加主页
- 面试时准备好演示

### 社交传播
- Twitter/X 置顶推文
- 学术微信群分享
- ResearchGate 个人简介
- 知乎/CSDN 文章引用

---

## 📞 获取帮助

**遇到技术问题？**

1. 📖 查看 `README.md` 详细文档
2. 📊 查看 `OPTIMIZATION_SUMMARY.md` 了解优化细节
3. 🐛 检查浏览器控制台错误信息
4. 💬 GitHub Issues 提问

**需要定制开发？**

可以考虑添加：
- 博客系统
- 评论功能
- 在线简历生成
- 项目展示页
- 研究组介绍
- 更多...

---

## 🎉 恭喜！

您的专业学术主页已经优化完成！

**现在就推送代码，让全世界看到您的研究成果吧！** 🚀

```bash
git add .
git commit -m "🚀 Launch optimized homepage"
git push origin main
```

---

最后更新：2025-10-27

