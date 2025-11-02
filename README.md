# 🤖 AutoFAQs — Frontend

Beautiful, simple React frontend for the AutoFAQs project — a small FAQ generator and demo app.

Live demo: http://Punit-Koujalgi.github.io/faq-frontend

---

## ✨ What is this?

AutoFAQs is a compact React single-page app where a user can enter context (say from there website) and hit evaluate to generate a set of FAQ questions that the users of their website might have.

This repository contains the frontend only. It can be used as a static site (see `build/` and `public/`) or run locally for development.

## 🚀 Key features

- Lightweight React app (Create React App)
- Minimal dependencies: React, Bootstrap, axios
- Organized components under `src/components` with small UI types in `src/components/types`
---

## 🧰 Tech stack

- React 17 (Create React App)
- Bootstrap 5
- axios for HTTP (used when extending to a backend)

See `package.json` for exact versions.

---

## 📦 Quick start — clone, install, run

1. Clone the repo

```bash
git clone https://github.com/Punit-Koujalgi/faq-frontend.git
cd faq-frontend
```

2. Install dependencies

```bash
npm install
```

3. Run in development mode (hot reload)

```bash
npm start
```

Open http://localhost:3000 in your browser. The app uses `react-scripts` and the start script includes `--openssl-legacy-provider` to avoid some legacy OpenSSL builds on older Node versions.

4. Build for production

```bash
npm run build
```

The optimized static output will be in the `build/` folder. You can serve it with any static host or use GitHub Pages.

5. Deploy to GitHub Pages (optional)

This project includes a `deploy` script that uses `gh-pages`. Before running it, install `gh-pages` if you plan to use it.

```bash
# install if you don't have it
npm install --save-dev gh-pages

# build + publish
npm run deploy
```

## 📁 Project structure (important files)

- `public/` — static public files used by the app
- `build/` — generated production build (committed here for GitHub Pages hosting)
- `src/` — source code
	- `App.js`, `index.js` — entry points
	- `components/` — UI components and small type variants
	- `utilities/Data.js` — data loader / helpers
- `data/passages.js` and `passages.txt` — source content for the FAQ/passages
- `package.json` — scripts and dependencies

---

Currently, the project is deployed with Github Actions to Github pages!

