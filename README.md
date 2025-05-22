# next-clean-view-config
Configuration for VSCode to streamline the project view by hiding build and dependency folders in Next.js/React projects.

# VSCode Clear Dir — Clean Explorer for Next.js/React Projects

🚀 Hide irrelevant folders and files in VSCode to improve code navigation and reduce visual noise — perfect for code reviews, focused development, or preparing a project for sharing.

---

## ✨ What It Hides

This config removes clutter from the file explorer by hiding:

### 🛠️ Build & Cache
- `node_modules/`, `.next/`, `.turbo/`, `.cache/`, `dist/`, `build/`, `out/`, `coverage/`

### ⚙️ Tooling & Config Files
- Git: `.git`, `.gitignore`
- Next.js: `next.config.js`, `next-env.d.ts`
- TypeScript: `tsconfig.json`
- Linters & PostCSS: `eslint.config.mjs`, `postcss.config.mjs`
- Package managers: `package.json`, `package-lock.json`, `yarn.lock`, `pnpm-lock.yaml`, `bun.lock`

### 📄 Logs & Docs
- `*.log`, `README.md`
- System files like `.DS_Store`

---

## 📂 Example `settings.json`

Place this inside `.vscode/settings.json`:

```json
{
  "files.exclude": {
    "**/node_modules": true,
    "**/.next": true,
    "**/.turbo": true,
    "**/dist": true,
    "**/.cache": true,
    "**/coverage": true,
    "**/build": true,
    "**/out": true,
    "**/.DS_Store": true,
    "**/.git": true,
    "**/.gitignore": true,
    "**/*.log": true,
    "**/next-env.d.ts": true,
    "**/next.config.js": true,
    "**/next.config.ts": true,
    "**/tsconfig.json": true,
    "**/package-lock.json": true,
    "**/yarn.lock": true,
    "**/pnpm-lock.yaml": true,
    "**/bun.lock": true,
    "**/package.json": true,
    "**/postcss.config.mjs": true,
    "**/eslint.config.mjs": true,
    "**/README.md": true
  }
}
