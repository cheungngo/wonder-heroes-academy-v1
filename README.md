# 🦊 Wonder Heroes Academy

**A gamified cognitive training platform for children, designed to make brain exercises feel like magical adventures.**

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

---

## 🌟 Overview

Wonder Heroes Academy is a mobile-first web application that presents cognitive training exercises as "Daily Missions" within a whimsical, hero-training narrative. Children progress through a series of mini-games that target core cognitive skills such as working memory, attention, pattern recognition, inhibitory control, and task switching.

The platform is built as a lightweight, standalone collection of HTML files — no build tools, no frameworks, no server required. Simply open in a browser and play.

Powered by **Cheung Ngo Medical (翱翔醫療)**.

---

## 🎮 Missions

| # | Mission | Cognitive Target | Description |
|---|---------|-----------------|-------------|
| 2 | 🧪 Magic Brew Buddies | Working Memory | Mix glowing potions for hungry monster customers by remembering recipe sequences. |
| 3 | 🌈 Rainbow Rule Race | Inhibitory Control | Tap the correct rule before the rainbow timer runs out — rules change to keep you on your toes. |
| 4 | 💎 Glowy Memory Gems | Visuospatial Memory | Remember and reproduce glowing patterns on a treasure grid. |
| 5 | 🦕 Dino Train Rescue | Planning & Flexibility | Swipe track switches so cute dinosaurs reach the correct stations. |
| 6 | 🌟 Meteor Buddy Watch | Sustained Attention | Tap special shooting stars before they zoom away while ignoring distractors. |
| 7 | 🐠 Ocean Treasure Hunt | Visual Search | Find all the glowing fish hiding in a busy, animated reef scene. |
| 8 | 🎉 Echo Echo Party | N-Back Memory | Tap when the dancing animal matches the one from two steps ago. |

---

## ✨ Features

- **Mobile-First Design** — Optimized for phones and tablets with touch-friendly hit targets and responsive layouts.
- **Multilingual Support** — Switch between English (🇺🇸) and Traditional Chinese (🇹🇼) with a single tap.
- **Zero Dependencies** — Pure HTML, CSS, and vanilla JavaScript. No npm, no bundlers, no external frameworks.
- **Immersive UI** — Animated starfield, floating particles, gradient backgrounds, and a bouncing mascot create an engaging atmosphere.
- **Accessible Navigation** — Large card-based mission selector with clear icons, descriptions, and color-coded categories.
- **Offline-Ready** — All assets are self-contained. No network requests are required after initial page load.
- **Lightweight** — The entire hub page is a single HTML file under 15 KB.

---

## 🚀 Getting Started

### Quick Start

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-org/wonder-heroes-academy.git
   cd wonder-heroes-academy
   ```

2. **Open the hub page:**

   ```bash
   open index.html
   ```

   Or simply double-click `index.html` in your file manager. Any modern browser will work.

3. **Tap a mission card** to launch that game.

### Serving Locally (Optional)

If you prefer to serve via a local HTTP server:

```bash
# Python 3
python -m http.server 8000

# Node.js (npx)
npx serve .
```

Then visit `http://localhost:8000` in your browser.

---

## 📁 Project Structure

```
wonder-heroes-academy/
├── index.html          # Main hub / mission selector
├── game2.html          # Mission 2 — Magic Brew Buddies
├── game3.html          # Mission 3 — Rainbow Rule Race
├── game4.html          # Mission 4 — Glowy Memory Gems
├── game5.html          # Mission 5 — Dino Train Rescue
├── game6.html          # Mission 6 — Meteor Buddy Watch
├── game7.html          # Mission 7 — Ocean Treasure Hunt
├── game8.html          # Mission 8 — Echo Echo Party
├── README.md           # This file
└── LICENSE             # License file
```

Each `game*.html` file is a fully self-contained game — all HTML, CSS, and JavaScript are embedded in a single file for maximum portability.

---

## 🛠 Technical Details

### Technology Stack

- **HTML5** — Semantic structure and Canvas API (in game files)
- **CSS3** — Animations, gradients, `backdrop-filter`, CSS custom properties
- **Vanilla JavaScript** — ES6+, no external libraries

### Browser Support

| Browser | Supported |
|---------|-----------|
| Chrome / Edge 90+ | ✅ |
| Safari 15+ | ✅ |
| Firefox 95+ | ✅ |
| Samsung Internet 16+ | ✅ |
| IE 11 | ❌ |

### Design Principles

- **Single-file architecture** — Each page is self-contained for easy distribution, embedding, and offline use.
- **No build step** — What you see in the repo is what runs in the browser.
- **Progressive difficulty** — Games are designed to adapt or be arranged in increasing cognitive demand.
- **Child-safe** — No ads, no tracking, no external network calls, no data collection.

---

## 🌐 Localization

The hub supports runtime language switching between:

- 🇺🇸 **English** (default)
- 🇹🇼 **繁體中文** (Traditional Chinese)

To add a new language, extend the `TX` object in the `<script>` section of `index.html`:

```javascript
const TX = {
  en: { /* ... */ },
  zh: { /* ... */ },
  ja: {
    bubble: '今日もトレーニングしよう、ヒーロー！',
    title: 'ワンダーヒーローズアカデミー',
    // ... add all keys
  }
};
```

Then add a corresponding button in the language dropdown.

---

## 🎨 Customization

### Changing the Mascot

Find the `.mascot` element in `index.html` and replace the emoji:

```html
<div class="mascot">🦊</div>  <!-- Change to 🐱, 🐶, 🦁, etc. -->
```

### Adjusting the Color Theme

The background gradient is defined on the `body` element:

```css
body {
  background: linear-gradient(180deg, #0a0a2e 0%, #1a1050 20%, #2d1b69 45%, #4a2c8a 70%, #6b3fa0 100%);
}
```

Modify these color stops to change the overall mood.

### Adding New Missions

1. Create a new `game*.html` file.
2. Add an entry to the `games` array in the `TX` object for each supported language.
3. Add a corresponding color pair to the `CARD_COLORS` array.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 🏥 About

Wonder Heroes Academy is developed and maintained by **Cheung Ngo Medical** as part of an initiative to provide accessible, evidence-informed cognitive training tools for children.

---

<p align="center">
  <sub>⚕️ Powered by <strong>Cheung Ngo Medical</strong></sub><br>
  <sub>Made with 💜 for little heroes everywhere</sub>
</p>
