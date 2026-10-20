# 🛒 Project 29: Shopping List — MetaBox Intern Challenge

> *"A list that remembers."*

A sleek, zero-dependency Shopping List web application built for the **MetaBox Technology Intern Challenge** (60-minute build). Designed with an Apple iOS/macOS dark liquid-glass aesthetic, instant state reactivity, and full `localStorage` persistence.

🔗 **Live Demo (Vercel):** [https://your-vercel-url.vercel.app](https://your-vercel-url.vercel.app)  
💻 **Repository:** [https://github.com/azharsoopun/metabox-internship](https://github.com/azharsoopun/metabox-internship)

---

## ✨ Core Features & Requirements Implemented

- **Add Items with Quantity:** Rapidly add items with custom quantities (`min="1"`). Automatically merges duplicate unticked items by summing their quantities and includes inline `+` / `−` quantity steppers on every row.
- **Smart Auto-Sorting (Tick Off Items):** Ticking an item smoothly transitions it to the bottom of the list with a strikethrough state. Unticking an item restores it to its original chronological position at the top.
- **Clear Ticked Items:** Dedicated **"Clear ticked"** button with a live counter badge that purges completed items in one click (automatically disabled when no items are ticked).
- **Persistent State (`localStorage`):** Every mutation (adding, ticking/unticking, incrementing/decrementing quantity, and clearing) immediately syncs to `localStorage` (`metabox_shopping_list_v1`) with `try/catch` safety.
- **Stretch Goal — WhatsApp-Friendly Export:** One-click **"Copy for WhatsApp"** button formats the shopping list using native WhatsApp Markdown (`*bold*` headers and `~strikethrough~` for picked-up items) and copies it directly to the clipboard with visual confirmation.

---

## 🎨 UI / UX Highlights

- **Apple Liquid Glass Aesthetic:** Translucent frosted-glass container (`backdrop-filter: blur(28px)`), subtle ambient radial gradients, and macOS traffic-light header accents.
- **Live Progress Tracking:** Dynamic header counter and animated progress bar (`#30D158` Apple Green) that updates as items are picked up.
- **Keyboard-First Workflow:** Auto-refocuses the item name input after submission for rapid, frictionless entry.
- **XSS Protection:** User inputs are safely sanitized before DOM injection.

---

## 🛠️ Tech Stack

- **HTML5** (Semantic structure)
- **Tailwind CSS** (via CDN for zero-build, instant deployment)
- **Vanilla JavaScript (ES6+)** (State management, DOM rendering, `localStorage`, and Clipboard API)
- **Deployment:** GitHub + Vercel

---

## 🚀 Running Locally

No build step, `node_modules`, or API keys required. Everything runs directly in the browser:

1. Clone the repository:
   ```bash
   git clone [https://github.com/azharsoopun/metabox-internship.git](https://github.com/azharsoopun/metabox-internship.git)
