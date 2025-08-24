# 🍸 Mojito — React + Vite + GSAP + Tailwind

A stunning, scroll-driven Mojito website built with React (Vite), Tailwind CSS, and GSAP. This project showcases advanced animation techniques: SplitText-style reveals, buttery parallax, ScrollTrigger timelines, pinned sections, scroll-synced video, image masking, an animated carousel, and seamless cross-section narratives. Fully responsive and production-ready.

## ✨ Highlights

- **SplitText-style reveals** for headlines & ingredient lists  
  > Uses GSAP’s SplitText (Club GreenSock) if available, with a graceful fallback to a free splitter (e.g., SplitType).
- **Parallax & ScrollTrigger** scenes with scrubbed timelines
- **Pinned sections** to lock focus during key moments
- **Scroll-synced video** for cinematic storytelling
- **Image masking on scroll** (clip-path / CSS mask with GSAP updates)
- **Custom animated carousel** (drag/auto-play + momentum)
- **Section-spanning timelines** that stitch the whole story together
- **Responsive UI** that adapts cleanly from mobile to ultrawide

---

## 🧱 Tech Stack

- **React + Vite** for lightning-fast dev with HMR
- **Tailwind CSS** for utility-first styling
- **GSAP 3 + ScrollTrigger** (and optional **SplitText**)
- **TypeScript (optional)** for type-safe production apps
- **ESLint + Prettier** for clean, consistent code

---

## 🚀 Quick Start

```bash
# 1) Create the project
npm create vite@latest mojito -- --template react

# or with TypeScript
# npm create vite@latest mojito -- --template react-ts

cd mojito

# 2) Install deps
npm i
npm i gsap
npm i -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```


## 🛠 Scripts

```bash
npm run dev       # Start Vite dev server with HMR
npm run build     # Production build
npm run preview   # Preview the production build locally
```

---


## 🌐 Deployment

- **Vercel**: Zero-config for Vite. Push to a repo and import.
- **Netlify**: Build command `npm run build`, publish directory `dist/`.
- **Static Hosts**: Serve the `dist/` folder (remember proper SPA fallback).

---

## 📋 Accessibility & Performance Tips

- Respect `prefers-reduced-motion` (skip heavy timelines when on)
- Use `will-change` sparingly; stick to transform/opacity
- Lazy-load media and leverage modern image formats
- Debounce/RAF any scroll-linked DOM reads/writes
- Keep timelines paused by default and activate via `ScrollTrigger`

---

## 🔐 Licensing Notes

- **GSAP** is free for most use cases; **SplitText** is a Club GreenSock plugin and requires a license for production. If you don’t have one, use a free text splitter (e.g., SplitType) and identical GSAP timelines.

---


## 🙌 Credits

Built with ❤️ using **React + Vite**, **Tailwind CSS**, and **GSAP (ScrollTrigger)**. Cheers! 🍹
