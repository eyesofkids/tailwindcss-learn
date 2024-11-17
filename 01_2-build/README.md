# 1_2

需要加上`-i`，代表输入文件，`-o`代表输出文件，`--watch`代表监听文件变化。

```bash
npx tailwindcss build -i ./css/tailwind.css -o ./build/tailwind.css --watch
```

另外這個資料夾中需要有`tailwind.config.js`，可以透過`npx tailwindcss init`來產生。需要定義`content`正確的路徑。

例如 html 和 js 檔案，目前 index.html 和 index.js 都在根目錄，所以可以這樣設定:

> `tailwind.config.js`

```js
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ['./**/*.{html,js}'],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

不然會出現以下錯誤:

```text
warn - No utility classes were detected in your source files. If this is unexpected, double-check the `content` option in your Tailwind CSS configuration.
warn - https://tailwindcss.com/docs/content-configuration
```

## 參考資料

Tailwind CSS Standalone CLI，不需要在 node.js 中使用，可以直接使用 CLI:

說明: https://tailwindcss.com/blog/standalone-cli

下載 CLI: https://github.com/tailwindlabs/tailwindcss/releases/

```bash
# Create a tailwind.config.js file
./tailwindcss init

# Start a watcher
./tailwindcss -i input.css -o output.css --watch

# Compile and minify your CSS for production
./tailwindcss -i input.css -o output.css --minify
```
