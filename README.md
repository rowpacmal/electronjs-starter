# Electron.js Starter

A minimal boilerplate for building modern desktop applications using **Electron**, **React**, **Vite**, and **TypeScript**.

---

## ✨ Features

* ⚡ Lightning-fast development with **Vite**
* ⚛️ Modern UI with **React 19**
* 🧠 Type-safe code with **TypeScript**
* 🚀 Cross-platform builds with **Electron Builder**

---

## 📦 Project Structure

```
electronjs-starter/
├── src/
│   ├── electron/         # Main Electron process
│   └── ui/               # React frontend
├── package.json
└── vite.config.ts
```

---

## 🚀 Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/your-username/electronjs-starter.git
cd electronjs-starter
```

### 2. Install dependencies

```bash
npm install
```

### 3. Run in development mode

```bash
npm run dev
```

This will start both:

* The Vite-powered React renderer
* The Electron main process

---

## 🛠 Scripts

| Command              | Description                                |
| -------------------- | ------------------------------------------ |
| `npm run dev`        | Run Electron + Vite in development         |
| `npm run lint`       | Run ESLint on the project                  |
| `npm run preview`    | Preview Vite build (renderer only)         |
| `npm run dist:mac`   | Build `.dmg` for macOS (ARM64)             |
| `npm run dist:win`   | Build `.exe` for Windows (x64)             |
| `npm run dist:linux` | Build AppImage or similar for Linux (x64)  |

---

## 📁 Electron & Vite Setup

This template separates the main and renderer processes cleanly:

* Electron main process is written in TypeScript, located at `src/electron/`
* React renderer is served via Vite and lives in `src/ui/`
* Build outputs are managed by `tsc`, `vite build` and `electron-builder`

---

## 📤 Packaging

We use `electron-builder` for creating distributables:

```bash
npm run dist:mac     # macOS
npm run dist:win     # Windows
npm run dist:linux   # Linux
```

Update `build` settings in `electron-builder.json` for custom configurations like app icons, file associations, etc.

---

## 🧑‍💻 Author

🐥 [@rowpacmal](https://github.com/rowpacmal)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
