# GitHub Pages 部署指南
> ARZ AI Academy 課程招生頁

## 第一步：在 GitHub 建立新 Repo

1. 前往 https://github.com/new
2. Repository name 建議取：`arz-ai-academy` 或 `ai-course-landing`
3. 設為 **Public**（GitHub Pages 免費方案需要 Public）
4. **不要**勾選 Initialize with README（本地已有檔案）
5. 點 **Create repository**

## 第二步：推送到 GitHub（在專案目錄執行）

```bash
# 設定遠端（把 <你的帳號> 和 <repo名> 換成實際的）
git remote add origin https://github.com/tmparz/ai-course-landing.git

# 確認 branch 名稱（可能是 master 或 main）
git branch

# 推送（若是 master 就改成 master）
git push -u origin main
```

> 💡 若系統要求登入，用 GitHub 帳號密碼，或設定 [Personal Access Token](https://github.com/settings/tokens)

## 第三步：設定 GitHub Pages

1. 進入 repo 頁面 → **Settings**
2. 左側點 **Pages**
3. Source 選 **Deploy from a branch**
4. Branch 選 **main**（或 master），資料夾選 **/ (root)**
5. 點 **Save**

## 第四步：等待部署

- GitHub 會自動部署，約 1–3 分鐘
- 完成後網址會顯示在 Pages 設定頁：
  ```
  https://<你的帳號>.github.io/<repo名>/
  ```

## 日後更新

每次修改 `index.html` 後執行：

```bash
git add index.html
git commit -m "update: 說明修改內容"
git push
```

GitHub Pages 會自動重新部署，幾分鐘後生效。

## 注意事項

- 已建立 `.nojekyll` 檔案，避免 GitHub Pages Jekyll 干擾
- 頁面是純靜態 HTML，無需任何後端
- TailwindCSS 改為 Vanilla CSS，無需 build step
