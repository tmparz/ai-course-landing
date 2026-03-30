# 20260331-01 ARZ AI Academy 招生頁 UI/UX 優化計畫

## 背景
現有 index.html 以 TailwindCSS CDN 為基礎，設計功能完整但風格偏嚴肅，缺乏：
- 行動版漢堡選單
- 滾動動畫
- 社交證明（學員心聲）
- 痛點共鳴區塊
- 無障礙設計（a11y）

## 設計策略（來自 UI/UX Pro Max）

| 項目 | 選擇 | 理由 |
|------|------|------|
| 風格 | Organic Biophilic + Soft UI | 親民、溫暖、符合目標女性受眾 |
| 字體 | Varela Round + Nunito Sans | 圓潤友善，降低技術恐懼感 |
| 主色 | Forest Green #2D4F3E | 延伸品牌原色，增添自然溫暖感 |
| 輔色 | Amber #F59E0B | CTA 強調用色，高對比引導點擊 |
| 結構 | Hero→痛點→導師→課程→社交證明→定價→Footer | 轉換漏斗最佳架構 |

## 執行內容
1. ✅ 全面重寫 index.html（Vanilla CSS + 設計 token）
2. ✅ 行動版漢堡選單（RWD）
3. ✅ IntersectionObserver fade-up 動畫
4. ✅ 新增「痛點共鳴」區塊
5. ✅ 新增「學員心聲」（Testimonials）
6. ✅ prefers-reduced-motion 無障礙支援
7. ✅ SEO meta tags（title/description/og）
8. ✅ .nojekyll 建立（GitHub Pages）
9. ⏳ git init + push 到 GitHub
10. ⏳ GitHub Pages 設定

## GitHub Pages 部署步驟
```bash
git init
git add .
git commit -m "feat: 優化 UI/UX，準備 GitHub Pages 部署"
# 在 GitHub.com 建立新 repo
git remote add origin https://github.com/<你的帳號>/<repo名>.git
git push -u origin main
# 到 repo Settings → Pages → Branch: main / root → Save
```

## 驗收標準
- [ ] 手機版選單正常開關
- [ ] 滾動時元素依序淡入
- [ ] 所有 CTA 按鈕可點擊（cursor: pointer）
- [ ] GitHub Pages URL 可正常訪問
