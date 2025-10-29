# 更新日志 / Changelog

All notable changes to this project will be documented in this file.

---

## [3.0.0] - 2025-10-29

### 🧹 Simplified & Cleaned

#### Removed
- ❌ **News Section** - Removed news board as not needed for student stage
- ❌ **RSS Feed** - Removed `/feed.xml` and related functionality
- ❌ **Unused Data Files** - Deleted `teaching.json`, `talks.json`, `service.json`, `news.json`
- ❌ **Redundant Documentation** - Cleaned up 5+ outdated documentation files

#### Changed
- ♻️ **UI Optimization** - Adjusted section backgrounds for better visual hierarchy
  - Publications: Changed to gray background (`bg-gray-50`)
  - Projects: Changed to white background (`border-t`)
- 📝 **Navigation** - Removed "News" link from both desktop and mobile nav
- 🗂️ **Data Structure** - Simplified inline data, removed unused fields
- 📚 **Documentation** - Consolidated to just `README.md` and `CHANGELOG.md`

#### Improved
- ⚡ **Performance** - Reduced page complexity and data loading
- 🎯 **Focus** - Streamlined content to highlight research and publications
- 📦 **Maintenance** - Easier to maintain with fewer files and cleaner structure

### 📊 Code Statistics
- **Removed**: ~90+ lines of code
- **Files deleted**: 10 (5 data files + 5 documentation files)
- **HTML lines**: 856 → 824 (32 lines reduction)

---

## [2.0.0] - 2025-10-27

### ✨ Added / 新增功能
- 🌍 Complete bilingual support (Chinese/English) with auto-detection
- 📱 Fully responsive design for all devices
- 🎨 Dark mode support with user preference saving
- 📊 Dynamic GitHub repository loading
- 🔍 Publication search and filter functionality
- 📡 RSS Feed support
- 🗺️ Sitemap.xml for SEO
- 🤖 Robots.txt configuration
- 📧 Contact form (mailto protocol)

### 🎨 Improved / 优化
- ⚡ Performance optimizations: preconnect, DNS prefetch, lazy loading
- 🔍 SEO optimization: Meta tags, Open Graph, Twitter Cards
- ♿ Accessibility improvements: ARIA labels, semantic HTML
- 🎯 Better code organization and structure
- 📦 Data/presentation separation (JSON data files)

### 🐛 Fixed / 修复
- ✅ Fixed JSON format errors in inline data
- ✅ Corrected missing data file references
- ✅ Improved icon loading timing

### 📁 New Files / 新增文件
- `data/i18n.json` - Internationalization strings
- `data/site-data.json` - Personal information and links
- `data/publications.json` - Research publications
- `sitemap.xml` - Site map
- `robots.txt` - Search engine configuration
- `README.md` - Project documentation
- `LICENSE` - MIT open source license
- `.gitignore` - Git ignore configuration

---

## [1.0.0] - 2025-10-20

### Initial Release / 初始版本
- Basic single-page architecture
- Alpine.js + Tailwind CSS framework
- Publication showcase
- Project list
- Contact information

---

## 🎯 Future Plans / 未来计划

As the career progresses (PhD/Professor stage), these sections can be easily added back:
- **Academic Talks** - Invited presentations
- **Teaching Experience** - Courses and student supervision
- **Academic Service** - Reviewing, committees, etc.
- **News Updates** - Awards, media coverage, etc.

Simply create the corresponding JSON files and add sections to `index.html`.

---

**For detailed information, see [README.md](README.md)**

Last updated: October 29, 2025
