# 🎌 Anime Vault

A modern anime discovery platform that lets users browse and explore popular anime series and movies through an elegant, responsive interface with smooth animations and infinite scrolling. Built with **Next.js**, **TypeScript**, and **Tailwind CSS**, with live data pulled from the Shikimori anime API.

🌐 **Live Demo:** [anime-vault-site.netlify.app](https://anime-vault-site.netlify.app/)
📂 **Repository:** [github.com/rkazumovi/Anime-Vault](https://github.com/rkazumovi/Anime-Vault)

![Next.js](https://img.shields.io/badge/Next.js-14-black?logo=next.js)
![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?logo=typescript&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3-38B2AC?logo=tailwindcss&logoColor=white)
![Framer Motion](https://img.shields.io/badge/Framer%20Motion-11-black?logo=framer)

---

## Overview

Anime Vault gives anime fans a centralized place to discover popular anime by browsing titles, scores, episode counts, and format (TV series vs. movie). The initial catalog is seeded with a curated set of well-known titles, and additional anime is loaded live from the **Shikimori API** as the user scrolls, using a Next.js Server Action combined with an intersection observer for a seamless infinite-scroll experience — no pagination buttons required.

## ✨ Features

- 🎬 Browse popular anime series and movies with cover art, score, episode count, and type
- ♾️ Infinite scroll — new anime loads automatically from the Shikimori API as you scroll, powered by a Next.js Server Action and `react-intersection-observer`
- ⭐ Ratings/scores and episode counts displayed per title
- 🎞️ Smooth entrance animations for each anime card via Framer Motion, staggered by card index
- 📱 Fully responsive grid layout (1 to 4 columns depending on screen size)
- ⚡ Server-rendered with Next.js App Router for fast initial loads
- 🎨 Modern, dark, anime-inspired visual design

## 🛠️ Built With

**Languages**
- TypeScript — type-safe application and component logic
- CSS — styling via Tailwind CSS

**Frameworks / Libraries**
- [Next.js](https://nextjs.org/) 14 (App Router) — React framework with Server Components and Server Actions
- [React](https://react.dev/) 18 — UI library
- [Tailwind CSS](https://tailwindcss.com/) — utility-first styling
- [Framer Motion](https://www.framer.com/motion/) — card entrance animations
- [react-intersection-observer](https://www.npmjs.com/package/react-intersection-observer) — viewport detection to trigger infinite-scroll loading

**External API**
- [Shikimori API](https://shikimori.one/api/doc) — live anime catalog data (titles, cover art, scores, episode counts), fetched server-side via a Next.js Server Action

**Build Tools & Tooling**
- [PostCSS](https://postcss.org/) + [Autoprefixer](https://github.com/postcss/autoprefixer) — CSS processing
- [ESLint](https://eslint.org/) — linting and code consistency

**Deployment**
- [Netlify](https://www.netlify.com/) — hosting and continuous deployment

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or later recommended)
- npm or yarn
- Git

### Installation

1. Clone the repository
   ```bash
   git clone https://github.com/rkazumovi/Anime-Vault.git
   cd Anime-Vault
   ```

2. Install dependencies
   ```bash
   npm install
   ```

3. Start the development server
   ```bash
   npm run dev
   ```

4. Open your browser and navigate to `http://localhost:3000`

### Build for Production

```bash
npm run build
npm run start
```

### Lint

```bash
npm run lint
```

## 📁 Project Structure

```
Anime-Vault/
├── app/
│   ├── action.tsx        # Server Action fetching anime data from the Shikimori API
│   ├── layout.tsx        # Root layout
│   ├── page.tsx          # Home page
│   └── globals.css       # Global styles
├── components/
│   ├── Hero.tsx           # Landing hero section
│   ├── AnimeCard.tsx      # Individual anime card with entrance animation
│   ├── LoadMore.tsx       # Infinite-scroll trigger and card loader
│   ├── MotionDiv.tsx      # Framer Motion wrapper component
│   └── Footer.tsx
├── public/                # Static assets (icons, images)
├── next.config.js
├── tailwind.config.ts
├── tsconfig.json
└── package.json
```

## 📱 Responsive Design

The anime grid adapts from a single column on mobile up to four columns on large desktop screens, with a mobile-first layout throughout.

## 📦 Deployment

This project is deployed with **Netlify** and is live at:
👉 [anime-vault-site.netlify.app](https://anime-vault-site.netlify.app/)

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

1. Fork the repository
2. Create a feature branch
   ```bash
   git checkout -b feature/new-feature
   ```
3. Commit your changes
   ```bash
   git commit -m "Add new feature"
   ```
4. Push to your branch
   ```bash
   git push origin feature/new-feature
   ```
5. Open a Pull Request

## 📄 License

This project is intended for educational and portfolio purposes. Anime data is provided via the [Shikimori API](https://shikimori.one/api/doc) and is subject to that service's terms of use. Anime titles, images, and related media are property of their respective copyright holders.

---

<p align="center">⭐ If you found this project interesting, consider giving it a star on GitHub!</p>
