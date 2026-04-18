# AT95 — Personal Portfolio

A clean, bilingual (EN/SR) developer portfolio built with vanilla HTML, CSS, and JavaScript. No frameworks, no build step — just fast, accessible, and deployable anywhere.

**[Live Demo →](https://at95bl.github.io/html-portfolio)** &nbsp;·&nbsp; **[Contact →](https://linktr.ee/at95)**

---

## Preview

| Dark Mode | Light Mode |
|-----------|------------|
| ![Dark](https://via.placeholder.com/480x280/0D1117/3B82F6?text=Dark+Mode) | ![Light](https://via.placeholder.com/480x280/F6F8FA/0969DA?text=Light+Mode) |

> Replace the placeholder images above with actual screenshots once deployed.

---

## Features

- **Bilingual** — full Serbian / English toggle, preference saved to `localStorage`
- **Dark / Light mode** — system-preference aware, toggle persists across pages
- **Responsive** — works on mobile, tablet, and desktop
- **Print-ready** — clean CV layout when printing or saving as PDF (nav and buttons hidden)
- **Zero dependencies** — plain HTML/CSS/JS; Font Awesome loaded via CDN for icons
- **Fast** — no bundler, no runtime, no JavaScript framework overhead

---

## Project Structure

```
html-portfolio/
├── index.html          # Main portfolio page (hero, skills, projects, education)
├── aboutMe.html        # Extended personal story
├── contact.html        # Social/contact links
├── images/
│   └── profileImage1.jfif
└── style/
    ├── index.css       # Main stylesheet + design system
    ├── aboutMe.css     # About page styles
    └── contact.css     # Contact page styles
```

---

## Getting Started

No build tools required.

```bash
git clone https://github.com/AT95BL/html-portfolio.git
cd html-portfolio
```

Then open `index.html` in your browser — or serve it locally:

```bash
# Python 3
python -m http.server 8080

# Node.js (npx)
npx serve .
```

---

## Deployment

The site is static and deploys to any host.

**GitHub Pages**
```bash
# Push to main — Pages serves from root automatically
git push origin main
```
Then enable GitHub Pages in your repo settings → Pages → Source: `main / (root)`.

**Netlify / Vercel** — drag the folder into the dashboard or connect the repo. No config needed.

---

## Design System

The portfolio uses a single CSS custom properties–based design system defined in `style/index.css`.

| Token | Dark | Light |
|---|---|---|
| `--bg` | `#0D1117` | `#F6F8FA` |
| `--bg-card` | `#161B22` | `#FFFFFF` |
| `--text` | `#E6EDF3` | `#1F2328` |
| `--accent` | `#3B82F6` | `#0969DA` |
| `--accent-2` | `#22D3EE` | `#0891B2` |

**Fonts** (Google Fonts, loaded via `@import`)
- Display / headings: [Syne](https://fonts.google.com/specimen/Syne)
- Body: [Plus Jakarta Sans](https://fonts.google.com/specimen/Plus+Jakarta+Sans)
- Code / labels: [DM Mono](https://fonts.google.com/specimen/DM+Mono)

---

## Customisation

**Swap out your photo**
Replace `images/profileImage1.jfif` with your own and update the `src` in `index.html`.

**Change accent color**
Edit `--accent` and `--accent-dark` in the `:root` block of `style/index.css`.

**Add a project**
Copy one of the `.project-card` blocks in `index.html` and fill in your details and tech tags.

**Add a language**
All bilingual content uses `.lang-en` / `.lang-sr` class pairs. Add a third class (e.g. `.lang-de`) and extend the CSS toggle logic and JS accordingly.

---

## Browser Support

| Browser | Support |
|---|---|
| Chrome / Edge 90+ | ✅ Full |
| Firefox 88+ | ✅ Full |
| Safari 14+ | ✅ Full |
| IE 11 | ❌ Not supported |

Uses `backdrop-filter` (frosted glass nav) — degrades gracefully to opaque background on unsupported browsers.

---

## Author

**Andrej Trožić** — Final-year Software Engineering student at ETF Banja Luka.

[![GitHub](https://img.shields.io/badge/GitHub-AT95BL-24292e?style=flat&logo=github)](https://github.com/AT95BL)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Andrej_Trožić-0077b5?style=flat&logo=linkedin)](https://www.linkedin.com/in/andrej-tro%C5%BEi%C4%87-57957122b/)
[![Linktree](https://img.shields.io/badge/Linktree-at95-43e660?style=flat&logo=linktree&logoColor=white)](https://linktr.ee/at95)

---

## License

This project is open source under the [MIT License](LICENSE). Feel free to use it as a template — a credit link back is appreciated but not required.
