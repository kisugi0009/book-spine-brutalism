# 書背厚度計算機

一個印刷業用的書背厚度計算工具，Brutalism 風格介面，單一 HTML 檔案，無需安裝任何套件。

---

## 功能

- 支援最多 5 種紙張同時計算
- 每種紙張可輸入紙張名稱（選填）、頁數、條數/張
- 內建紙張條數對照表，點 `?` 按鈕開啟查閱，可搜尋過濾，點選自動帶入條數與紙張名稱
- 即時顯示合計厚度與書背厚度（合計 + 1mm 裝訂誤差）

## 計算方式

每種紙張個別計算後加總：

```
書背厚度 = Σ ( 條數 × (頁數 ÷ 2) ÷ 100 ) + 1mm
```

## 使用方式

直接以瀏覽器開啟 `book-spine-brutalism.html`，或透過 GitHub Pages 存取。

### GitHub Pages

```
https://kisugi0009.github.io/book-spine-brutalism/book-spine-brutalism.html
```

## 技術

- [Tailwind CSS](https://tailwindcss.com)（`@tailwindcss/browser@4` CDN，無需建置流程）
- [Space Mono](https://fonts.google.com/specimen/Space+Mono) + [Inter](https://fonts.google.com/specimen/Inter)（Google Fonts）
- 純 Vanilla JS，無任何框架相依

## 授權

MIT
