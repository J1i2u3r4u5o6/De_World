# De World 角色介紹網站

這是一個可部署的單頁靜態網站，使用 HTML、CSS、JavaScript 製作，不需要後端，也不需要安裝套件。

## 檔案結構

```text
De World/
├─ index.html
├─ style.css
├─ script.js
├─ README.md
└─ assets/
   └─ images/
      ├─ hero-bg.svg
      ├─ character-placeholder-1.svg
      ├─ character-placeholder-2.svg
      ├─ character-placeholder-3.svg
      ├─ member-placeholder.svg
      └─ qr-placeholder.svg
```

## 如何執行

直接用瀏覽器開啟 `index.html` 即可。

在 VSCode 中也可以安裝 Live Server 擴充功能，對 `index.html` 按右鍵選擇 `Open with Live Server`。

## 如何替換圖片

所有圖片建議放在：

```text
assets/images/
```

### 替換首頁背景

1. 將你的背景圖放進 `assets/images/`
2. 開啟 `style.css`
3. 找到 `.hero` 裡面的這行：

```css
url("assets/images/hero-bg.svg");
```

4. 改成你的圖片檔名，例如：

```css
url("assets/images/my-background.jpg");
```

### 替換角色圖片

開啟 `index.html`，搜尋 `character-placeholder`，把 `src` 改成你的角色圖片路徑。

範例：

```html
<img src="assets/images/character-1.png" alt="角色一圖片" />
```

### 替換組員照片

開啟 `index.html`，搜尋 `member-placeholder.svg`，把 `src` 改成你的組員照片路徑。

範例：

```html
<img src="assets/images/member-1.jpg" alt="組員一照片" />
```

### 替換 QR Code

1. 將真正的 QR Code 圖片放進 `assets/images/`
2. 開啟 `index.html`
3. 搜尋 `qr-placeholder.svg`
4. 改成你的 QR Code 圖片路徑

範例：

```html
<img class="qr-image" src="assets/images/de-world-qr.png" alt="De World QR Code" />
```

## 如何部署

這是純靜態網站，可以部署到：

- GitHub Pages
- Vercel
- Netlify

部署時請把整個資料夾上傳，入口檔案是 `index.html`。
