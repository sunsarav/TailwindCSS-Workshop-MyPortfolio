# Tailwind CSS Workshop — Developer Portfolio Landing Page

A responsive personal portfolio landing page built with Tailwind CSS 

---

## 🎯 Workshop Goal

Design and build a landing page from scratch using Tailwind CSS utility classes — focusing on layout, spacing, typography, and responsiveness.

---

## 🖥️ What I Built

A **personal developer portfolio** with the following sections:

| Section | Description |
|---|---|
| Navbar | Sticky navigation with logo and smooth-scroll links |
| Hero | Headline, About Me modal trigger, CTA buttons, and quick stats |
| Skills | Tech stack displayed in a responsive grid |
| Projects | Project cards with descriptions and tech tags |
| Contact | Email CTA and social links |

---

## ✅ Requirements Met

- [x] Tailwind utility classes used throughout
- [x] Fully responsive (mobile → tablet → desktop)
- [x] Clean layout with consistent spacing
- [x] Good typography hierarchy
- [x] Creative design with custom colors and animations

---

## 🔑 Key Tailwind Concepts Used

**Responsive prefixes**
Classes like `text-5xl md:text-7xl` apply different styles at different screen sizes. Tailwind is mobile-first — the base class applies on mobile, and `md:` overrides it on medium screens and above.

**Flexbox layout**
`flex items-center justify-between` is used in the navbar to push the logo to the left and links to the right.

**Grid layout**
`grid grid-cols-2 md:grid-cols-4 gap-4` creates a 2-column grid on mobile that expands to 4 columns on desktop — no media queries needed.

**Spacing**
`px-6 py-24 mb-6 mt-3` — `p` is padding, `m` is margin, `x`/`y` are horizontal/vertical. The number is × 4px (so `py-24` = 96px).

**Custom hex colors**
`bg-[#1E293B]` — bracket notation lets to use any hex color not in Tailwind's default palette.

**Conditional visibility**
`hidden md:flex` hides an element on mobile and shows it as flex on medium+ screens. Used for the desktop navbar links.

**Hover + transitions**
`hover:bg-indigo-400 transition-colors` — `hover:` applies a style on mouse-over, `transition-colors` animates the change smoothly.

**Opacity modifier**
`bg-indigo-500/10` sets the background to indigo at 10% opacity — great for subtle tag pills.

---

## 🎨 Design Decisions

- **Color palette:** Deep navy `#0A0F1E` base, electric indigo `#6366F1` accent, slate body text
- **Logo font:** Playfair Display (Google Fonts) with a purple-to-indigo gradient applied via `background-clip: text`
- **Interactive element:** A pulsing ⓘ icon that opens an About Me modal on click
- **Scroll animations:** `IntersectionObserver` adds a `.visible` class when sections enter the viewport, triggering a fade-in slide-up effect

---

## 🛠️ Tech Used

- HTML5
- Tailwind CSS (CDN)
- Vanilla JavaScript (modal toggle + scroll reveal)
- Google Fonts — Playfair Display

---

## 🚀 How to Run

1. Download `index.html`
2. Open it directly in any browser — no build step needed
3. Tailwind loads from CDN, so an internet connection is required

## 🌐 Live Demo

👉 [View Portfolio](https://sunsarav.github.io/TailwindCSS-Workshop-MyPortfolio/)

