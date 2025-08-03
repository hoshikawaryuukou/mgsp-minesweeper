# mgsp-minesweeper

想做一個 ts 專案
踩地雷
他是一個多專案repo
有包含
1. 踩地雷核心 純邏輯
2. 踩地雷 終端包含 cli web electron
3. 彩帶地雷api


-----

- 套件管理器 : pnpm
- Monorepo 建置工具 : Turborepo
- 前端建置工具 : Vite
- 前端框架 : Vue 3
- UI 元件庫 : Vuetify 3
- 桌面應用程式框架 : Electron
- Schema 驗證庫 : Zod
- pinia
- vitest
- rollup
- netlify ?
- simple-git-hooks
- lint-staged

Code Quality
- 程式碼規範 : ESLint
- 程式碼格式化 : Prettier

-----

## 🧱 專案結構概覽（Monorepo）

```
root/
│
├── apps/
│   ├── cli/             # 命令列工具
│   ├── web/             # 瀏覽器遊戲
│   └── electron/        # 桌面 app
│
├── apis/
│   └── channel-a/       # 給合作方 A 的 API
│
├── packages/
│   ├── game-core/       # 純邏輯（盤面邏輯、遊戲流程）
│   └── utils/           # 共用工具（加密、驗證、格式轉換）
│
├── scripts/
│
├── package.json         # monorepo 總管
├── tsconfig.json        # 共用 TypeScript 設定
├── turbo.json           # 若使用 Turborepo 管理建置流程
└── README.md

```