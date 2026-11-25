# E-commerce Demo — 前端合併分支

這個分支把兩個專案並排放在一起，**所有檔案都是從原本的 `Full` 分支原樣複製，沒有修改任何程式碼**。

## 三個分支的關係

| 分支 | 內容 | 來源 |
| --- | --- | --- |
| `main` | StuLeave 學生請假系統完整原樣（保留完整 git 歷史） | `nasircy/WedDemo_StuLeave` 的 `Full` |
| `Full` | ZhiQi 志氣核銷系統完整原樣（保留完整 git 歷史） | `nasircy/WedDemo_ZhiQi` 的 `Full` |
| `frontend-combined` | 兩個專案並排放在不同資料夾（本分支） | 上面兩個分支的 `Full` |

## 本分支的資料夾

### `frontend-stuleave/`

Astro 前端（學生請假系統），來源為 StuLeave `Full`，原樣複製。

- 頁面與元件：`src/pages/`、`src/layouts/`、`src/components/`
- 靜態資源：`public/`、`src/public/`
- 設定：`astro.config.mjs`、`package.json`、`pnpm-lock.yaml`、`tsconfig.json`

### `frontend-zhiqi/`

Django 前端（志氣核銷系統），來源為 ZhiQi `Full`，原樣複製。

- 純前端 Demo：`frontend-demo/`（可直接用瀏覽器開啟 `index.html`）
- 模板：`templates/`
- 靜態資源：`static/`
- 樣式設定：`tailwind.config.js`

每個資料夾都保留原本的完整結構與設定檔，因此兩邊可以各自獨立執行、互不影響，也不會互相覆蓋同名檔案（例如 `app.css`、`app.js`、`favicon.svg`）。

## 執行方式

StuLeave（Astro）：

```bash
cd frontend-stuleave
pnpm install
pnpm dev
```

ZhiQi 純前端 Demo：直接用瀏覽器開啟 `frontend-zhiqi/frontend-demo/index.html`。

需要完整後端功能時，請切換到 `main`（StuLeave）或 `Full`（ZhiQi）分支。
