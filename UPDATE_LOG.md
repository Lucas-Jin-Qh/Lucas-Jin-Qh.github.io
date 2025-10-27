# 📝 主页更新日志

**更新时间**: 2025-10-27  
**更新内容**: 根据真实简历优化主页，删除虚构内容

---

## ✅ 已完成的更改

### 1️⃣ **头像更新**
- ✅ 将头像从 GitHub URL 更改为本地文件 `top.png`
- ✅ 更新 Open Graph 和 Twitter Card 图片链接

**修改位置**:
- `index.html` 第 132 行 - 主头像
- `index.html` 第 17 行 - OG 图片
- `index.html` 第 24 行 - Twitter 图片

---

### 2️⃣ **中英文描述更新**
根据 `data/i18n.json` 中的真实内容更新了描述：

#### 中文描述
```
AI研究生，就读于 USTC · IAT（电子与信息工程 M.Eng.），
专注多模态基础模型与高效优化；
目前开放 RA/合作与 2026 入学 PhD 机会。
```

#### 英文描述
```
M.Eng. student at USTC · IAT focusing on multimodal 
foundation models and efficient optimization; 
open to RA roles and PhD applications (2026 intake).
```

**修改位置**:
- `index.html` 第 336 行 - 中文 hero 描述
- `index.html` 第 338 行 - 中文 about 描述
- `index.html` 第 350 行 - 英文 hero 描述
- `index.html` 第 352 行 - 英文 about 描述

---

### 3️⃣ **删除虚构内容**

#### 已清空的示例数据
- ✅ `index.html` 内嵌的 news 数组（已清空）
- ✅ `index.html` 内嵌的 publications 数组（已清空）
- ✅ `index.html` 内嵌的 talks 数组（已清空）
- ✅ `index.html` 内嵌的 teaching 数组（已清空）
- ✅ `index.html` 内嵌的 service 数组（已清空）
- ✅ `data/talks.json` - 清空示例报告
- ✅ `data/teaching.json` - 清空示例教学记录
- ✅ `data/service.json` - 清空示例学术服务

#### 更新的研究关键词
**之前（虚构项目名）**:
- VRI/VRST
- LIT
- HySSM-Pyramid
- ULRA/J-ORA/QISA
- DeepSeek-OCR

**现在（真实研究方向）**:
- 视觉-语言模型
- 模型优化
- 多模态学习
- 模型对齐

---

### 4️⃣ **简历链接更新**
- ✅ 将简历链接从 `./static/CV_LucasJin.pdf` 更新为 `./Qihang Jin_Resume.pdf`

**修改位置**: `index.html` 第 179 行

---

## 📁 保留的真实数据

以下文件包含真实内容，已保留：

### `data/publications.json` (3 篇论文)
1. **From Memory to Alignment: A Comprehensive Review of Large Language Model Optimization**
   - 第二作者：Qihang Jin (Lucas)
   - 发表于：IEEE TechRxiv (preprint)
   - 年份：2025
   - 链接：✅ 有效

2. **Effect of Brain-Computer Interface on Limb Motor Function...**
   - 作者：Qihang Jin et al.
   - 状态：Under review
   - 年份：2025

3. **Multimodal Representation Learning and Fusion**
   - 作者：Qihang Jin et al.
   - 状态：Under review
   - 年份：2025

### `data/news.json` (1 条新闻)
- **2025-10-27**: TechRxiv 预印本上线
  - 链接：✅ 有效

### `data/site-data.json`
- ✅ 邮箱：qihangjin@mail.ustc.edu.cn
- ✅ GitHub: https://github.com/Lucas-Jin-Qh
- ✅ Google Scholar: 有效链接
- ✅ arXiv: 有效链接
- ⚠️ ORCID: 需要更新为真实链接
- ✅ Twitter: @Qh_Jin_Lucas

---

## 📋 数据结构说明

### 工作原理
网站使用**双层数据系统**：

1. **外部 JSON 文件** (`/data/*.json`) - 优先级高
   - 实际显示的内容来源
   - 易于更新和维护

2. **内嵌数据** (index.html 中的 script 标签) - 备用
   - 当外部文件不可用时的后备方案
   - 现已清空虚构示例数据

### 更新内容的方法
只需编辑 `/data/` 目录下的 JSON 文件：

```bash
# 添加新论文
编辑: data/publications.json

# 发布新闻
编辑: data/news.json

# 添加报告/教学/服务
编辑: data/talks.json / teaching.json / service.json
```

---

## ⚠️ 待办事项

### 必须完成
- [ ] **更新 ORCID 链接**
  - 当前：https://orcid.org/ （占位符）
  - 需要：您的真实 ORCID 链接
  - 修改文件：`data/site-data.json`

### 可选补充
- [ ] 添加论文的 BibTeX 引用
- [ ] 上传更多研究成果（如果有）
- [ ] 添加教学/报告经历（如果有）
- [ ] 完善论文的 PDF 和 Code 链接

---

## 🚀 部署步骤

### 1. 检查文件
确保以下文件在根目录：
- ✅ `top.png` - 头像图片
- ✅ `Qihang Jin_Resume.pdf` - 简历文件
- ✅ `index.html` - 主页
- ✅ `data/` 文件夹及其内容

### 2. 推送到 GitHub
```bash
cd /home/jqh/Lucas-Jin-Qh.github.io

# 查看更改
git status

# 添加所有文件
git add .

# 提交
git commit -m "更新主页：使用真实头像和简历内容，删除虚构数据"

# 推送
git push origin main
```

### 3. 访问网站
等待 1-2 分钟后访问：
🌐 **https://Lucas-Jin-Qh.github.io/**

---

## 📊 文件清单

### 已修改的文件
- ✅ `index.html` - 更新头像路径、描述、删除示例数据
- ✅ `data/talks.json` - 清空示例数据
- ✅ `data/teaching.json` - 清空示例数据
- ✅ `data/service.json` - 清空示例数据

### 真实数据文件（未修改）
- ✅ `data/publications.json` - 3 篇真实论文
- ✅ `data/news.json` - 1 条真实新闻
- ✅ `data/site-data.json` - 个人联系信息
- ✅ `data/i18n.json` - 中英文界面文本

### 新增/优化的文件（之前创建）
- ✅ `sitemap.xml` - SEO 网站地图
- ✅ `robots.txt` - 搜索引擎配置
- ✅ `README.md` - 项目文档
- ✅ `LICENSE` - MIT 许可证
- ✅ `.gitignore` - Git 配置

---

## 🎯 网站当前状态

### 内容概览
- **论文数量**: 3 篇（全部真实）
- **新闻动态**: 1 条（真实）
- **研究方向**: 视觉-语言模型、模型优化、多模态学习
- **学术报告**: 0（待添加）
- **教学经历**: 0（待添加）
- **学术服务**: 0（待添加）

### 展示效果
- ✅ 使用您的真实头像 (`top.png`)
- ✅ 真实的个人介绍（来自 i18n.json）
- ✅ 真实的论文列表（来自 publications.json）
- ✅ 真实的新闻动态（来自 news.json）
- ✅ 自动加载 GitHub 仓库
- ✅ 完整的中英双语支持

---

## 📝 后续建议

### 内容完善
1. **完成 ORCID 链接**
   ```json
   // 在 data/site-data.json 中
   "orcid": "https://orcid.org/0000-0000-0000-0000"
   ```

2. **添加 BibTeX 引用**
   - 为 publications.json 中的论文添加完整 BibTeX

3. **补充教学/服务经历**（如果有）
   - 编辑 `data/teaching.json`
   - 编辑 `data/service.json`
   - 编辑 `data/talks.json`

### 质量提升
1. **优化头像**
   - 确保 `top.png` 清晰度良好
   - 建议尺寸：400x400 或更高
   - 格式：PNG（支持透明背景）

2. **完善论文信息**
   - 添加缺失的 PDF 链接
   - 添加 Code 仓库链接
   - 完善作者列表

---

## ✨ 总结

您的主页现在：
- ✅ **100% 真实内容** - 所有虚构示例已删除
- ✅ **使用本地头像** - top.png
- ✅ **链接真实简历** - Qihang Jin_Resume.pdf
- ✅ **准确的个人介绍** - 基于 i18n.json
- ✅ **真实的学术成果** - 3 篇论文，1 条新闻

**可以放心部署和分享！** 🎉

---

更新完成于：2025-10-27

