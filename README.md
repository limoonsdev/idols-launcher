<div align="center">

# 🎮 idols launcher

### A modern Windows desktop launcher built with Tauri + React.

![Tauri](https://img.shields.io/badge/Tauri-24C8DB?style=for-the-badge&logo=tauri&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)

</div>

---

## ✨ Overview

**idols launcher** is a Windows desktop application combining a React interface with a lightweight Tauri shell and the idols ecosystem backend.

The application provides a polished desktop experience with authentication, configurable appearance and game-related launcher workflows.

## 🏗️ Architecture

```text
┌──────────────────────┐
│      React UI        │
│  Pages / Components  │
└──────────┬───────────┘
           │
┌──────────▼───────────┐
│   State & API layer   │
│ Zustand · Axios · RTK │
└──────────┬───────────┘
           │
┌──────────▼───────────┐
│      Tauri shell     │
│     Windows app      │
└──────────┬───────────┘
           │
┌──────────▼───────────┐
│    idols backend     │
└──────────────────────┘
```

## 🛠️ Stack

- **Tauri** — desktop application shell
- **React 18** — interface
- **TypeScript** — application code
- **Vite** — frontend tooling
- **Zustand** — state management
- **TanStack Router / Query** — routing and data fetching
- **Framer Motion** — UI animation
- **Axios** — HTTP communication

## 🪟 Windows prerequisites

1. Node.js 18+
2. Rust + Cargo via rustup
3. Visual Studio Build Tools with Desktop C++ workload
4. WebView2

## 🚀 Development

```bash
npm install
npm run tauri dev
```

## 📦 Build

Frontend:

```bash
npm run build
```

Desktop application:

```bash
npm run tauri build
```

Tauri installers are generated under `src-tauri/target/release/bundle/`.

## ⚙️ Configuration

Application configuration lives primarily under `src/config/`.

Keep credentials, tokens and private endpoints out of version control.

## 📁 Project structure

```text
src/
├── components/     # UI components
├── pages/          # Application pages
├── state/          # Client state
├── config/         # Application configuration
└── ...

src-tauri/          # Tauri / Rust layer
installer/          # Windows installer tooling
```

## 📌 Status

This project is actively evolving. APIs, configuration and UI components may change between releases.

<div align="center">

**Built by Limoons.**

</div>
