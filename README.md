# 前端 Demo

這個分支放兩個原本獨立的**純前端 Demo**，各自使用獨立資料夾，程式碼完全沒有修改。沒有整合首頁，用下面路徑區分。

## 兩個 Demo 的路徑

| Demo | 入口路徑 | 說明 | 來源 |
| --- | --- | --- | --- |
| 學生請假系統 | `stuleave/index.html` | XX大學請假流程示範：申請、審核、統計與管理後台 | `nasircy/WedDemo_StuLeave` 的 `main` |
| 志氣企業核銷系統 | `zhiqi/index.html` | 企業費用核銷示範：單據、審核流程、預算統計與圖表 | `nasircy/WedDemo_ZhiQi` 的 `main` |

每個資料夾都保留原本的 `index.html`、`app.js`、`demo.css` 與 `static/`，所以同名的 `app.js`、`demo.css`、`static/` 不會互相覆蓋。

## 三個分支的關係

| 分支 | 內容 | 來源 |
| --- | --- | --- |
| `main` | StuLeave 學生請假系統完整版（保留完整 git 歷史） | `nasircy/WedDemo_StuLeave` 的 `Full` |
| `Full` | ZhiQi 志氣核銷系統完整版（保留完整 git 歷史） | `nasircy/WedDemo_ZhiQi` 的 `Full` |
| `frontend-combined` | 兩個純前端 Demo，按路徑區分（本分支） | 上面兩個 repo 的 `main` |

## 開啟方式

直接用瀏覽器開啟：

- `stuleave/index.html`
- `zhiqi/index.html`

兩邊都是純靜態頁面，不需要安裝套件或啟動後端，資料存放在瀏覽器本機（localStorage）。

若用本機伺服器（建議，避免瀏覽器對 `file://` 的限制）：

```bash
python -m http.server 8000
```

然後開啟：

- `http://localhost:8000/stuleave/index.html`
- `http://localhost:8000/zhiqi/index.html`

完整後端版本請切換到 `main`（StuLeave / Astro）或 `Full`（ZhiQi / Django）分支。
