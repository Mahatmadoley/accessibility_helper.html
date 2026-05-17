# AccessAid — Accessibility Companion Website

> A free, browser-based accessibility toolkit designed to make the digital world easier and more inclusive for people with disabilities.

---

## 📖 Description

**AccessAid** is a lightweight, single-file HTML website that provides a suite of accessibility tools — all running entirely in the browser, with no backend, no data collection, and no installation required. It was designed with the needs of visually impaired, hearing impaired, motor-disabled, and cognitively diverse users in mind, following **WCAG 2.1 AA** accessibility standards throughout.

The site includes a live accessibility toolbar that lets any visitor instantly customise their experience — switching to high contrast, larger text, a dyslexia-friendly font, or reduced motion — without needing to change system settings.

---

## ✨ Features

### 🛠 Accessibility Toolbar
Always visible at the top of the page, allowing users to toggle:
- **Larger Text** — increases base font size across the entire site
- **High Contrast Mode** — switches to a black/white high-contrast colour scheme
- **Dyslexia Font** — loads OpenDyslexic, a font designed to improve readability for dyslexic users
- **Reduce Motion** — disables all CSS transitions and animations
- **Reset All** — restores all settings to their defaults

### 🔊 Text to Speech
- Paste or type any text and have it read aloud instantly
- Choose from all browser-available voices and languages
- Adjustable playback speed (0.5× to 2.0×)
- Stop playback at any time
- Fully powered by the Web Speech API — no data leaves the device

### 🎨 Colour Contrast Checker
- Pick foreground (text) and background colours using a colour picker or hex code input
- Instantly calculates the WCAG contrast ratio
- Shows pass/fail results for:
  - Large text AA (≥ 3:1)
  - Normal text AA (≥ 4.5:1)
  - Normal text AAA (≥ 7:1)
- Live preview of how the colour combination looks

### 🔠 Font Size Tester
- Drag a slider to preview text at sizes from 10px to 40px
- Quick presets: 16px (Body), 18px (Comfort), 22px (Large), 28px (Extra Large)
- Switch between font families: Atkinson Hyperlegible, sans-serif, serif, and monospace

### 📚 Resource Directory
Curated links for:
- Visual impairment (NVDA screen reader)
- Hearing impairment (National Association of the Deaf)
- Motor/physical disabilities (AbilityNet)
- Cognitive & learning differences (Understood.org)
- Web accessibility standards (W3C WAI / WCAG)
- Disability helplines including India's NHFDC (1800-11-1921, toll-free)

---

## ♿ Accessibility Standards

This project is built to be accessible by design, not as an afterthought:

- **Skip to main content** link for keyboard and screen reader users
- All interactive elements have proper `aria-label`, `aria-pressed`, `aria-live`, and `role` attributes
- Keyboard navigable — every feature works without a mouse
- Focus indicators are clearly visible on all interactive elements
- Semantic HTML5 landmarks (`<header>`, `<main>`, `<nav>`, `<footer>`, `<section>`)
- Colour contrast meets WCAG 2.1 AA throughout
- Uses **Atkinson Hyperlegible** — a font designed specifically for low vision readers

---

## 🚀 Deployment (Netlify)

This project is a single HTML file — no build step required.

### Option 1: Drag & Drop
1. Rename `accessibility_helper.html` → `index.html`
2. Go to [netlify.com](https://netlify.com) and log in
3. Drag and drop the `index.html` file onto the Netlify dashboard
4. Your site is live instantly at a `*.netlify.app` URL

### Option 2: GitHub + Netlify (Recommended)
1. Rename the file to `index.html`
2. Push it to a GitHub repository
3. In Netlify: **Add new site → Import from GitHub**
4. Select your repo — leave all build settings blank
5. Click **Deploy**

Future updates are deployed automatically when you push to GitHub.

---

## 🗂 Project Structure

```
accessaid/
│
└── index.html        # The entire application — HTML, CSS, and JS in one file
```

No dependencies to install. No build tools. No frameworks. Just open `index.html` in any modern browser.

---

## 🌐 Browser Support

| Browser | Support |
|---|---|
| Chrome / Edge | ✅ Full (best TTS voice selection) |
| Firefox | ✅ Full |
| Safari | ✅ Full |
| Mobile browsers | ✅ Responsive layout supported |

> **Note:** Text-to-speech voice availability depends on the operating system and browser. Chrome on Windows/macOS typically offers the widest selection.

---

## 🛡 Privacy

- **No data collection** — all tools run locally in your browser
- **No cookies or tracking**
- **No external API calls** — the only external resources are Google Fonts (for typography) and the OpenDyslexic font (loaded only when the dyslexia mode is activated)

---

## 📄 License

This project is open source and free to use, modify, and distribute.

---

## 🙌 Contributing

Contributions are welcome! Ideas for future features:
- Screen magnifier tool
- Keyboard shortcut guide
- Reading ruler / focus line overlay
- Colour blindness simulator
- Dark mode toggle

Feel free to open an issue or submit a pull request.

---

*Built with accessibility at its heart — for every person, on every device.*
