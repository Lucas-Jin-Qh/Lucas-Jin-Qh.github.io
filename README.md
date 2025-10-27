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
- ⚡ **Performance**: Optimized loading with preconnect, lazy loading, and content visibility
- 🔍 **SEO Optimized**: Meta tags, Open Graph, Twitter Cards, structured data
- 📊 **Dynamic Content**: Auto-loads publications, projects, news from JSON files
- 🎯 **GitHub Integration**: Automatically displays latest repositories
- 📡 **RSS Feed**: Subscribe to updates at `/feed.xml`

## 📁 Project Structure

```
Lucas-Jin-Qh.github.io/
├── index.html              # Main HTML file (single-page architecture)
├── data/                   # Data files (JSON)
│   ├── i18n.json          # Internationalization strings
│   ├── site-data.json     # Email, links, social media
│   ├── publications.json  # Research papers
│   ├── news.json          # News updates
│   ├── talks.json         # Academic talks
│   ├── teaching.json      # Teaching experience
│   └── service.json       # Academic service
├── feed.xml               # RSS feed
├── sitemap.xml            # SEO sitemap
├── robots.txt             # Search engine directives
└── README.md              # This file
```

## 🛠️ Tech Stack

- **Framework**: Pure HTML + [Alpine.js](https://alpinejs.dev/) (lightweight reactivity)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/) (CDN)
- **Icons**: [Lucide Icons](https://lucide.dev/)
- **Fonts**: [Inter](https://fonts.google.com/specimen/Inter) (Google Fonts)
- **Hosting**: GitHub Pages (static, no backend needed)

## 📝 How to Update Content

### 1. Update Publications

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
  "bibtex": "@article{...}"
}
```

### 2. Update News

Edit `data/news.json`:

```json
{
  "date": "2025-10-27",
  "text": "Your news update (supports both zh/en)",
  "link": "https://optional-link.com"
}
```

### 3. Update Personal Info

Edit `data/site-data.json` for email and social links.

### 4. Update Translations

Edit `data/i18n.json` to modify UI text in Chinese/English.

## 🚀 Local Development

1. Clone the repository:
```bash
git clone https://github.com/Lucas-Jin-Qh/Lucas-Jin-Qh.github.io.git
cd Lucas-Jin-Qh.github.io
```

2. Serve locally (choose one):
```bash
# Python 3
python -m http.server 8000

# Node.js
npx serve

# PHP
php -S localhost:8000
```

3. Open `http://localhost:8000` in your browser

## 🎨 Customization

### Colors

The site uses sky blue (`#0ea5e9`) as the primary color. To change:

1. Update `meta theme-color` in `<head>`
2. Search and replace `sky-` classes in Tailwind CSS
3. Update gradient backgrounds as needed

### Sections

To add/remove sections:

1. Add HTML section in `index.html`
2. Add navigation link in header
3. Update i18n strings in `data/i18n.json`

## 📊 SEO & Analytics

- ✅ Meta tags (title, description, keywords)
- ✅ Open Graph (Facebook, LinkedIn)
- ✅ Twitter Cards
- ✅ Structured Data (Schema.org Person)
- ✅ Sitemap (`sitemap.xml`)
- ✅ RSS Feed (`feed.xml`)
- ✅ Robots.txt
- ✅ Canonical URLs

To add Google Analytics, insert tracking code before `</head>` tag.

## 🌍 Deployment

### GitHub Pages (Automatic)

1. Go to repository **Settings** → **Pages**
2. Select **Source**: `main` branch, `/root` folder
3. Save and wait ~1 minute
4. Visit `https://Lucas-Jin-Qh.github.io/`

### Custom Domain (Optional)

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

Last updated: October 27, 2025

