# Lucas Jin (金启航) — Personal Academic Homepage

[![GitHub Pages](https://img.shields.io/badge/GitHub-Pages-blue)](https://Lucas-Jin-Qh.github.io/)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

🔬 **AI/ML Researcher** focusing on Vision-Language Models, Efficient Fine-tuning, and Long-Context Modeling

## 🌐 Live Site

Visit: [https://Lucas-Jin-Qh.github.io/](https://Lucas-Jin-Qh.github.io/)

## ✨ Features

- 🎨 **Modern Design**: Clean, responsive UI with dark mode support
- 🌍 **Bilingual**: Full Chinese/English support (auto-detection + manual toggle)
- 📱 **Mobile-First**: Fully responsive across all devices
- ⚡ **Performance**: Optimized loading with preconnect and lazy loading
- 🔍 **SEO Optimized**: Meta tags, Open Graph, Twitter Cards, structured data
- 📊 **Dynamic Content**: Auto-loads publications and projects from JSON files
- 🎯 **GitHub Integration**: Automatically displays latest repositories

## 📁 Project Structure

```
Lucas-Jin-Qh.github.io/
├── index.html              # Main HTML file (single-page architecture)
├── data/                   # Data files (JSON)
│   ├── i18n.json          # Internationalization strings
│   ├── site-data.json     # Email, links, social media
│   └── publications.json  # Research papers
├── sitemap.xml            # SEO sitemap
├── robots.txt             # Search engine directives
├── README.md              # This file
├── CHANGELOG.md           # Version history
└── LICENSE                # MIT License
```

## 🛠️ Tech Stack

- **Framework**: Pure HTML + [Alpine.js](https://alpinejs.dev/) (lightweight reactivity)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/) (CDN)
- **Icons**: [Lucide Icons](https://lucide.dev/)
- **Fonts**: [Inter](https://fonts.google.com/specimen/Inter) (Google Fonts)
- **Hosting**: GitHub Pages (static, no backend needed)

## 🚀 Quick Start

### 1. Clone Repository

```bash
git clone https://github.com/Lucas-Jin-Qh/Lucas-Jin-Qh.github.io.git
cd Lucas-Jin-Qh.github.io
```

### 2. Serve Locally

Choose one method:

```bash
# Python 3
python -m http.server 8000

# Node.js
npx serve

# PHP
php -S localhost:8000
```

Then open `http://localhost:8000` in your browser.

### 3. Deploy to GitHub Pages

1. Go to repository **Settings** → **Pages**
2. Select **Source**: `main` branch, `/root` folder
3. Save and wait ~1 minute
4. Visit `https://Lucas-Jin-Qh.github.io/`

## 📝 How to Update Content

### Update Publications

Edit `data/publications.json`:

```json
{
  "title": "Your Paper Title",
  "zhTitle": "论文中文标题（可选）",
  "authors": "Author1, Author2, ...",
  "venue": "Conference/Journal Name",
  "year": 2025,
  "pdf": "https://link-to-paper.pdf",
  "code": "https://github.com/your-repo",
  "tags": ["Tag1", "Tag2"],
  "bibtex": "@article{...}",
  "abstract": "Paper abstract in English",
  "zhAbstract": "论文摘要（中文）"
}
```

### Update Personal Info

Edit `data/site-data.json`:

```json
{
  "email": "your.email@example.com",
  "links": {
    "github": "https://github.com/your-username",
    "scholar": "https://scholar.google.com/citations?user=YOUR_ID",
    "linkedin": "https://www.linkedin.com/in/your-profile",
    "twitter": "https://twitter.com/your-handle"
  }
}
```

### Update Translations

Edit `data/i18n.json` to modify UI text in Chinese/English.

## 🎨 Customization

### Change Theme Color

Current: **Sky Blue** (`#0ea5e9`)

To change:
1. Search and replace `sky-` classes with your color (e.g., `blue-`, `purple-`)
2. Update `<meta name="theme-color" content="#YOUR_COLOR" />`

### Hide/Show Sections

To hide a section, add `hidden` class:

```html
<section id="about" class="hidden ...">
```

To reorder sections, move the entire `<section>` block in `index.html`.

## 📊 SEO Features

- ✅ Meta tags (title, description, keywords)
- ✅ Open Graph (Facebook, LinkedIn)
- ✅ Twitter Cards
- ✅ Structured Data (Schema.org Person)
- ✅ Sitemap (`sitemap.xml`)
- ✅ Robots.txt
- ✅ Canonical URLs

### Add Google Analytics (Optional)

Insert before `</head>` tag:

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

## 🌍 Custom Domain (Optional)

1. Add `CNAME` file with your domain:
   ```bash
   echo "yourdomain.com" > CNAME
   ```

2. Configure DNS:
   ```
   Type: A
   Name: @
   Value: 185.199.108.153
          185.199.109.153
          185.199.110.153
          185.199.111.153

   Type: CNAME
   Name: www
   Value: Lucas-Jin-Qh.github.io
   ```

## 🐛 Troubleshooting

### Website not showing?

1. Check GitHub Pages is enabled (Settings → Pages)
2. Verify branch is set to `main` and folder is `/root`
3. Wait 1-5 minutes for deployment
4. Clear browser cache (Ctrl+Shift+R / Cmd+Shift+R)

### Data not updating?

1. Validate JSON syntax at [jsonlint.com](https://jsonlint.com/)
2. Clear browser cache
3. Check browser console for errors (F12)
4. Verify file paths are correct

### Dark mode not working?

Test in browser console:
```javascript
localStorage.getItem('theme')  // Should return 'dark' or 'light'

// Reset if needed:
localStorage.removeItem('theme');
location.reload();
```

## 📄 License

MIT License - feel free to fork and customize for your own use!

## 🤝 Contributing

This is a personal homepage, but suggestions and bug reports are welcome via [Issues](https://github.com/Lucas-Jin-Qh/Lucas-Jin-Qh.github.io/issues).

## 📧 Contact

- **Email**: qihangjin@mail.ustc.edu.cn
- **GitHub**: [@Lucas-Jin-Qh](https://github.com/Lucas-Jin-Qh)
- **Twitter**: [@Qh_Jin_Lucas](https://x.com/Qh_Jin_Lucas)
- **Google Scholar**: [Profile](https://scholar.google.com/citations?user=pSvQSKsAAAAJ&hl=en)

---

**Built with ❤️ using Alpine.js + Tailwind CSS**

Last updated: October 29, 2025
