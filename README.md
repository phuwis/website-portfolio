# Phuwis Watthana - Portfolio Website

A modern, responsive portfolio website showcasing IT Solutions Architect expertise with interactive features, smooth animations, and dark/light theme support.

## 🌟 Features

- **Responsive Design** — Works seamlessly on desktop, tablet, and mobile devices
- **Dark/Light Mode** — Theme toggle with localStorage persistence
- **Smooth Animations** — Scroll-triggered reveals, entrance animations, and transitions
- **Parallax Background** — Subtle depth effect on all sections
- **Interactive Components** — Accessible modals, keyboard navigation, and hover effects
- **JSON-Driven Content** — Easy content updates via `assets/data/portfolio.json`
- **Accessible** — WCAG 2.1 AA compliant with focus outlines and ARIA labels
- **No Dependencies** — Pure vanilla HTML, CSS, and JavaScript

## 📁 Project Structure

```
website-portfolio/
├── index.html              # Main HTML file
├── index.css               # Styling with CSS variables for theming
├── README.md               # This file
├── assets/
│   ├── data/
│   │   └── portfolio.json  # Portfolio content (projects, skills, contact)
│   └── images/
│       ├── 27002.jpg       # Logo image
│       └── parallax-abstract.svg  # Parallax background
```

## 🚀 Quick Start

### 1. **Local Development**
```bash
# Navigate to project directory
cd website-portfolio

# Start a local server (Python 3)
python -m http.server 8000

# Or use Node.js
npx http-server

# Open browser
# http://localhost:8000
```

### 2. **Edit Content**
Update `assets/data/portfolio.json` to customize:
- Hero section (name, tagline, CTA)
- Navigation menu
- Featured projects
- Skills (categorized)
- Contact information
- Footer copyright

Example:
```json
{
  "portfolio": {
    "hero": {
      "name": "Your Name",
      "tagline": "Your Professional Title",
      "cta": "Call to Action"
    },
    "projects": [
      {
        "id": 1,
        "title": "Project Name",
        "description": "Brief description",
        "link": "https://project-url.com"
      }
    ]
  }
}
```

### 3. **Update Logo & Images**
- Replace `assets/images/27002.jpg` with your logo
- Update logo path in `portfolio.json` → `"logo": "your-image.jpg"`

## 🎨 Customization

### Colors & Theme
Edit CSS variables in `index.css`:
```css
:root {
  --bg: #ffffff;           /* Light mode background */
  --text: #111111;         /* Light mode text */
  --accent: #000000;       /* Accent color */
  --shadow: 0 6px 18px...  /* Shadow effect */
}

[data-theme="dark"] {
  --bg: #0f0f0f;           /* Dark mode background */
  --text: #f0f0f0;         /* Dark mode text */
  /* ... */
}
```

### Fonts
Change in `body` CSS:
```css
body {
  font-family: 'Your Font', system-ui, sans-serif;
}
```

### Animations
Adjust animation timing in `index.css` (look for `@keyframes` and `animation:` properties):
- `fadeInUp`, `slideInLeft`, `scaleIn` for entrance effects
- `scroll-reveal` for scroll-triggered animations
- `spin` for theme toggle button

## ⌨️ Keyboard Navigation

- **Tab** — Navigate through focusable elements
- **Enter/Space** — Activate buttons and project cards
- **Arrow Keys** — Navigate nav menu (← →)
- **Escape** — Close project modal
- **Smooth Scroll** — Click any `#section` link

## 🌓 Theme System

- **Auto-detect** — Uses system preference on first visit
- **Manual Toggle** — Click moon/sun icon in header
- **Persistence** — Saves preference in localStorage
- **Smooth Transition** — 0.4s color fade when switching

## 📊 Sections

### Hero
- Full-screen welcome section
- Name, professional tagline, CTA button
- Fade-in animations on load

### Featured Projects
- Grid layout (responsive)
- Click to view modal details
- Hover effects with scale & shadow

### Skills
- Categorized skill items
- Centered layout
- Slide-in animations on scroll

### Contact
- Professional message
- Links to Email, LinkedIn, GitHub
- Email link copies address to clipboard

### Footer
- Copyright notice
- Minimal styling

## ♿ Accessibility

✅ **WCAG 2.1 AA Compliant**
- Semantic HTML (`<section>`, `<nav>`, `<header>`)
- Focus visible outlines (3px solid accent)
- ARIA labels on interactive elements
- Color contrast ≥ 4.5:1
- Keyboard-only navigation supported
- Screen reader friendly

## 🔧 Technical Stack

| Technology | Purpose |
|-----------|---------|
| HTML5 | Semantic structure |
| CSS3 | Styling, animations, theming |
| JavaScript (ES6) | Interactivity, state management |
| JSON | Content data source |
| SVG | Lightweight parallax background |

## 📦 Browser Support

- Chrome/Edge 88+
- Firefox 87+
- Safari 14+
- Mobile browsers (iOS Safari, Chrome Mobile)

## 🚀 Deployment

### GitHub Pages
```bash
# Push to GitHub
git add .
git commit -m "Portfolio updates"
git push origin main

# Enable GitHub Pages in Settings → Pages
# Select: Source = main branch, folder = root
```

### Netlify
```bash
# Install Netlify CLI
npm install -g netlify-cli

# Deploy
netlify deploy --prod
```

### Vercel
```bash
# Install Vercel CLI
npm install -g vercel

# Deploy
vercel --prod
```

## 📝 License

This portfolio is provided as-is for personal use. Feel free to customize and deploy.

**Attribution**: Built with vanilla HTML, CSS, and JavaScript.

## 📧 Contact & Support

For questions or improvements:
- **Email**: phuwisw@gmail.com
- **LinkedIn**: [Phuwis Watthana](https://www.linkedin.com/in/phuwis-watthana-8205a437b/)
- **GitHub**: [phuwis](https://github.com/phuwis)

---

**Last Updated**: December 2025
