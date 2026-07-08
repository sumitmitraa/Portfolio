# Alex Chen — AI Engineer Portfolio

A modern, dark-themed, multi-page portfolio website built for an AI Engineering student. Features smooth animations, particle backgrounds, responsive design, and a bubbly UI with generous whitespace.

![Portfolio Preview](https://img.shields.io/badge/Portfolio-Live-purple?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

---

## 🌟 Features

| Feature | Description |
|---------|-------------|
| **Dark Theme** | Deep navy-black background with purple accent colors |
| **Particle Background** | Animated floating dots with connection lines on every page |
| **Scroll Reveal Animations** | Elements fade in smoothly as you scroll |
| **Animated Counters** | Numbers count up when they come into view |
| **Typing Effect** | Auto-typing text in the hero section |
| **Skill Progress Bars** | Animated bars that fill on scroll |
| **Project Filtering** | Filter projects by category (All, NLP, CV, LLMs, etc.) |
| **FAQ Accordion** | Expandable/collapsible questions on Contact page |
| **Floating Form Labels** | Labels animate when you focus on input fields |
| **Mobile Responsive** | Fully responsive with hamburger menu on mobile |
| **Back to Top Button** | Appears after scrolling down |
| **Glassmorphism Navbar** | Blur effect navbar that shrinks on scroll |

---

## 📁 Project Structure

```
portfolio/
│
├── portfolio.html      # Home / Landing page
├── about.html          # About Me page
├── skills.html         # Skills, Experience & Education
├── projects.html       # Projects showcase with filtering
├── contact.html        # Contact form, FAQ, Social links
│
└── (images/)           # Add your project screenshots here
```

> **Note:** All CSS and JavaScript is embedded in each HTML file. No external dependencies except Google Fonts.

---

## 🚀 Getting Started

### Option 1: Direct Open
1. Download all 5 HTML files
2. Place them in the same folder
3. Double-click `portfolio.html` to open in browser

### Option 2: Live Server (Recommended)
```bash
# Using VS Code Live Server extension
# Or using Python
python -m http.server 8000

# Then open http://localhost:8000/portfolio.html
```

### Option 3: Deploy Online
Upload all files to:
- GitHub Pages
- Netlify
- Vercel
- Any static hosting

---

## 🎨 Customization Guide

### 1. Change Name & Branding

Open each HTML file and find:
```html
<!-- Logo -->
<a href="portfolio.html" class="logo">
    <div class="logo-dot"></div>
    alex.dev          <!-- Change this -->
</a>

<!-- Hero Name -->
<h1>Building <span class="gradient-text">Intelligent</span><br>Systems That Matter</h1>
<p>I'm <strong>Alex Chen</strong>, an AI Engineering student...  <!-- Change name -->
```

### 2. Update Contact Information

In `contact.html`:
```html
<a href="mailto:alex@example.com" class="info-link">alex@example.com</a>  <!-- Change email -->

<!-- Social Links -->
<span>@alexchen</span>        <!-- Change username -->
<span>/in/alex-chen</span>   <!-- Change LinkedIn -->
```

### 3. Add Real Project Images

Replace emoji placeholders with actual images:

```html
<!-- Current (Placeholder) -->
<div class="project-image p1">
    <span>📄</span>
</div>

<!-- With Real Image -->
<div class="project-image p1">
    <img src="images/smartdoc.jpg" alt="SmartDoc AI" style="width:100%;height:100%;object-fit:cover;">
</div>
```

Create an `images/` folder and add your screenshots.

### 4. Update Skills & Progress Bars

In `skills.html`, find skill cards and modify:
```html
<div class="skill-bar"><div class="skill-progress" data-width="92"></div></div>
<!-- Change data-width value (0-100) -->
```

### 5. Change Color Theme

Find `:root` CSS variables in each file:
```css
:root {
    --accent: #a78bfa;        /* Main purple color */
    --accent-bright: #c4b5fd; /* Lighter purple */
    /* Change these hex codes to your preferred color */
}
```

### 6. Update Education & Experience

In `skills.html`, edit the timeline cards:
```html
<h3>M.S. in Artificial Intelligence</h3>
<div class="edu-school">Stanford University</div>  <!-- Change university -->
<span class="edu-year">2024 — 2026</span>           <!-- Change years -->
```

---

## 📱 Responsive Breakpoints

| Breakpoint | Behavior |
|------------|----------|
| **> 992px** | Full desktop layout, side-by-side grids |
| **768px - 992px** | Tablet layout, stacked columns |
| **< 768px** | Mobile layout, hamburger menu, single column |

---

## 🎯 SEO Tips

1. **Update meta tags** in each HTML file:
```html
<title>Your Name | AI Engineer Portfolio</title>
<meta name="description" content="Your description here">
```

2. **Add Open Graph tags** for social sharing:
```html
<meta property="og:title" content="Your Name - Portfolio">
<meta property="og:description" content="AI Engineer & Researcher">
<meta property="og:image" content="https://yourdomain.com/og-image.jpg">
```

3. **Add a favicon**:
```html
<link rel="icon" type="image/png" href="favicon.png">
```

---

## 🔧 Adding a Backend (Optional)

The contact form currently shows a success animation but doesn't send emails. To make it functional:

### Option A: Formspree (Easiest)
```html
<!-- Replace <form> tag in contact.html -->
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

### Option B: Netlify Forms
```html
<form name="contact" netlify>
```

### Option C: Custom Backend
Use Node.js, Python Flask, or any backend to handle form submissions.

---

## 🐛 Troubleshooting

| Issue | Solution |
|-------|----------|
| Particles not showing | Check if canvas element exists; ensure no JS errors in console |
| Animations not working | IntersectionObserver needs modern browser (Chrome 51+, Firefox 55+) |
| Mobile menu not opening | Check that `toggleMobileMenu()` function is loaded |
| Scroll not smooth | `scroll-behavior: smooth` works in modern browsers; add polyfill for older ones |
| Fonts not loading | Check internet connection (Google Fonts CDN required) |

---

## 📄 License

This project is open source. Feel free to use, modify, and distribute.

---

## 🙏 Credits

- **Fonts:** [Inter](https://fonts.google.com/specimen/Inter) by Google Fonts
- **Icons:** Emoji icons (replace with [Lucide](https://lucide.dev/) or [Font Awesome](https://fontawesome.com/) for production)
- **Design Inspiration:** Modern glassmorphism and dark UI trends

---

## 📬 Contact

Have questions or want to collaborate?

- Email: alex@example.com
- LinkedIn: linkedin.com/in/alex-chen
- GitHub: github.com/alexchen

---

> **Built with 💜, lots of ☕, and a passion for AI.**
