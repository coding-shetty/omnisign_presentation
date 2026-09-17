# OmniSign — Hackathon Presentation Site 🎤🤟

> **Note: this is a companion / pitch-deck repo.** It contains the animated
> presentation website for **OmniSign**, not the sign-language translation app
> itself. If you're looking for the actual ASL translation tool, see
> [The actual OmniSign app](#the-actual-omnisign-app) below.

**OmniSign** is an AI-powered American Sign Language (ASL) translation web app
that breaks communication barriers between the deaf community and the hearing
world — using real-time hand tracking, on-device ML, and speech synthesis,
entirely in the browser. It was built for **KalpAIthon 2.0** at Kalpataru
Institute of Technology, Tiptur.

This repo hosts the scroll-driven, slide-style presentation site used to pitch
OmniSign to judges: hero, problem, solution, live-mockup demo, how-it-works,
features, tech stack, innovation, impact, future scope, team, and closing.

## ✨ What the deck covers

- **Problem** — 466M+ deaf people worldwide face daily communication barriers
- **Solution** — point your webcam at signing hands, get speech + text out
- **Pipeline** — webcam → MediaPipe hand landmarks → ASL recognition → phrase
  builder → Web Speech API output, all at 30+ FPS in-browser
- **Highlights** — sub-50ms recognition, 100% private (zero server calls),
  phrase builder, text-to-sign, ASL learning mode, works offline

## 🛠️ Tech stack

| Layer      | Tech                                                                 |
|------------|----------------------------------------------------------------------|
| Framework  | [React 19](https://react.dev/) + [TypeScript](https://www.typescriptlang.org/) |
| Build      | [Vite 7](https://vitejs.dev/) + `vite-plugin-singlefile`             |
| Styling    | [Tailwind CSS 4](https://tailwindcss.com/)                           |
| Animation  | [Framer Motion](https://motion.dev/), `react-type-animation`, `tsparticles` |
| Scroll FX  | `react-intersection-observer`, custom `useAnimations` hooks          |

## 🚀 Run it locally

Prerequisites: [Node.js](https://nodejs.org/) 18+ and npm.

```bash
npm install
npm run dev
```

Then open the URL Vite prints (usually http://localhost:5173).

Other scripts:

```bash
npm run build    # production build → dist/
npm run preview  # preview the production build locally
```

## 📁 Project structure

```
src/
├── App.tsx              # slide deck composition (lazy-loaded sections)
├── components/          # one component per slide + Navbar, ParticlesBackground …
├── hooks/               # shared animation variants (useAnimations)
├── utils/               # helpers (cn)
└── main.tsx / index.css # entry point + global styles
```

## 🤟 The actual OmniSign app

The live ASL translation tool (webcam → MediaPipe → speech) lives in its own
repo — **that's the main artifact**:

> **TODO:** link the OmniSign app repository / live demo URL here once it's
> pushed to GitHub.

If you maintain this profile: pushing the app itself matters more than this
deck for hiring purposes — the app is the stronger artifact.

## 👥 Team

Built at KalpAIthon 2.0 by **Diganth N** (Team Lead), **Yashas A** (AI/ML),
**Diganth A R** (Frontend), and **Vijeth HJ** (Integration).

## 📄 License

No license file is included yet — all rights reserved by the authors unless a
license is added.
