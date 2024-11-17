# NOTE

建立專案

```bash
npm init -y
```

安裝套件

```bash
npm install -D tailwindcss postcss autoprefixer vite
```

初始化 tailwindcss+postcss

```bash
npx tailwindcss init -p
```

重要!!修改`tailwind.config.js`，設定`content`正確的路徑:

> 假設 index.html 在根目錄，可以這樣設定:

```js
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ['./index.html', './src/**/*.{js,ts,jsx,tsx}'],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

修改 package.json，加入`scripts`:

```json
{
  "scripts": {
    "dev": "vite"
  }
}
```

啟動開發伺服器

```bash
npm run dev
```

vscode 安裝 [Live Preview 套件](https://marketplace.visualstudio.com/items?itemName=ms-vscode.live-server)

用 Command(Ctrl)+Shift+P 開啟 vscode 命令選擇區，輸入 "Simple Browser: Show"，即可開啟瀏覽器預覽。
但它功能比原本的 Live Server 少很多，要開發應用程式還是要使用外部的瀏覽器。
